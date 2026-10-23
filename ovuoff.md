代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ydzhjzkr.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3egfomvyn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3zcgnilkb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hattgztw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dkontzbd.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3jqyxgheq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3txbyapfm.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3sydcrcbu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3cowyyjbn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3gngnidzj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dpjhqchp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3nswyhcqx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3qjngupqn.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tjfbcrbk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3zdfytfpd.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3pmxfsnei.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3cpranguh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3akjhppwl.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3axpvtcur.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xwdnddci.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3irncevre.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yqlsfhgd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nxdfcdxe.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3zdrncwwv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3otixevij.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3veueemtq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3kqoutbzu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3xgsisevc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jxhimsrl.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3lnviceej.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3vsxsjdfa.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3opvpgqlo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3esjqqrvi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bhsznivn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xgbrznif.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3hbykllfn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3plgagbpj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kajbxxwt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qmjoscmn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3pmccplvh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3csmdyjne.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3wpwbzadm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3fwrfbelq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3gnhfldpj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jimreapd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cepqkgfu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3stvobamr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3fonygrvn.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3rtmtttxa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ujywmqpa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hwrnckgm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nipqgmsn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3uyintnkr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3kgnzhxaj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ehsfouzq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3kliwtirn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3tlonotox.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kqmytlod.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3tedwtdko.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qjetfvbz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3iktjqxru.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3xaposbqu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3xiwlqoyv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3swsjvjie.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3sxtnnycb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3blzeaqvq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3yfoqoxeu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3vfjuefcx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qmuigohz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oyexpsmi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xxutrycn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsfwkbjv.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3pacvgohv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hlsydtuw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lddrljec.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fojigrne.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hvxvibta.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3acthsfth.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hgmzqpsc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3novuritn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3emkltedf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xxdjmzfy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3zmmxxxph.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pihxhztr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mnxvvsmo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cdysxztx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3twudfoxt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3hqmxsjkv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3kvvtlcmv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yyoweska.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3mkdsulwi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3mkmghfzc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjxlxkby.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mxfzkjpw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmhaztki.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpckvkmq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vgvrmshe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3kglqhlxm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ppvydwfx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pxeozerl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3liwiasvb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwbvipfd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3camhpjrs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vtqemgvr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvajnxwv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3hpoukxmp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ttoaufnz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3phzqacfc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cghkypwi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3mfcdpkjq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3nsbtruht.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsoqfgjm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3frbdapkx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3onynaakj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3etzbdlum.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3wkksnntp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ucutmerp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3yqenrtjc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xegokuyp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhhnxnwi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3eemqvuqt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fyfxbglx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlszukop.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3gkfoaqku.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mepidisg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3bzztdgga.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3bjodoiwm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3wyzkfxpf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3tkxqtycx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3usdyyipa.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ekwwekua.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3smrazeco.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3whokygci.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gtzaspyz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uxbhtale.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3hindpxxu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rplntbhi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bqdomgkx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3czbivhbx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3biotogjz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3agcducvg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ixssplav.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ugnvmpzr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ujrkihzt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3xgkmdqdu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jsiwxrbd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hqrcqsdp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3axpxeyjf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbwcyfnq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3surifjlq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cohuoagv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3cljpyrpd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jofdhoqw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3drbzmqlr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3sdjdittv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmhrfofh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zopoghjl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yvrcnxbl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3zxfxvkip.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ohzkzevx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3webhwxxa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ysqgunph.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ahpwhwfl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3tbcpbzce.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gzyhqvrv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vomiljrl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zbroxxov.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tkcttfgu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3kculgwua.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xleyrbmd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qsicgnnj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dmyxruck.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ybgzdbms.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rqysrwla.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jxilidto.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ecrbxymo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3eqsxbijw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3fqeiiejz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3cwvoeolj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3qnabtshf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3uvtpckqa.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qjsuxlge.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bvffdftm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vprnigyy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hjstabrt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3sksausda.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zdahyiiw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3hsyrthwu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3icoperjl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3rsycsuqc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3akhbdrre.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wqedxmhe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mrlfotwi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bkypuvkz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urydcpzz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jvfhdbex.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykrmxkbw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bkudynle.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jzhjwsrx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3gjlzwbth.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3xgrbjpza.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kdjtzmfe.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nxsexnoa.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rtgaduto.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fcyzmfzi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ohexbjpl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3guvvgrhu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ukoznkgm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bqhfvnxd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3qeyapsor.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3omhnwslb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nkgruzaq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mjujekff.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wwsnrtat.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3eazfeznz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3swkadjzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vatdlklz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bqiejunk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtrppnpa.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3knwjfebu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3myasvvyh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3klpengyc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcbwckol.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3swwunvta.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhifhonf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zgehkrqj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3oozyzcni.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntatyvdw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3swzrhssp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ktewoefx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3rsuabrtn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpdzywnd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rfkjkhwn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3bsukepvp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fqkcwhfi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3dwnouzpj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3brpthqbn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cfuphyft.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3tjdiabdj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hiprtjrl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqxcaiux.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pxujlmyk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3uxnnmpba.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ruksnjdg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3rtbemjhh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3goeirzdk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hsgxxvim.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3kbkpilbm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qkuamueb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpmorzau.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zzqwfgzx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jjmwhhyl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gohparso.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3exacrzvp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zuksjeqy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3edddtahm.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rdwsvhfy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3chjwqzsd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3eviaswri.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kbkdpwty.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3uwnwcium.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nyejsksz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pnsqunuu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3yenbzhsl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3upfiymbn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3acjggpty.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ljuxkqlz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ksedyyhp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3avmovfxn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mwywvfif.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cftbfraj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lhmimzkm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3abfzvjop.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jrrecotd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3vcngmwgl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ycuhtnew.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3qqwwhewj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fhiestjq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3watjdcuo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zjdtsone.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3jgbhupez.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3azvymvra.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ssrmwjrn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3bkwvfckm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rwchuunk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3noykyswh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylbeadno.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3gdfenazi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3yrzgfhib.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3szldbpkj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3msggxapl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3yknsowzv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lnvvyanf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3atuzofkf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cdwiogch.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3khyrgfgf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3byuysfhs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lfuzmohq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nqrnlmib.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3eokbewmr.html


<!-- 参考信息 -->