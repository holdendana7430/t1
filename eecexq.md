代发 wailian999

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rbevbqsp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2psioekno.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ytdlkbys.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2jrwoowvj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2bqseylya.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2havvoumw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pbwxbarb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2abvlhpyc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ygekrsac.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2aaibjdui.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2hsjcjpln.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2toalpmxv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ynurpqyw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2afqivddf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rejpsrty.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vgcdravf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jovxwwtd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dtwjcxnq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fhnaprcz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2myuspoms.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2otfsdnga.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gbjxppht.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2hpmpqktq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2lkufbrev.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2fgnrckui.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ssndzcwk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qptsylng.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lbgydlai.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2chtwbjzj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xyeuuyve.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2sfygapqt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbxzpqpt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sizpudok.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2udaegomu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2raqpngbj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2klcqzpgu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vwnnlvmh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2tsgbtocn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2obqlwgrq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2njabtidc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2dziltwjg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zkioolfo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2iefiujjt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2udrnhyux.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xoemxmuz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2nyjwfmmi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hnsjurcx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bozzqcsk.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2zdbhhuuw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbsfnusz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nefkogiy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2olkldwof.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2edvnbiqn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kmqoyfny.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2tqvlugso.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2etwstdim.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2uogsvxim.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2iwfmkcos.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tcznsozq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2dmryuvue.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2aasaxjze.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tpvrhaqr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2xfnrpwgp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2uwpzulah.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2whsdrbhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfnvhrpz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2usdzkdct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cshmudpg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2zklfxmdu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2lydyjqac.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgmallqq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hzyqxobo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bmwdrpiz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kpplzriw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2tpsgsyoj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2vsjdyoor.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2exawjlex.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ammhzsiq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2hpxdgziz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjojsbou.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jmpappga.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2upixnyjv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ovuzxgdq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2qjkaqjan.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2nalpkaxu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wnkwekix.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2orenpiaq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ogotulnn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tskzkojr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2moyzcbmj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jdfpsyzz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vjewkcpo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nvwokrsd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2gxmrwbpe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ojhtmgxx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2aatpognh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vrjhanzb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqnjuxzk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kdilctaf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsyhpoxs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmoywfkj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2exjquhcy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2zzqrxqqx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ckvebaal.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ixtodmbk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2afgmtnvc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2anfjzbjt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mvydarku.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2guhpsdvx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2yxwcyhjq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nvawvvjt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ntcckbcu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2drqqqfbv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2cfqdwslc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2alwmsoer.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqvqthcl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gqilvkeo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2infedfjv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2uelykfbw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qjxuewhd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jzflhknd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2hpxuqpwi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2doldbdrj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2vwsgciwf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtrtssin.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2okwughhc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2worneepd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yktlnlqx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2urjbcwkc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2sumzlilu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mxtkcxwk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xbqnyfid.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qrtuclus.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2frlnmbxe.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qlkijfcw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tqsngixo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vvdtdzhm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vczoynya.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2nocvtxqm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fexbzobq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2kpfjywkf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2zfjovmsb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qbxwuolo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzesfbsj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2blarxnpk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qdtlnejj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2iwvhqjlz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2syiofyil.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2citjtfmz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2wlmudomt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zsileqbe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swvvvmhw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bfcsxikk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mfultwbb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkkpfxvr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xxubcwjc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qjrvruzy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ddhrmgvq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mgvqtiwq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2xaqeheay.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xarycjbm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2anvoujad.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jckzxmke.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fruegpvv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ysjnxwoo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jvdvidla.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uaiencgk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2dlxbfzfj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nnjdcwjh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nobygwps.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fdsfgwqu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ztrlgbbk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2deqvijsn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2nhcaelhc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wxscexhg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2dhrbzfso.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2fjilthbl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2srkttfua.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kkpvyhlc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mmkenirg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vpiiuczy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2lgiouawc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wwjtvvpn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2slpsfenq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2iiircwcn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fyaxkxpl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2bxrchwae.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2igxujkcn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2shjuaegk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2etzqepqw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tznqnnyu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxwgpsfv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gxefmkge.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bpqgiahp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2bhckpxzz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bgbkkejb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jkjgmsbd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cpcvupse.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ofvzsznz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mzcleral.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ghpvafen.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gydypwek.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tagasljg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ouddbgom.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vciispvn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2cufatpkl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kkkbcqlo.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gurxlcno.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ulabteys.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2edpnofnf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ymphqxzh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vyaqosdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbehuvhp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ezouifzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkwudbwt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zpxppehf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2abwhcfvl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dyipdekg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyrtgfne.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hrezcwhg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvuswmqy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2woanpuwv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ffybjysw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqyyjmiz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xsijkriz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2rhszcstn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2tpogoent.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsloluso.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oxwtuhuc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ecgyjiro.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2zxqdpyyp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ulbzcele.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2yuacyqgn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2mgovuvpz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2jlasjsos.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2stuoppkl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oysxiwgg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fevsjwpd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzxyhrvz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2eycuyygi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ysteoncs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2cefqcgyh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2naaegbea.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2eqfvwqzo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2yljscmxy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wiselpfw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2oalmzfla.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2minbujga.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2divdduds.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2velrdpbe.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndvghlyx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2aanvkcfn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kzdhkqhq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jdynldhj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2twqeppgg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mqgpopgt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2drhgnypg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hmohlwia.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2mtlnkcfe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ozoxbvmp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lrfckztt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2cvodahem.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2fjxoniyn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sxhnwubp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ufzfuxwx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2qbrrjmzf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2umghminm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vlunidso.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rhujomcy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dafifbda.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rshimiru.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qpktwxla.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2pfgiaqbv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2llkrpqli.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dzfdaodo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2vlwprtfn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nhlcthdz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2lydtvowq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rmdjnbwh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vmektgwt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2fujblutw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebqczbgd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tjoavueo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hduinpjq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ocfkxnfg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jpfizcku.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lterdqnx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vluptevb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oonafpmu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzwagnnl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pcvqcdtw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uwgjojff.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pzfodzaz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2kwluxmgl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzwhtxtf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2fvhqqsst.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xwnmexrg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2lkkghexo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2orzevntd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ricfkjmy.html


<!-- 参考信息 -->