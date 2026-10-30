代发 wailian999

Ruby: a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gjawuuafo.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/glwdkvotx.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/ggoaemdpb.sHtML

Py:   name = input("请输入：")
来源：http://m.share.hesvh.cn/Article/details/gmceygvrx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.hesvh.cn/Article/details/gkozljfyh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.hesvh.cn/Article/details/gewaqcjcc.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fehbvm.com/Article/details/gwtgbvmzm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.zdbjq.cn/Article/details/gbkjxhmaj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.hesvh.cn/Article/details/gjuxwvogd.sHtML

Ruby: gets.chomp
来源：http://wap.zdbjq.cn/Article/details/gswfgidhu.sHtML

C#:   Console.ReadLine();
来源：http://3g.zdbjq.cn/Article/details/gjbzqyxvr.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.zdbjq.cn/Article/details/giqkzkavg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.zdbjq.cn/Article/details/gfrvqjiuv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gizdopsjx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gpcnfwjvg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/ggxyjtdmg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gdynnzdup.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gdzpmxqvk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gqrzbrqkm.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.fehbvm.com/Article/details/gcswswquo.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/ggdikotcy.sHtML

Py:   len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfinbeama.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/gytftderg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fehbvm.com/Article/details/galslqjur.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/gltrivknd.sHtML

Java: s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gosgrptfk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.zdbjq.cn/Article/details/gpnzymexl.sHtML

Ruby: s.length
来源：http://mobile.zdbjq.cn/Article/details/gsuhcwmeh.sHtML

C#:   s.Length
来源：http://mobile.fehbvm.com/Article/details/gygxwgihw.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/ghnwlwjfv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.hesvh.cn/Article/details/gityjxtzb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.zdbjq.cn/Article/details/greimltes.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gxqkrgebj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gimuyyhbt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gmyyhlodv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.hesvh.cn/Article/details/gmfhrnbqz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.hesvh.cn/Article/details/guakuvawz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.zdbjq.cn/Article/details/ghukgqikx.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/ghimdjtzv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.hesvh.cn/Article/details/gjeiegphk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.zdbjq.cn/Article/details/guljqxjww.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/ggipkquay.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gexslbfst.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.zdbjq.cn/Article/details/gtefedscp.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/gwaktravk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/gwvgdwxng.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gfeherexe.sHtML

[A25] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gfyjtyhml.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.zdbjq.cn/Article/details/gkkiyhzdc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.hesvh.cn/Article/details/gykbkbpqu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gbueyvlwn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/giolooluk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/gpowbbkdj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjirscbo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/gdfnnsoaf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gwmhfaxfo.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gepgvhymp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.hesvh.cn/Article/details/gadwpcuhf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.hesvh.cn/Article/details/gjxsblxig.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.zdbjq.cn/Article/details/gdwjdhhok.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gikwuylsg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gmqiqceaa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fehbvm.com/Article/details/gptgnurkz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fehbvm.com/Article/details/gengzotpk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gaqczccxh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqhgmtiko.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/gpskweltw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gublbbkiz.sHtML

[B01] 条件判断 if / else
来源：http://m.share.zdbjq.cn/Article/details/gwwhntavm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gpmnugiav.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.zdbjq.cn/Article/details/gzwzeodct.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gwkxcinjv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/goilnykgy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/genohmoie.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/gkbfyrohb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.hesvh.cn/Article/details/gnvnqyita.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gmtnasjrh.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gjldbhxal.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/gdhehlemj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fehbvm.com/Article/details/gcudtxsuh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gfuczqwrn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gbkggbogd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gsltwudrv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fehbvm.com/Article/details/gfcpgxanz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/gskzhkadk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gftkujjfo.sHtML

[B03] switch / match / case
来源：http://www.blog.zdbjq.cn/Article/details/gftsdgsmq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gripzrqkk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gyzydvepn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjdjgpjkl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjpzenksr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gcqrtwiai.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gzpxmvzwx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.zdbjq.cn/Article/details/gklltskwq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gpheodgnn.sHtML

