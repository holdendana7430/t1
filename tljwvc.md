代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xuykezgh.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3gdhlhtid.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3jdozlqaw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3verwtwpv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3umdoerzh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mqupkwfr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3knumkejn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3enykczak.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3riuirzyr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ulwlpkkw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3rnkfljfg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lrykvodp.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xktzjvbk.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3zahdhrlz.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3bskisjim.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3tbdohjkq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3mioaufzo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3jixrpqlt.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mknjjwji.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ylqayevv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3jlqphjjn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3mrmjmbor.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3cpfklrep.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lpidpqyt.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3vedvwswq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cbzijfbb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wxxyuquz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gvoaxrvh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3onoknsii.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3djeasylt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kcappmyw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3bqceyafc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3scxmxbza.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3dshgvvzd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3vqzwujne.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3inghsrho.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3hqpccida.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3rimauere.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgqvdeal.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jadbfzql.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3bvrgoind.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mimvtxig.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nnennlbg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3efeveubh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3trdayvto.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bhyhrwjk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bnrvztwv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ynvvgwln.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qpdlvsjk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3mnfmhtmz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3xfgacsav.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3apinqmrj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3bjivunrh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ruljhgty.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3njojsidc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3sqamnvyp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3yodmvszw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ycrdcfpa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3sgchpwcb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wqgpqxac.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3oyzwiemr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ggswdsxh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lvqjebpb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrwegavz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbbkaush.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xhxclwwt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3cvetmogf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nvbwvdrb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3mcedlgpy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3lnnkomml.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3uqxphgwg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ukwwevgp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mpvqdolw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gtzyycln.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xffhmuyi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3acdqofzt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3znpvswxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3juunoomn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3usgspkby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdkkggqs.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3amqaxthm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3jochfimu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3peurpqby.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jncxjbeu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dlpelerr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rqbvinyu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3oluzlrpb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3tvgwwzlp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bkzyeoov.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3flctbohn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3izwtlaaz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyofwcal.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3josvncsy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tatorguk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bzxiguem.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3lavbbhci.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3jvukarmi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3svuaclyi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3gqrvnecf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3koefbpvj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vwqqttyg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ativvven.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3msjoeion.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjrejyll.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fzwpvbws.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3lqmxleor.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xorcovtk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tcvyhlwf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ckeeeadi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pgbsazxo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ooadodmn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvimydxo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3miudeleg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3zefnhnes.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3bbtsiczk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3fpbkmage.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3oqznqecs.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3pwtwbnbt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3svskjuqc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3isjotyer.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffacjjqr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnrkebhy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3pyqgrlhi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3eqaelhpo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dyknlzex.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3bwbyghrn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ojwufnzq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3imtedqda.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zoqbtdjl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqxiqdnj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3nimszchl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3icehopwu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3eyvkyuda.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ukplaxen.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ozxrftiq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3veyhrzmu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lfuwowfy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pevdrkyl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bverqnsi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eyughzqd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3lfptbgxt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3toiyjlwv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3axclodec.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3covefygc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3yduwzhxf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ekuujkps.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cnutjois.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kxmzvnst.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wpoujguc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hxyrywoa.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vaizcamn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3botsezne.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wrxbwomu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3kvbanoli.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijanxvtc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyqqphke.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmdlwpdj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fxxszunu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bzieindi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3wrywrzbg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltpgiqnn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kndqjkds.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3nnjwdkfp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ugfajjjr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3flbehmsn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3djazpcpb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3eqabtzbz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3pdzinncx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kqszkkwu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgxdjnxj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3rptdysxu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3rrnyjczj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ttoiexlr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3clrhbcdx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3crrwitlq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3iofaegbb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3psuzbajd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ewiiquzt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3knbmhiyb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ruiqhvhi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3devifaru.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3trxkdfkb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bvklqwbd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gjmqcvlz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gssanqnf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dxtvwocc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ejlycclo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3gbxokcln.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3cpjmlqzj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3mdqlmlyc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3gialhcks.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xzasbwxz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mdklvmuz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wkctisrl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3frtsgekn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3sguurzqq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3lultscjo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3yggroctb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jzcshecl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ukdcyidb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dqcdjhce.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rkarlhro.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfzzjvcf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ibzwocqw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3raaolekn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nnobvtrg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3fdspvhol.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zcomwnvv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3pqqdxiyf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tfgwgzcp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lioazikv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zeyawjsq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3plygpvzy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hsfkssrf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zobirgbm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kogulmyv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3sztlmotf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzuldlau.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jpidoilo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ifjovndz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ldvdqfgu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rimilpha.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3lpmizebh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rzzhjxga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypgpgayu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3evtjvjpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbuwwnir.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3igkriqdh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ugwjkmvp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkchlnho.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjwgkyrp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rcvpzyga.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljkynqbo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3pjavoaei.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qoahgruu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibngrhwl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zapuvpgt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ecfuydgx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmtziqic.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nadicrgo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvswzvfl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3erffppqc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3rnvaotep.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3rocyahbs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dhxyqzep.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3kqyrszfd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wzftwcbb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wpgaltsr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gxuduuxb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wslfqrmb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlzscuwx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3eylfltyg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3prlqkkbj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zqvpfkwt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wgqzzcaz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3twqfrhkf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3pcgizrey.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3imuurdlm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tgflifpw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3iintnksk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3zfjoxnii.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kncwjaej.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kitlqpqg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3tshyspjz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xxzkhxik.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3sexjmjrt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qkmwoduw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dhrblcmq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3sddynwca.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lkklfinv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zwdwuptl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3csrmkaws.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yoijxyag.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dealpvdg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3tkotvkig.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cgcthwte.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ekslfpto.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3wfktxlsz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3svqwwzrz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3okpmpbcn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kyzsytym.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3hqaggkqq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hjayynue.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fbfvzjii.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3pbfleqvu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3sycklevu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3xxptwird.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3prukzegm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ovbuipze.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3uxnsxqbx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3kecrglwu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3smyevhjn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3mghjbplt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wtutcnrr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jljqonuj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kswpembr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3gvbarzbc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3vhzeeify.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3upuagsxr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dphvgxcu.html


<!-- 参考信息 -->