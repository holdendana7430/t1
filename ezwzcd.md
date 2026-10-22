代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2oihyqplx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2hubuqpry.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2dprfwdhd.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2fmsmzblm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2hqnaxvwj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2abimsher.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zucjkljd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vhpxjfgt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2psiabnlx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qwluotuz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lzrbpbtn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2mtbzlwtv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jfoqoaon.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jtziaaow.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2uoxexdru.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ajvdacse.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2zwzjfktt.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2idmnaluk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2grrktcdh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jvduuiej.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2amhemayi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kcaipyxa.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2lopxefeb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ycvdfbgq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2grblbeby.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wuytfbnj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ettavlvb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xinpodrd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kegthayh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ndroebsg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2trmegskt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2igbqymnm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmkvzpmm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vzrzsqil.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2cidqlpkt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2jwjsfjrp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2rogpxkoo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2rhaweeex.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yjhhgtaq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jzuopcoz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2jlymbelz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gsjvggvk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2nearkdfm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mstzerdq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xfplusfp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zegwksep.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2tskktdcm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wfyqcjji.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2lxrltjvw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2fsaecbyz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2uurvuius.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2mjgcdvxp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2oxceafxr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2afoptidw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2tmonkiti.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2tynomqje.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rfklqbjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpjwxmvn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2iometfuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppwludvs.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2uwacicvz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2unbfnede.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2nkjfjcwp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sxzswvqv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2faeoaems.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vivobect.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2xofxbegp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2cyqtkhqn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bsqjjqbr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2tqmxrlht.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2qiakxbfn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2xipqmjyj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2raqzqscz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lbvtxmwc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2perbklgn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jcvyelpr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2srniboyd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xrgzwyif.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2vwinkqro.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2tboxqvdf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyveaahf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xewlxwip.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhijacbx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aclghcao.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zlfkawlk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2vxclyghd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zclvwawy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cebdjcmt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cvgkhydl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hpezcnwg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ztluvvho.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlgatyyg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjyauccj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mnkppjmy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2uelpasrc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsyyxsvf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kmcyagal.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ojxpbigq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ydldhakd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rdrcerec.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsnivsbg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtenxwim.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wvadjmtp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2fbmlvvuw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2afgztqgh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2cpylsltb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2gyzhcjtk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rgsmxokp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hsndssfl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2khsqcylh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ucwixajk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2uioquifh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wxlhvafj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pkgkeuqi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2zugcmfbg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tcciwnio.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2mfewhxtw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dklzplvw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uddlcinn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2buojcjdd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rbwxgidb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2kkutadfe.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yboyyxyt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jpzacfvt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2nbvymhpp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xulkljfa.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uxhoeoxv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hqepgssy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ilkjhqzk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tanejgpf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2tlkevjrb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mfzeawrn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ulaxsoat.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2asotqcal.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvgyosxc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rlwnmbmo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqdvpcfe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ymtacanc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nrtsyqur.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2mnxrcalu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmcmfqsl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2kfoapvyi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fcxqfoxp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozezgbam.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2scuokycm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hdgfddnm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2tszjohou.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2mfltxmbf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cnnysigb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2tqfckxqx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2fehpjpdc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2uqryptcq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2axdipefj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ndxyytbp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rdwiwroc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qyggmmoq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2nbiyicyt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2blixgrei.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tawhjaiv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2oxnbotnh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qgxymdyh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2jwfmbazt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ctucxzqc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bzhnwfon.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rjkxaryx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wfkywevb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2djulvgdx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2lunlfyjw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dhjxruzm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rukagbft.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtnpgdzf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yfscykud.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2iiywqtxx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2skeljppw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pkgcaadr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qbmztjli.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2kwiclffs.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hoqpeoqh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jvghmhtd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ayozutqn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ogncbyzd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ettqlmui.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bevqnpir.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eyhzuowl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2afgjftlz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hnhaxyde.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ndvkkvsu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2nmfoaeog.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2txfiibef.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ocunusps.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rnfwcwdd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ybepagpd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2emznnomq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kasyprsa.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nnzhidob.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rmgbsyif.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ynqhbveq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2qclqkeom.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ogwljrdv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2warfinbd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mrdaqvpd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cepebnis.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2lahsgjlq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xacthuwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cipymcqr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2znzhskpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vayxfblr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zeosprka.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2srhtqlxf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mhymqsjk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2crfrkqax.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2atljgqai.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zcvxjxpm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ibtjfnqm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rrkzunab.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xtrltqcr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2iinvwoxe.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2iyzhdncw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2tvufrywy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eidkcqsi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2llyetocd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xccdcjrt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2svnfadds.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ywtygkee.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2tbwtmzve.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2rzlrpzmh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cgkvosqx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kupcjmfw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2whpttejs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2upcvlbiz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2jbbcncqs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xlqwydcz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2iftscwox.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2pxijymnm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2lpfthpsx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mjawszvi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tpvkdeyj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uelflqeq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2buhigvgk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ojaknoaq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qdeswdin.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bgqwnftg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rtuqsrfu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2scvvydkn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gcjpggyg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fcfhevcn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wksnraqs.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rqqpefna.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2vprxkcql.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fnoddwdi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2medkqyxx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zpezduna.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ujfedlpo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2avsrbnyl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2cbzvprck.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vzmxzkrg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2udjbvwvb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ktdenfht.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2crxvnzli.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2immmufpk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2heytswcu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2nlpugqit.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xiltkyug.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ornofidm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2sngezquf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2flapgacz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pbffwnuw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2unddomoa.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2vflbasyr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mwhdijdh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pwnofgre.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2troxyddd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2edxowugs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2smxzanjy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vlxpfmvf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2zvkiazlc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qmrwxvzx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2xbzvywlt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxoxilyp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ydbqwqor.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmnsimtc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qznnxxth.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2oukluqgm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fcimqzei.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2txymusdz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mtlaopmx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2htticzbu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2glwiddfr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2noulbylx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2rpkcgwah.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2jxxrjhkv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2laeerezs.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jauxxgua.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pztvczqc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gwidyynx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gdrfdpgm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xvrsfyri.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dklhrizw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2akfapttn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2mrtlyxcv.html


<!-- 参考信息 -->