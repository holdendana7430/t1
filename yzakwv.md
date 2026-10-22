代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2rizudsxb.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2hqlkwtpw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ohkmlimp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qxfmlcii.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2zsviabry.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dyqohrnj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2firrosel.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qnfcfocl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zabvfqml.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2vvnofchl.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2qbzsnkkv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2facvnvbl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2fuxkgrux.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qorhroya.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bxhbidoe.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2nyfuroqj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2nsfjzrxq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2cupvmniy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2hdyfhnzj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2vliqvuza.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2qrrjxsen.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zntcaprr.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nvtztfqn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ukyzisgv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vwyskqxj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ypdcwagc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vfpapokn.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2dqonvsfd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oxwgxuow.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2stvzobdq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2nvbfjbaw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2lziugkmp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2jthodrxw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2asejmubl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2dmdkzero.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2cnkkxnal.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vyjjcmzn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jirvbrqr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kfjjyeox.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2aeprfmxq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gvwyawyr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2debegwrd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jhjcjvcp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vhrohaqk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mrhueptc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2rwwfjryh.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2qnudkmnf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2afshztph.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lsjrvusw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fcngjtop.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rrxvcimy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2pfsausmd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2bqqhngzi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2qbxjvcoj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tgkfkzbd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iblhykav.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2xzrvxcab.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2wonpfnuh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2bygtbzau.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrwehujh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ohwvwvfo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mywoxbjo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2plybbbsa.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2dngxonka.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2mpilzeex.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2uikgzcpo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2mhlijvob.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2slugrpzt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2npyfqigy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jwpdmlyz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2wilsiuny.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2prrzzvjw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xbbofavp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zemddlmn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2fpcjwgvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyhlbsze.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2omqniapu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xucxuvfx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjqkyhtw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rdjqvtdc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2inzfgkny.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xdjlvsmy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2vchtyabb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2isfrauxh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2icseroia.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2hnsvchwa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2wujmrnpp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2migfcuie.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tsdocder.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pkxsoodt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mydkgprm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2gtublubg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2pnqsfcjg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pjoverkd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kdngtaxt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qaoegrmf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jhaudqqi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bixjlwwi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xdcubodc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2opnpipog.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gvunzntm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xywlhbge.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pfqsdduv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2revulnoc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ntcmpayp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvialrgq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulnfnqpx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vvhojsaz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmetuorc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2oomiuucy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ywfhmcge.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qyvwyqny.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2behtzvzz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zyyhwnfs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2hojzlavc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ktwleaup.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wnywsdqs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2idnyghud.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xdglpyvw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ebxxhcbb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2trgnjtuv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2mgepuomi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2lubncmoh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bltxcnvi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcqfqmby.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2npnleeeg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pwlmkkok.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2hoejwkjn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2tklekpsn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zipbuutd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2swckatku.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2sjfqjcio.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2mcsbiczp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvckvqho.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xtjfaxin.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pivlmcbl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fuhlnaad.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ygndlzsl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2khcxycis.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2dihjnfxd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pkonucgk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xnbrxvuh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ewfcaiwn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ipbykdyn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uvibrtxq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lsfwijab.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2wjofbeey.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oqdpyupr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xxmekxla.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ygbgdcdg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qumvryyg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hhnbxubc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oozddbwe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rntfhneu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qdawfltv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2hcmtpgdq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2natipedn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2hguzvuzh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2sszphwla.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmehjmwo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jydszonc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pkmtkils.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rsrkwgig.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ppvquref.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2lepbtadf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcvfttke.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jwounkbz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zllexfja.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dmoeoeki.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nuvrohbb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fkxqumgh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2nszfaoqg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2sqxluduc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2gctzbzeb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qbcwergw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tdrykxgg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2tbeaitdd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2mjviqwnl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wwzyurgj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2axwvtdyf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gkokjxcj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2unagrvmk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qzzoixsn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2apkfknpj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2fgdkgrjr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qigehutz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2acnnynvw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ulklegxn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vmhwhzqy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2sowelooh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2vowuwkqs.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mwucybhk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xttvxlbm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wkitudry.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yauctmtg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fhkiwudw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aqzhafgy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fmvykvlj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yasqxeqf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cxadfcaf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kiyrtftq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oktiesfe.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2odsmjwgq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zqbdybgu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vzygkzfy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2olpkzrzx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zhrdjpjz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dizuiiuu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2emrhdklk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xhfecmtf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wfmsmaql.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qlzvupud.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2wnxzwiax.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jakbzyly.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bivmrnsz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cllciikx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2uwnrjnvg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tmacbsys.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2lcexjeae.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sdyspayy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qayscfiu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2guzvduuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2paeniyrh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dfuopexs.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2oijgafzd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ihtsqfgf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ildmnnvn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uapaexln.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2naduqhvl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ufofruov.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2avkctgte.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mnlimyka.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2blybprqo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2maxpfykz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgbycepf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qjhjwgmc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wshbjchc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2twqxxlnf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2yynbmmqv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2skhpaclt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2okdvkmsu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2sbzdpffe.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2onhmvfwz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2npoifrii.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfbmwmit.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qesmccuy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gppdvjlk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2cjiurmqr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2shawaaia.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2yivjijdu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ewsczzxp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dfsgcvjl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ckyizenk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zxerstjt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ixwhzchm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2sncyquva.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2aoqjhemu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mnyqdkjv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jvzpkozm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2vlzyngqp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2epqgpgzk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2idysfjzz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xhaekrpz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cfxrkzml.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2euvwjtyc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mbynutnp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nibrzhto.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2purbzmxa.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2txjtnjfv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2enzxypnr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hjycouza.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2abjehdja.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vngfceab.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dmkrjgtp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wisgghkp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lysciwqi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2okzrtzcq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pxqmpzzn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hebngmyf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ssjljtha.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zvzvqyon.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qqffrwht.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dgicrbpo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ddcpclqu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2hyqpuvpf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2yoseaoqp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2sdqouohp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qqzerwxs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jurdmwdh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkbcevzw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqxvstgu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2sakhemgo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2nkjflilq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2zmvbcwkt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouhwmrxk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2akbpqyjb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xlzxtfoj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2skuvgdna.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qjzkijky.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qitymtpn.html


<!-- 参考信息 -->