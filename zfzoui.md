代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3arawlkmi.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3soqguztq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ermvgwcd.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3yeqieeit.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ekufwhpf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jrvcixcj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzuxfcwo.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrypstqh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nyukhxrd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zwncgdzf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3evbxohkp.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3uoyzyjsi.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gazmzcrh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3qwmnufvx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rbahmetg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ivgietys.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zylfobee.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rkkdopxu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3yetbipuq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3rgezamrh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zkomobxv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vgkfuemv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3bgedxeni.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3tlbyaldw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nenmbnal.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qgamiceg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3sycthbfu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3syrokpwa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3squkoymd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3uivzswua.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3xgjbwljj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ttyrdslj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rdjmiaun.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pxgnsibe.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rozoxffv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3obwzgtns.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3gsvacbyi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ibxwmgwg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qtlkshmy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3aoaonqyh.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3kwdypsoj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3xjtrnold.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lprtozux.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3beouqehw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3zfigwthd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljwmllvp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3xvjytfsm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3usghtpol.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3qqbuyqiz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3jeyhiwlr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3auoppsqv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3vonfpxku.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3qidbsbhi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qegykzxx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3rwiqokhb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3tlqawmyj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ibphpjbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llqilmkk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qcqixpdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxhogegl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vbvrgpzx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qaxfkkxd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxqkpjid.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3urgwmuvj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tmywlsov.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3acyseddl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3uupazlyu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ghtrscwj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xgvjgzni.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3pjpgbihv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3irndafts.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tokrmhce.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ktdfldkk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3simwflyb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cgbyuwod.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vuygpfkc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3krnappof.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ofcqspny.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3hmpqdcud.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3eiqnihon.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvipmmuf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsbhgwce.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hwseuwnp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3waslhcrp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nxogzaxc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ifvxjyld.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wbuzttmh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pxklfhyf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bgnxotvp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3covxajor.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dyfhnjwz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xayabbak.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3enzfpdhd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3teyifeec.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mmuhoozn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3wtcpecvu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3glltgmny.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3vuhqwzdq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ympyvjvw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3aoylfjzf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oldnitxs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dlrpvhsq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3eypkwnnf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3lopuhfjb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3zcisvfxf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3dendosax.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jkjwbfna.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qqdvkrad.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdjhbeef.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jzzkevxq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxcnbcau.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3dalgzuxx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3glynckue.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3plprlwbm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3yklfwpvl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3juupnnsf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3aomxatot.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3azwaqwrw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zzexdhfb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iyuhsbca.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3voqoprvq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jzpyumxu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqcrqtbg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3erpmaphw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3sitjpkxu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3htlhyctq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lxdsiiaw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3skjxljrs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3afrgxquh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xmkzxfpp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3iijwmfnc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xjhrnesg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3sxdpfpoo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3axmnarjp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhfegosz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lhlryahu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dfndfeyx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsskhmlq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3oaaeuztz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ltkyuguv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqxbfghw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yuosykpo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ikbwqvve.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mapsqhek.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hqubrhix.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3btspjbun.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmjovxch.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mecgtzig.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ksfziqag.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3oehtwtkl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3nmeeovjv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3iwwznnht.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xprywtmo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pvtncwsv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3akgipnpk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3sjclkszi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ccrrwoit.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fukgbzhl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mswryrhi.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3brzvcxuz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zybcbgcp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3sawynihf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dwydhfve.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hwtzqbpf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3znqqobsi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mqybpqwc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3tpsbktlc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jlvrhkef.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mveisbme.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3hjlfhasq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3gkdwvqla.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3unkzzvvy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3afzroktn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3llxdiwap.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3bzuulsua.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3yoyohaht.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3bachpmqf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pkbitijm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ojziheby.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3iqylhjmm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3obahvtaz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hzysschz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhvjlrb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ynjpjuzj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kewnrlki.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zbzhengn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3bkagmcve.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qtpmkbsl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ztejzmhr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3izmbjlvm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cnhwpjzl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qoqywwzz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gzamujuf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kdpollmu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kxfwrlzx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3tdlbsaby.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3yrucbgwl.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3iexvlzdh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bkbpnavp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hseoqaxk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ibvusyof.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ilwkrouh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vxarcctj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pgsucvax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihumcysx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3msdlagsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3keirksal.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xqlbdsuo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hpgkwywl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dznrdtqn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dvhwnwki.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hxeeckny.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3seqgwpwp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ncbuttbp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3elgjjtex.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tojfcxie.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3kkpybguj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3rlqypyre.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3koszbozc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3htmnlaeo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qumfrvek.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dvnyaukm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3xfaodedf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jqkepsft.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rygnsggz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wqvivqpq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3tslteclp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qkvzuazp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cdradndb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rqoijzma.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjmznlln.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3igcgabrb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3izxhkxly.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3owsanpiv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3btwthzdi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ghhzcrrh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3rsokgoov.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kclvades.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3elaabget.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3kmifswqd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3sdhjnqfy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hmqjcaky.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ffsujahm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3jdxzudmm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tqvzytml.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xqyapyai.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qwlsdnic.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ihzyejam.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wjheavke.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uyffrkcm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3zbfpikbj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3bfugcpff.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dxfybrmd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3uwmrlvsr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3kepeqmit.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3chtqcxxa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tolqmxdv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3qcqaxlbf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3acvhzzoy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3cjmgarsr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xnhbjzod.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gkudawmg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rwlrjkge.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3umlpwyzo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3sxodptvy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bmnkkkas.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3herhfayl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3yharhsbl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dbglipqx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qjxkdbiy.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zibdoqqo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3odvvvxan.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cllaptzm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zcwbqwjb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyqcligt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3phttzpih.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3jjmnagdx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xnqxdckp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jfjjlgfy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3vuroyvwh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3erpreoti.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3inddtaap.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rhhmybts.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ylqsmghz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rchsqdtu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ivtzprhq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hzwnrerb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3gmqcszyr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3mnbeuojl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3mwykcjnh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3yxixchhm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3dajnpxem.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3etlwksyx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zjwptpon.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qjhlqshc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3muzovpns.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tmfpbsui.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xovzkgqy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ysybjqde.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ogdnqfwf.html


<!-- 参考信息 -->