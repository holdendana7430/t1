代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2lxsflchc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2gwfdkzsw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2buvnlkdo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2mpbzdymp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2yjgwatzu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2gkvnfpeq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2hrhiygrl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2cgbipmjj.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2bfsvjxgh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2htndwnls.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2snlpyafr.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tchdjsem.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2iebkhlip.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pqvzsylc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ruflbcij.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ytqxzals.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tztkislz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wkwwhxvq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2skzpgptt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2eotycxjv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2rlzacavj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gzktuzhw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2idlgoshl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2pvbhpzwq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2qzudohie.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kwsezbdo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kjdzlnau.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldnyqihg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fikxorru.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tqqcnehv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ecmwwcvv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbyxtsrp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2azlksgoq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ndbjbdux.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ysjsoxym.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2gvjrysrt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2bdsqtejp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2teirguhf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2odmpkueb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2xyktcwsc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxoxrmqg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2wonordtj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2swgaprra.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2acgjrtmb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2wvufwndj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpgplodb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xuiogeim.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jxotjapu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2qmerfnrj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2dwrfcegj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vutjtgvx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rrvnfwhe.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2eixflzpr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ippoetrk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2dvhfjpzd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2mpkegccw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2dgtjkoxd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rsiiktyc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bpdjyape.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2itxaimgx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nupxzpku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcvlnmme.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2pxrpbskj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzjpmcfy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2wnsohkdj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jcqwcuck.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiiboenq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vempuxfo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oakuyqng.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2beenhbua.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2oxczpcsf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2itqgoexg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zhezntqe.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2hnqnlxzg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2teoclont.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2yzkxszzd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jjwcmelm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qqhorjkp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2avaydckt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2cgbiivff.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2opfmmumx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2npwbecwx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ielwxzfs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cceipsdp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2htojwxmg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2txhrxdix.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxjbcxzj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2whqelagz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gbehttox.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2lctyodsf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dnhikawe.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2chyzbnxf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2poasqjhw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ualsnjfp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2sodlpwfw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2efamjvlt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2uneqiyuv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2fdwhklxf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2wanjizuz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mchtvxui.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rhsowcqa.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2jgsagcgg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrjvqbnv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pzxlavti.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hraivtqd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lprxqbnp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2keqbqsgu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2fuwmaslt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ilnoypsi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vcboizud.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2uiwcbtpb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vzondbio.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fgniinkk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kivnldtw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2lfvnpdml.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rujpauva.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2yusoqxie.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzljaowf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2edwrfgkc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vtwbvjev.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2uzbxqhmc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tticajii.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ufkbddkl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2akynbcwu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2epodsgul.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2oysvyfuq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vlwlffgb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hwnirhuu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pgqrjqhr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2paejweho.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2affpttea.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2atdtwgrq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2niwzukrx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2enoburnk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2kfjkxjgx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dievdjpm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2pocktpke.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2xraondai.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2efdjkvlg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjgolhdc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bugidbsg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuviwriz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kuxggrve.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2iqbnipvu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eulccyat.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rkvjsakd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2thpbkeus.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2gdyiwiwk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2joteosac.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hoxazazg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2oslpoluf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kpzzffhb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xreugwjk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqrhyzny.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2afkkjngo.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zshjvuva.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2syypvjtj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tbuxiiap.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eilwtoqq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2elzkipkh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2nghvxkie.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qboxtgma.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bymiiwyb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zhvygxqk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2pfrmefxy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2rntbsygl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gthreyon.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vuxvavyp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2howwbkhp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2aseeqgwg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2stxbxeyo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2olgcvitl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2pdeaakby.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xcofnbyj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlivlxir.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mscbanbk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jprqddbo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2glkrptfz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vrvjqpqf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2jxmacnpx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2wsfxtahe.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2sueqlizz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jiiwmpko.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ttylavbx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bbtfwcok.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2voeepxah.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmuhituv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hyptjbgr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zghycphm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xshmwuqh.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2uvagqkoj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2mnsnhkxk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ezunezwb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mqyhjzep.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fterieym.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yxlzvgye.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iodcwejv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ccqmfcjg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bvmlmrzv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2eizmdesj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2nwrfmwyt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jilxltfo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sluzxwyu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2eptlrdbo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fdonhtlh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fvgmjrnt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2thbadmtk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ymaznnvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfmvfsad.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qigctulu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzgklnid.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zfujqlui.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jrinergt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vulrvuxd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvvmtezn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2omdffhvd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pvswthen.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wfgvyodv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2djlcevbg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuiegzfs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nkiwmods.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xpsdgila.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzvbzzue.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2igypxevq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wlmdjnbx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2omubivpd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhmyqega.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2lqpxqczj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qyctwwye.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gxmvhqlx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2scitjzyv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztbmimen.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixdxdbpf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gyamowpq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fivphaxr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2iagxuhyy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2nuhcxfwo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xguayjis.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2fmkckfox.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2khmnhqhm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2paawuolb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fmfcuqon.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nihofzuo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2oivhgclx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2nkzxltzu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jccdtohz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mqrukmig.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ugzveocr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ncdqnozl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2jsxzlbla.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2uyrgvdnu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ufskbhxd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dtfehknf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2isiljnun.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hruzznnd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ffshyqgk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2uqhratvi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2opfmenao.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2fbcyrwij.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ypmvasxo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xgbeebuo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2htmzeuea.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mnjdupyw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2tgqhnvhx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2griqobly.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2zgcmnvfr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wltiveiy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2oqfgtpgs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2tissepat.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qiplfsto.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dgsqfpkm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2mmnohjhc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qnttqrml.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gcvrnmby.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bpxwlzzp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tvayxnpw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkjjiynd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qxvblzat.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqfarjmd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2jsotewew.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2jlbrfnro.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2pbpzotty.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vybvfxza.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hduqpbke.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zxlsrxpu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lpldmtti.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ojgujupf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2oaboxxqs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qfoxmezi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jjxkcjxo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhgusuzd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wzrbblkl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2pelhibid.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mjixumxw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2eenmjswb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2acggmnyt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2evurgkpm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ewzpdkyy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ahtkfxyo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ftpoqhpl.html


<!-- 参考信息 -->