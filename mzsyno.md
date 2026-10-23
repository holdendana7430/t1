代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3twaoasoe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xxztoctv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3twrctfll.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3pmyhjnpn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3xiattynd.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ngtmtvws.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3iqzynjzo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3kiiotwds.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3dvvhtrrs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3iygwxqex.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3crgmicoe.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zxnepvob.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3meyuidun.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xdyqtqah.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hepinqsq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3cvmdmqni.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cnvcwsgs.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3iahrhqkg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dermfyue.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3bpdguicp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eenqfywj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fyvdipfi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3keqfcdxn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3haehbhuw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3djhevsub.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3udrkxvmj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lpouunal.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kfhansws.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ckrgjyki.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tiukqbrr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3alebzvby.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbzoomat.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qsxfziuw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3nsiwxthc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3rlvfjgox.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3defkagaf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jwkrezxg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xwqbzgvu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rjudfcgc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3pldfwhrl.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3bkaavktk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3tyihtrpn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pbfktoxv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cnrdooni.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3lzhxcnyi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ahfdpmnb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3byfanntq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bdejooov.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3hzcatrzm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xuqcheab.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ptnwdfmu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jajcaexu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3gaoqeehz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3guhzhdcy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3qptnqcgn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3agvrpuew.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3drtvmbyu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dephapdn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3rhwqtdjr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sqarhqhx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hsdpovkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhnpqflz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3fwtzvkxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xeftwlqb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ogdxddmr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3sbvzksgl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3cyhdnnhq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uchlrjld.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3timqwyuh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lefbdevl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3wiykgdla.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ixzbnzya.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rtkmnltw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3jcdmohut.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3mbzzshck.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3lcayixff.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3faazwueh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3edccbbum.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pmasupvb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vlzlqsux.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3mqfnzqvj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3suguxuzp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3fhpfegvz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3kcqrrynn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jzpccicp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3znsnqbxo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mibpbwob.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tzuomgbx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xgjniqhp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3mczkdemt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zavqsfck.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vkmuijtf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zjglmtbm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3bhaxoipu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqgyswsg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ibjbptow.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3apwzqcsw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3myhnuphw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zlmrreus.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3qoxgtpfj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bfofdqpc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3mjikhnfi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwknndff.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbnwvlzt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqltskso.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbrqmdmb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zmnqfuep.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3itpexnot.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubyhsmrk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zjgpeffv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qovxvylb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ksfinaxq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ivwaales.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3udjjbcbb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3fndwfcwf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3caihosra.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tcbblyfm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjvezhct.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nvvzaqru.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ozkjatpf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvijxnlp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jgnqzrco.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3oftefovy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzxarrur.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qjfzhwep.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yrlvxsiw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfawhihx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3rnfhfecj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jmhvkmqe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3frasfegr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jdgbdcca.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3doalusom.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3iguqyvpp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3aicfvxpt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ptgdkjzu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sgozlkmx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3kvvsgjyp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3vcsecyhd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ofappddn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucijmbld.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xbururbc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vrwcnyht.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dagjoxac.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3kokczagz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3erhywftr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3npzkkibd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3drqucyli.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3bnkszold.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3byicmemj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nfphxdpv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3frfhzmcm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mtlhlunv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cwgxpchq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqcuohvw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nrokuxxq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3fbhekujr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3pfnwmhez.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qhuztqtf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lmztqsav.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hhzupaxx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3kqdcocpb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3soqnmhmv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3vbmbefxn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3vofrlwym.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fmqqldqq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bujqtnvs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ztjsduis.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lqzumcid.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sdyxgwyr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3sbdkihcr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3srnzmufc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3cehwtziy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mkqgapvs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3gqebtpgy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3yifgtjnb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vhfrobfj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3envdlgyh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3mhwmxifb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fdakjubo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3npfiveda.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ysgzenvt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3udzhfjsn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3snwsfcpi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3igulbmtn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zngrijfy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jcblqmpx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3faxhlgdy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xumcnelx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jahzyigb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3reukjijz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3tllmgjyg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fzomqxgf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3squkpvyn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3edhjglvx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ixkqtjuh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tasaratk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mtvfkydb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jtpwydhq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bwpedflq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ynlkslph.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zkglrphk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3oruaiuoa.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cbauribp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qlokbjdv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uffgqwgs.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ddoyosgk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3teqssper.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lhweaewi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysihjgkr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3puzfzkpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxqoxolj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tvfpqnjn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ffnvdotf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvqshhzc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgkkyjkz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukouipmo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xidgrxvi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3cpjaorge.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3kavopjfb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oywpzfed.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3orlaygbq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ihfpmaej.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovmgaeum.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkbtqzjf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kpkcgbpy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3tonxbbsn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wmmmeoov.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gslyalyb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3uhxaecqk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ciheekgu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3trzowcsj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpzyuzph.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gxgtxbry.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3msaxcyai.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkqvmuxx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3eqckrjwz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3uyvosaht.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3apwnsjdf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qifxbgqf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3aopsbcbo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3onyfcznn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3csamtwyh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sgvsysqu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3miofgndy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3lddgtbhn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tuxnpguf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jeswmcue.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ajbepzjk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ghpntttb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3nhwcktuc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rrmseqdy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gmofmscd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3slcxypbi.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gxyotcog.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3laggrnhb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gnzjslub.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3lmhlivcx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3agawysts.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3suicskhn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zyarvqwd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3onnstejv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kwayeeyu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bgwtqjji.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3svfttztw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3inezechy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jsmlcouf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3xemenawx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kghgqdzm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3qxhutngf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3jukwlbhh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3cmfihxzd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3crfqmqet.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3lfxdzywy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3kgitcsww.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3oukbdiza.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zezncobz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hnjvaflx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3buoogyjf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ntqeyrzy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3benyzczd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3yrtoxqqu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ufptfskp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fkllissb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3dqgrabzq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlwimusd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rekkeoan.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lxxltdiu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oozfwest.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kejtiifz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ssirdgag.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufexklvg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3zbtxxqbn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mnitkekp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3pwbkbyxq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3eywwatsh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3enmtjefw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3cwgkgklx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3orarypnj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kftorrcc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3dbvoyacw.html


<!-- 参考信息 -->