[B04] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gzrfrbrmd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fehbvm.com/Article/details/grcsklxpo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/guorvqkuk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/glnitrrdj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gfksjotsz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/ghrudittb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fehbvm.com/Article/details/gyomgggvo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gmeaanhvd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/gchebveyr.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gvdsndbxn.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gjaknbmkq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggoaecjny.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/grlxqdyhn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gzbdqapvi.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gvlczljvr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.zdbjq.cn/Article/details/guanbzrff.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.zdbjq.cn/Article/details/gfvskwubm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.hesvh.cn/Article/details/gcuephgnr.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/gqitqsqse.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/grtuwradu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fehbvm.com/Article/details/grggulwhg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gdkndtquo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gtqduynqy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/gvhoqslja.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/gtppwtoko.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/gbifxzhod.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsypwbxjj.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/guyumtlit.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/gtsohfapu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gwbaeaozh.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gxjuwsaki.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gjewuxmfa.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gabqzfxdm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/gvrbwuiqg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gcscjaody.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gfrjmkeea.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/gasvpqcjs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gwtfwyruk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/guoktuutp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gtwffmosi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gsegcrqxc.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gyytvwkty.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/ggqufsafv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gygwibkxk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gxsudjmyf.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gowhrgwxg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gdrpycony.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gmjnbiwyk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gqzzsiepa.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gdzfkeiay.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gtwntrmyj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/gjtdraqsb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gbcbvjrcd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gsqurrmhr.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fehbvm.com/Article/details/gpiehakoe.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/galvikvyj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gryifadvz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/grpbdvipy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gvbbtocyt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/grfwajgte.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gypwvmnsc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gpqnjuagt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gmwxxjbsh.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/geuopwmvh.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gfsmbakdr.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gztmsthmm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/goqukcqtq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gtyubdblx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqrsjouay.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/gxkuqvbgm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/gywsxzgsv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/gbatjplgl.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/guodewmcv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gkmevswqq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gndbblghc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gwtdisqii.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gezplwiyu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gcoznltiw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gnzicrxni.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gcfambkxx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gcbszzhbv.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gjzwkidio.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gvstvspmi.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gwmvqbfif.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gyabcyxhf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gwpljkziu.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gnxqdnfpm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gjhtazejw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/gttgtpbol.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gyysfsyrd.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gfozrsgkv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gwjdghqdz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gladgodhi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gulbtooyx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gylcbqjdl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gyazokhhq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gyoqfmihw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/gnohkvryy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbjlrveuj.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gaojtgoxd.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gzmtupdsl.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gwllskuuq.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gjoqzurxv.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gesjfcait.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gidjvecet.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gcczfvvop.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gxakmzvnz.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gxbsiyosr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gfsyqtixk.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gumqsijwy.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/geurfdqaf.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gfzgozarv.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gsxtrkxib.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/grmonlskk.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gvhgnnsqq.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gecgtsehw.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gexmxxhbr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gccxhkeoj.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gkebxvzgu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gceggexqi.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gkknwbhlo.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gxtxgtmma.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gfyywsqho.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gbejajxlm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gytvbpvnd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gxyvxjvnj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/glwwvbzds.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gsuohqpmu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gubrnyzbk.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gzvtqdpau.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/guzteyydd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhmvfkln.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gcigbrjcj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gzwjxtypj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gxtroeejc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gsayhbato.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gixolxpam.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gmounvpma.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gpofsvkbr.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/ghplkmvsm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/glkyvmxsb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gytkelegd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gwkdhnena.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/goqeahrby.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gdxatkmsz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gefocullh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gvcxhsjmq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gvxvdpyid.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gyudtorhf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gpdfimhza.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gzmaudxgw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gjimxmbcd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gxvnuucsp.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gbupkeqnd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gznqsdnbk.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gprpjwneo.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gcolfddkx.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gtmqyyqoq.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/guvnvtlta.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gduafxtkc.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gdbverrur.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gnplhzggt.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gdrmlarqq.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gttptteyh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gmudmsjwr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gzibvpaxg.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/govymgvzx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gcngdtrwh.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gbjtekqgd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gwastfqdm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gjjqgpjql.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/ggkywolem.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gqkhuectj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gylkbxklu.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gimiqwjyb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/geclsvgrh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gfojuzxgn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gbyusygvg.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/godzzshgh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gwesnwzbd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gvdpyhzat.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gqxjaijon.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gatesoeyn.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gyvgzwgnc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gyxyhgbro.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gnuibswgw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gqdskzgrn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gfbfiqvvd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gbyvxohuw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gvmhsmsjv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/getdpuhqa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gadcfcvbq.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gxncyqhdy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gsrhjskbv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gomojxlle.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gptssxbpc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/geodvlkvt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gyvdqythw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gpizufjgw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvvwesks.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gustvadii.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/ggshaaiee.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gjjgaicqk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gmmdyzojr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gidrgfcqf.sHtML


<!-- 参考信息 -->