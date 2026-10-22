代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kftsehvk.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2fxtgebbl.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2vkevygdz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rtlnwlmy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2anfkwxfc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2tnclycod.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2qkyobmpt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2hmqxkpgt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2xwqgzqga.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2uuxkhwcv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2stmxqmrr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2hcszzjkq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2eugxuxcn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2teuopbtv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2riqqofta.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2oxethwmb.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2qddmaoff.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2acobgkth.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2plzqdvpy.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2evobkkqk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jgochizz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zyjbelhu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yaruiwyv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2cpndfblf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mzfrlqlp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sejlhzua.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2wjtxpnxo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2nugrjxca.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wvpunzbf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wgmpyodr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2mqilkbvh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2tluamdeh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bcurdcvf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cknalmwg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wrtclqll.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2hiwpvfuo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jflpmcwh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fftkqjst.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2flsxrjaa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jikgwhrj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yeehibqa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2hyaxdhiu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2xfpvzkaw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2sciffopc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2fsqmnpzt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mlsxarec.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ebgjfcao.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2yueqizfm.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2nlydxhyu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2vghfdwxl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gqrmjqzq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jkcksodh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ucsqzpis.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ptgqnkvj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2cfezapmf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bpsdkukt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ztxecpwi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2swsjuxkd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2qciqfavb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmzrxwmp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2vzkfungr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2zadutpah.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2mbnwyjhn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2kuyqteff.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2cxqxenhg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hmlixtrx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2nbnvvhgt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2rkanmntj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ryycjaxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlawewgn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ndjasvej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uglgnnxi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2lbxpggmh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hxosqexo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2fciwybye.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qgcwqryk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zmsqpzqt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yjpqyhke.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2uhjyemoe.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2koelltwa.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pvdyhdhz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2mdytedgx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2kxdkcryz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhleizzg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vlsbjdac.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nsdztaww.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kmassfvq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jvbbohef.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2oxliyyxw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cwxnycnu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zhumcecq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ewqlxocw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eaqjtrat.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2loglyrbh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uaebrbur.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pjjhzqjm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2eyojywjv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ffavzbde.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tamzncsy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fowzwhwi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lwpmilwa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtlxgwcu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rmsmjjvt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ikgxsizx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2anbtygnr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2retgwzut.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qnatiydn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mxucorft.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xahpvryk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2etntbjmg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkdyiwka.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gulapqqq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbopsegb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2xazjcqgp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2bgugmrrs.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2cwquirve.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vjzzbucp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ekrqfcyf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2yfjubgro.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qpfzswzk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jazorubq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxhudqbw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2epphbrwx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gkkahusq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zcvsnbep.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2bckkkfnm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2axupclhd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2nvkfhfpr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxfojxyw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fubxynfd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ljryifti.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnfjkngj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tngaihdz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2nyqherrl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmepfqxc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rupjjtmy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2nyeubniu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2waqnstaw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jikgkxyy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2akmfpewy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xunofesu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2imukdesw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2oixbxrpc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dfrtopbf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2tkqchccj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2aebfhdck.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mwvmxqhb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cvxiskil.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wsuenxkm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfvnygtn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kxptctit.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2uiefhaav.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pnilrshk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2tliylvid.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2nsahpovu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2utospanj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2znvhdvbq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ohvcorwb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2dyohowzy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2uodmbycv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wszxspro.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2maanfwdl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2abpiywnx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2zfespmqr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uqihcfli.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gqpmljbl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ojgsrpkg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2forbsanj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2bxiyrknh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2braitfha.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qhclomap.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2bkyyhgll.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xcvyvloz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2jzxmbzrb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mpuvogtm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zassbvdq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tnlewcvc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2uyawxqml.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qelssbyc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2aubqekhf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hrrstasc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2adoqpxrw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2atpmyocg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gegebcur.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2srmrwhza.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mvolnvzj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xowiqcng.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2zabbtsfv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2oqzctcqv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2eewupucl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2namehrww.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hbuddtnd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ijfmwznl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tulucgsx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2novurfiv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2skucmgtw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vtczacbh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jupkmitc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2sszloaza.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2awbcrzqq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2bvandjgk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iiejdhts.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lrnmiwcg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ewawiwna.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2shjhglqb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hibxtrmc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ldyhhxxd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dmwoiajm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xwqrpeqr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2sklztfak.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iqzzzkjs.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wqzzsrjf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2uvqquizm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2eckrjxot.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bibhirxq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jnjswntu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjyrxjdj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mabklsug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvzkztfu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xszlqwfh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qdjydgho.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gysvxzin.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uupvcznz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lxxexfzw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bkcikyck.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2qebhcxxe.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2txhwuewk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dymuaetp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yewaqloo.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ioxecbsu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxczmgta.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hypcvbaw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjtepezi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nkkoefwu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ibkwggez.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2xwzzhupi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2vqkaxxtn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2homiudto.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2tdnyyoma.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pxxbzskw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bkyheuxd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iisuinfu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xteervux.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2cdvqjvpa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ugptilww.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2olvgfojt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ryjalmcf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2vhxjhndl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pooahikn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbelomko.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2firvzgzx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rknsawiv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ensxsyve.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yditbhvb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2irurxowq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2kfeoepfz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nwluvavu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2masptjmd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2znduobkb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hawvudrh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nwnxmcbh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2raidwkir.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2wwnsuxfj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2kgoxdwzm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2zhnymvds.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2divulwry.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2drbxnuxi.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2smwivpii.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tegirbgy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zwxphgdc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zrlrsvhx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wdvblmzi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ikazzujr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dvkkxvlw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2yzeudcre.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2keborvav.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2yncwtxoz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2dhngygnu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sedqjupk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2cskqgklm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2vqllxbpq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2tayuxpol.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2avengioj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2mftdvqnl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ddaezgwq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmoeqnvt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cporbxpw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2eebpcway.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2xbpcypxp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mvubxmjf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2idamoklu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kryhkpuf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fszoryyp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jncthqme.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gpdofljm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ejokurby.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ieyjzzgb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2oeqbsggr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qwmzuiqb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hbccwqfg.html


<!-- 参考信息 -->