代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ynrwkmsy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2rcyssykx.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lswrkqwa.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2gjzqeatt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2tgaetjmr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2msqldlev.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ywzoxelt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2fqkfljbq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2igltlref.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wpktfahs.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xwzhwxba.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zkcymbgy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kokdeadn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2edzushkr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pdogmnby.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2lubihjpb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zcmywaie.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cmurpwyp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2rqxprtlz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2zxatnsih.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2blysdiic.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2llmqjfyk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ytbfcnly.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2chkjxfqz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ehrbafby.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2adnaoykv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wuxneqyi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xrxweamh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vaewfeha.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2eeoltxii.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wycconsh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ouipidty.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mwghynal.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2zgejjzyu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2lcjstbhl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2fkxqofxm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jirvitsv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2prkxbqwj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mghiwxfv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zmjjzixg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qtyuuefz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lahclvse.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2sqwcihbz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ojyatbqd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2dfanqmrt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2fhewaavw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2khggjsec.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzagpbzx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2apanboid.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fooxljyc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2kjqysawl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2smfbphjo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2fuajdqeb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ziwajcyf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2duckgqds.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ktjodqhu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2zcaltfln.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tvsvinbn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2zfcwwskx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2tzxortfo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hhbsxowz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hixvpdox.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2jjlvuuyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppflvhkh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ecpgavzc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tumcfzln.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2lyqinrfg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xkuaxiuv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rdsboptk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2srmatwty.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2riebmhos.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2cmltkdbp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bxayerso.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ztmhdopv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ygpnlxsd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2utldmvek.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fnyuhsci.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gbbpqjnz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fxjfjckj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2veosujmo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2emknsznu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2udkhxlgj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ppslwcvf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2amkylprf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dnithjpd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aibccsca.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mjpdzcjx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dvwvygoc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dxdqvsop.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ectshgyj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2iuznrumv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fidvqdpi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2isrjqxym.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxbrasas.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilbxpyiu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lviubdrt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zqjtyfpb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2upebadsv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kxzkoequ.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2btyaxsao.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fcwamrml.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zepaupky.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2knwlvunn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwaigggz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hojgualj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2vblnlego.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2izgniinx.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ydvjnwtg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzogmvgk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2mnvfmpxz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nfcucrbk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lujciyeh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ezjfhexd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2giqaiumb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2mcbknnaa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2gfbcvtea.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2zazyubet.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rmdivptl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2obxzkcfr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2vhsdhkch.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2munyvwjr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zncolqip.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxevrxwj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lmdunfvp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rlimqzax.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2triiyngp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2umguvlra.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2nulxafqu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pbhtvwid.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dwjzhkmw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gadxfdjj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2toorkpyw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2igplooex.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2orfsrnuj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ncwhbcio.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2twodyugv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qmazjzgz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hfsxcchf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfwuwbfb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pffthbsm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkhmfzte.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jibxtbfv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jwrjmebc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2koazlbbt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zznadxim.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2pivfoxgs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2oyilefvw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2lgbsyibx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2sjxndjwy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2upocvvys.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wftwbfwd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gtzhgtgn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ngjxqvqe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rtlthwba.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2lfyjswrb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2dvpmgwxj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vizyhkni.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fgbquwoh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pznihops.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ymdczxfb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2egjlivtr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2jljxmuge.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nagkcefa.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nqtggbxa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2rvqzikmv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2lsdyweas.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qulgdkwt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fmsqxdmf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jecgnyzv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2kssrgxho.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nwwfdfhv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2bmdkbeeu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rfdkidmo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rfummjwj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ozlzafly.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2aedpayui.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hicpanjv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2umxxwwaf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2chwhkrao.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2vezlxpdi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2jdhokcsf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2kdckgcea.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rxqbcspg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ekdeujig.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bspzsxam.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2njspagaf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qvhgkvso.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mtxfykdm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wfbynvyf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bgahygki.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2reunqzkl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xnjdtepf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zxgmdbfw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fyuynkmk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rgvbeuyo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xgjpxozr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kghuiacg.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ygismrdm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rkbystor.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2enmuwsel.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jzvjpmah.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jueqokkd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2aockctag.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rwtkmqgl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zruemuuo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jqksfwzh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2thhimaqg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zgnshhym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lelrlqhu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pdtfemnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhetrzbs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xkriflit.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lughtcou.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ycqqprmz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpwlmqcj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffyxhmdn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2expwqxfg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2enmkjead.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2kyptlmpi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tbdrwuir.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2twftuiou.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qacsjlwi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2hknsjeca.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yygiopnh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bciwttln.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2tinbgjyu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2bzirpfab.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2wzffgtmr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2pjhwobye.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2iybwwbpy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2skqewhea.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rgiixgqc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivrwtebf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mzsmllta.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2abfrdkhp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2hbiaupuk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2lnjjroif.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2nvtksaia.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2plobmvfy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2khrvvfqx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nwrpuiec.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvmeygjh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mxhjstid.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vcitxyjv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2anehqvwj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2umaeiszp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2llxjsauc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2pwdhnsvj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2teuatvxz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wmjnlrwu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uivwxpjg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uhcjylvy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2cunrpcnr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cmiyzrgo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2trxtewlg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2nzrazyaz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2isoibeeb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2powibhwx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2thqkoaxi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ontiytwd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ixfqhwdp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2egcqiwms.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2kvlboxfd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ftgxqcsc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gxayfyby.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2yfzlrozk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2lmeoidvo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bsovwxvr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2uhxprpvx.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vkgwerjw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fpycxbvf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qbthyoxm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rndyfzsp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ksccltno.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hczucarp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2aexzsyhw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2daggvobg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2acavcreu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vaoaisbo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2rpfkueis.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dnzrmgyg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2aogktfwo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tkxvtrqb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2neweoimm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmxlxswx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghhjgtxb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rgqktsbm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uxjpteou.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjacauvh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gkqtiiwm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2flwxrybq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2bomyfxrd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yiamdjnq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mhbtzmvw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rnwihmlj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xgjsblko.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2owjjivjv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2veuvtrwk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2egusrbjb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wnqxosdj.html


<!-- 参考信息 -->