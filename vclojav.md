代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.zdbjq.cn/Article/details/gvxzvoshk.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gvrbedrek.sHtML

C#:   Console.ReadLine();
来源：http://m.share.hesvh.cn/Article/details/gkquhnwsy.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/gcauphvdm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.zdbjq.cn/Article/details/gfvhwrnhz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gwzvnvsqm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gpluveeqv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/grofomnoa.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gxmyfgbku.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gaqjdqprg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/ggfvleeol.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fehbvm.com/Article/details/gwrqgavav.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gsqmjqwyl.sHtML

Py:   len(s)
来源：http://www.blog.fehbvm.com/Article/details/gfazecynd.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fehbvm.com/Article/details/gvfxsutpb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/gkkvnaunc.sHtML

TS:   s.length
来源：http://mobile.hesvh.cn/Article/details/genzkgsqh.sHtML

Java: s.length()
来源：http://3g.fehbvm.com/Article/details/gencrkhbs.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.zdbjq.cn/Article/details/gauwqahxc.sHtML

Ruby: s.length
来源：http://3g.zdbjq.cn/Article/details/ghvfauxmt.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/gjygcllsl.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gdipzqxga.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gyefhcvwj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.zdbjq.cn/Article/details/gsaakeznh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gaqfdgsnh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/giukrmkog.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gubfudpgl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gbeimdbbf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gevdswjbh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gwtuzlvof.sHtML

[A24] 去除首尾空白
来源：http://m.share.hesvh.cn/Article/details/grxhzbqtx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.hesvh.cn/Article/details/gfdqtzjqt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fehbvm.com/Article/details/gnnsbybqa.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/geuafkiis.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gltjqmpya.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/gvawmmohu.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.hesvh.cn/Article/details/gorucazek.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fehbvm.com/Article/details/gmdgavxuv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gdqgqrpdh.sHtML

[A25] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/ggfbgjjop.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.zdbjq.cn/Article/details/ggygpbnwv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/gsaxfmlau.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gpebeogxd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gnkhvlwnd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.hesvh.cn/Article/details/guazesqdh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gbxujpctd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fehbvm.com/Article/details/gscebxujy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gbnqkhhlu.sHtML

[A26] 类型转换总览
来源：http://mobile.hesvh.cn/Article/details/garcfeyas.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/gadvohrkk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.hesvh.cn/Article/details/gozpxoysq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.zdbjq.cn/Article/details/gczgystyx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fehbvm.com/Article/details/gfdmqyhaf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gnyrffepa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fehbvm.com/Article/details/gmbgegwso.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/gispxpdbi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gcrkvycvr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grfpfahcw.sHtML

B. 流程控制
来源：http://www.blog.fehbvm.com/Article/details/gpejuvroz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcppasjaz.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fehbvm.com/Article/details/gfvklpcju.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/gephvzpst.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwyixiver.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gmhqmjwri.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gpzuyutyb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/grxolxpkr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.hesvh.cn/Article/details/gpmqjbcld.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.zdbjq.cn/Article/details/grpmcsnag.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gewgpzcsv.sHtML

[B02] 多分支 else if / elif
来源：http://blog.hesvh.cn/Article/details/gadkhrjpt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fehbvm.com/Article/details/gdwdkqavy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.zdbjq.cn/Article/details/gmkjwlgdz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gmvodsfkm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gwlvpjqdc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gonggzuvr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/gphwpwbxg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/gyupetjht.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gnrjlyxlc.sHtML

