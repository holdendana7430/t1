代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nzlnelbs.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2rbdpxfco.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2psutnmwk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rdqnyxdf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2aozidopz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2bumbiscn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gvrmqctz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ksegjiwh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2yipdnulo.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qmcjbftz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2pqesgyon.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vkpnrcek.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uzqddbto.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2luawhjhb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2lvzshjgd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ovfdkbyj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ubtemrul.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2jhrtmzql.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2fmzmlufy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2vxedwyav.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2rbzonczb.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2qfzekgih.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2btmpdgyh.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2mgsbnfta.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2vbfggmzv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xsxfpwkh.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2oyeenwky.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2msjpznmo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nyevksde.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vruiztnl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dvleiopo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2xziarckc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hqdxvayg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ieczymgv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2hwlmpidn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2idezscju.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ycnvzcwr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2rfbndcgp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dsnkxxio.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ivhhgpoz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2svcjtqbr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2sstwltef.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xxsmlczh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2mgjyggpq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2unytnvsn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aqzfcvno.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pkxevpfb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2blqsvzrv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wgirqtzp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2yatjpuxz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2tmwzrrmm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2kepwvrni.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cuuiyctv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nrcramvd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vntiupoo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2fbujafza.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2xtrrbrnt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2zcgeebcm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fwfdgzst.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gozysryz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2nwgcunxp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ybpnmsin.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2nuwjyblk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghotubuf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2cdweuran.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzohzyk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2phjglyva.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hbpyhevj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2cchknqvf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2lalxsmbc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tdansadm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2rsignyys.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2rockzwdc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2flkrsszk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2qsuultiy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2iydgmodn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2csoqajdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cupfatpt.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jbmbvojh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2maehxxwh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xijqdrmt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2lvmhtsdr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2cwrqtqjc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ouvnjuns.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dvztpaea.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ymuhdsuz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2zipdjisr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wzxspucs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ahbdnpwa.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2osfgvxjq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2zmucvetl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2znvjeuhy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wyyxaale.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pbdrqkxt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jnecnusz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ajpshyap.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2jpzniixi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gurpowiu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2igmegnvo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zebgdcfe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kafvivbh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bypqbifl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsrcdsyw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yauaajdo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kcjvboto.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2mggvkbqq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hyduxatg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ixinkkdu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2whgsavlu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohehhlhx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nygljxln.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jtlcvjmi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ugvcsgjz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2bftoeljr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2lokyumeq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kyehullf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xhqpbfsh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rdgczdks.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2agbicswk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2sedwkstq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2amlygyxl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2vlutwdis.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2adagphvi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zkrzggcx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqttzuxn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2uhqvizpi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2vrrsbshp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqgvcylf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzolleku.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lxgclaid.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2mjopcxtl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2djaqylsx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2zmnrszxg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2eztxqlan.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2svgpuucu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xgzawzmu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rliusncp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzcgmxvs.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcsegykx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xitouqdk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2hhmkpglm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2buqvjnnb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrywzdnt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2dbbqmccf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2tgccfvza.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2adanszdq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bgrllvqe.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mwgjtrmz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qlkvdljt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xvtosjhf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2nuqpyfuc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qrhvdtkc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2gmbvqpet.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2cpjawbdv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgsyesbb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gaidbwvh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtwxqabb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqhfmsdu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vnwigiba.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2perlgmut.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ghvtxatm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2losnqjfs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2cynpsjws.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ginnrkgy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ykpmiydn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dbxqfnvk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mzdmdqwp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ektnvqgy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cfhuqnyv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2hwtuzkwe.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2hrfwkatq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ntdlsftt.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ddybuxwa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dljxdcvw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jhqtqapk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uxvhkanh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ffizuqld.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wnrbgwem.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wgaapgkr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qhwnrdur.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2bemgmtrp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lqkjdkig.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qwwlniiv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2atqrctcm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yyomtcya.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wnqioogq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2aoitkrws.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ahajdknn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mklsntuq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2seksdxtx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2decqxxik.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2alemkbpg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cjcimvot.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2beqwixdz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2yptcnpzk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vpvftfzb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ygpsmauu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zcppmwfq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yipdqqfc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2tgggpnge.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xidixygg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zxxsoobf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yevahriw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xstybbqm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hppyvbbn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ofymhyey.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2sxkhfhoa.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wgoahrtg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2nxjgyztn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fibfotok.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dmskbpao.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ozkvfdyg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kzbevgtg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iatedrxd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kpepdhtm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2toscxkzn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kpqgtacr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmelsmsc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2itmmhijl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rsfhyjer.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kkorslzc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2winkxcgr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wdjinrhr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xsrrwotc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjecxvux.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ubjgjkjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbxtzoas.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tijzgjre.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kzkzzqdb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxydlsyl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qliqsfoh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ancbdzgr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sdkrmufh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mwkmpulo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ddfwmwvf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdstbdpp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2idrwxoex.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xaclxvkh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcjtizkq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hkjcdvay.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nknngbhj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qykwjtyv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2hvpkcpgx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ojhjjbwm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2mhqunjtf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jwlrhlbb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2rmegdaqt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ukasmpky.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqedcxpr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2swmlssqq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcwmspba.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ozczidqn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2igocqojd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ktgglrus.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2aghhoxgu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xqfqagis.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ebymogys.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tcfmyzpw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2mvwzuhjd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fbmalpan.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nnsadtvd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hnnlgqav.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lonvyucu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gpozkycs.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jzfnhjkn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2srembaer.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vsykvbfw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uxisrwls.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2zdncrafo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bpfrzfiu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xujetajx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2pwiswzil.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2feeczytt.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2udsmazpg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2blffefnp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mvgjhfcv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bbuhfyss.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ivovourp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2slguudld.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ydfndxkk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yvdivjqj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2metmffwo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ccfntxlx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xvkafipk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2kiuszbtx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2jgpffxdx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ymfduwip.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ditimxno.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2lyzrjezo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2dcvzbziw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2swbfkmqh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2mqkbtynm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeykdtds.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xcqsdshc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrautmza.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2twtnymxj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2gufxlroi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2amnmkfgs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hdleneux.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2rfkbetsr.html


<!-- 参考信息 -->