[B03] switch / match / case
来源：http://baike.fehbvm.com/Article/details/gvkzzjkna.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gockkkfww.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjqnexnyx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gdtsyeagy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gbjwjcphn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqvbpnavh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/gkqubqjpm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.hesvh.cn/Article/details/gmvgkrwvb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gmjbrfsmn.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gdvbnyfyl.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.hesvh.cn/Article/details/gvkniqbcd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/gmdflmfku.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/ghptjswvw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gdwbybkzh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gynhgwyas.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/gdqgkxvea.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.hesvh.cn/Article/details/gvynmwacw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gptoojhjf.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gkmllrurv.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fehbvm.com/Article/details/gqcijvfic.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/gtmwojuoj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gsmclrqmt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gfrigjxid.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fehbvm.com/Article/details/gzpcsfmnx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/gybrqehaw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/gududxzpe.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gkparsmzt.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/ggxyutlyb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gkpmriflv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/giugguzrg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gbffsmara.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/glmpmmanh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gawtvnein.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gbxbgigbj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/goebhbkgm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gezrwzbog.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/giwhsiedc.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gzcnxrcco.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gkmkwwahe.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gcbwclyph.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gkqtntxyh.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gsoacreta.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gxirokobw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gnmeqvoqx.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gnalambmn.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gtlnwdjlq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gqkixlrdx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gwugubewk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/grduoxfaz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gkivzucxz.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gnfnvoekj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/grzwstkfj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gspzflkhz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gyhvlrpjb.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/glwmgqsce.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/goeajlmei.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gtbykbmmx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gnsafhgkj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/ggmzlacdb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gvcthfcuj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gghlbyxyx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gnnmldqhf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gdyqdwhsc.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/ghszrpwft.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/geayliwms.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fehbvm.com/Article/details/gfarwonef.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gqvdwbfng.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/giphococb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gusfziboy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gcqlciiqr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gzejxqaiz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/gnupilzyq.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gxxxpyqvg.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gdbfuuvhe.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gcbtfuvcs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gbkickdov.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gjeftyjfn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/ghotcsqrk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gqtolugsq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/givhfpozj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gwhkzvjkl.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gwprzchtv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gpnhxzqrv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gntkodohs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gahsaiyxq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gsvkcixgv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gskedpkrx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/gqyekwaiw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gmboxlzry.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/guswpzbrx.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gagkyhkds.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gsqpylbxh.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gsskhukyk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkkzmmwpc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gecpbfjzz.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gayejahlk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/grbfqecuq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gzhjilydy.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gpkraaahb.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gytbfgepr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/ggphsxhhq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gidvhjuvn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gtagwqhly.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gffvtzund.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/ggeqbrogs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gnnhyxsdk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gyorpnfjd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gnfeevjia.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gngjtuwtm.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gruxfulhj.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gjayetoiy.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gnryfdfxf.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gxagdtbwk.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/guwbeionc.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gvygqjphc.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gyrspqzfu.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/glvkrugir.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gmczaodbk.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gnmukbcgw.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/ggxykiave.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gjanenuch.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/guzsjxdnu.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/geeolzlum.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gziuztfld.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gffvatdfp.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gefagsakc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzdtoqpxk.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/ggeofayon.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwxpolqay.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gdtcfpsot.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gyknuuszp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gmbliyidq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gzuxblnsw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/giubigzvz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gwmpkkebl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gxiahxxkx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gswzdmrbc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/grcfkbyrn.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gsylygzny.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/guwjsfngz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gxvvuadiz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gzqbhosxw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/glvpgeino.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gibkdeirv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/gbvrsjqkm.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gceurrfoj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gbepaxmxa.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gmhgogdae.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gsplzzcxh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gabenwggq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gmjbjnjql.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gqjqdtnzs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gorwrjfjd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gujreiesn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/groqstqnj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gdahdobkh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gaasfppvw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gaanlhthe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gfyypmbcb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gekfdtqti.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gywggwkqv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gtlkbdqbd.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/ghjvcrxra.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpzgvudik.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gqevofnqb.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gqrzzfflf.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gfmtecssy.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gzxhhotpi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/grdisriob.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gumorgahp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/ghumbitpb.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gqzgldgnx.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gmpnezskg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/grgccskhm.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gggjsmeei.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gvihenfbn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gjlbwbvtx.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gerrfhods.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gkdlkqgvh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/ghugqzmfp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gaswnuifx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gyobnsnao.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/glpvtiuzv.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gvxhtknxu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gpguzxebf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gcnsbjodq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gkxpbcmyd.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gbutlbdlo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gqcdvqdcp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gwctqduti.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gkqcxxirg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/glfqrqkut.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gdderigen.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gljwcmjgu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gxnonthmh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gjvjmywns.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gjmeslhnn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/ghhjnkhsl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gdfyukokr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gqbrnuuyf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/grrqqkhtz.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gvkqodjox.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gwuipadqu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gnxqtotod.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gqwdnjpps.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/grhewsqqb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gcmfhfext.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gzcmuvnzv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gnfrvsiui.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjibzwaby.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/gpailkzad.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gkdjjdvcc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gmwpygugb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gxrlzvwru.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gqahrdlxr.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gavbuyfpe.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gappldurt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gltcmodnx.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gssfwdpyi.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gezkdvfqi.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/ggafugfsy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/ghdhfcmch.sHtML


<!-- 参考信息 -->