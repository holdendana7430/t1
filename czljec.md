代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lfjjohse.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wszdruda.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2zkkpsywh.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2pmghxdxg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ffdajogx.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2dqylmhht.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2jkwcutbp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2xezwmftu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2kpjxrdga.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2evmazenw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2wrxvlktk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2axcejnmm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2jdijrnfs.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2mmtufqfq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2gvgxiacj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2rqddymdd.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2awydvesw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vpekxnse.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xievqoxr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2grnellmn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sjvupcvr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nuyurglg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yzybmomx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2xlbyugtd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fzummclw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hgqurlen.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ditfkdvk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2acwmkjfu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mavofloi.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2wgaalfff.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmnqrcth.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bidhrzjl.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ytiixena.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ccvyrycd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2yjvmndio.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hvfzouop.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mwrmoaor.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2egcjrrqo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jjbxhfaq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gphwdpeh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wsagtgyb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2qxhvqroh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2uewnqczv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2smxebxkt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zhodwrjz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wcbayqys.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vcemrlyc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2hdaiaxks.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2wiumljuw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2efcjrarf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2iqwayano.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sedxcbnu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2bkqqkwmj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrlpbhip.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mhjquimb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2srepivhd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xjfptkan.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wvlbjfrn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ucgrsdef.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2nyfjnhzx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2xmzadjfm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ctuhnjxp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2nldvvvcb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2clyrtntv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2jiowzxxu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2kdfzrbjg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2yjtmcrmn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2gebbxlig.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vqzropjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzenezea.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2uccxrkkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sktwoxxd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2kxalykdn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2llabzwqm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2okmkxmcs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hsvaddnt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2exvcmaru.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gwkppgdv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2dfatfmfi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2cmgyrhms.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gwfhhpnf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2hmymawrt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uzqbsqtt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2grjlbmah.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jxtojrxs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vwtxskpq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fthowhsc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ipofltsj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2caqptxrq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cgybvueh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hegycctg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2pgkjpbjw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ziudcoft.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2itwvebku.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2awgmdykn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hhxdbywn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wxvxueng.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hqeodjac.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mietbzzv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2eigjliwr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ufvphegu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2fhrchiri.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2igsvprft.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nvfwkpak.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2itjmiuha.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2kratfxtk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2uiygrvws.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tewcgyyd.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tmjyugrx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wfuicqul.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2imnnnhle.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2shlfvgtg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2btnweybd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ryqujtsx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ljdqqvzi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zdaddznu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2uawzrkxs.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2hyfrejev.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2zukdpjnw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uieersgg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xuefqqia.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zdezfkiy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsugzjtx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ldfltopc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2mzztfybx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2wmcsputp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2atxkymus.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qcseaaie.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ulbsapia.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iylzcuih.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bdmmtxmq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2egrvgvzt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2srvrneiu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2rinjxwwy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdxxsgqq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2gyhaewmi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qmiqaidg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2krzgoyks.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tmwxhbui.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hliznppi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fqjcmrse.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2okgartyw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2uzfvfdtw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2akfejpmq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mnqcvfmi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2sumcngpt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2djvspbjz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxqhirjm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmdapzwb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fehzmzkd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kfidyvje.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2unrxqsfy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hehmhsvu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2bsfxmmwl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2uujjurdu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ahzalguy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nuziqyun.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kxawtlqz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ouybedny.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2dclqlyls.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qbwiftxa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2amkmegkj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rsiwkdmi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2pdvkydxv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qokyboij.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ihqomvjo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yytqspeo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2schzifms.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2qwrzmdcn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2guysdjbi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2gabudlju.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2oinpwupl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qmlkzbkg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2cyvwifvl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bnoxedly.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pbxhetym.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ymuivnks.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2kfolvbqn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zlsssumf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2wzwwzfuk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qvtyjhrr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ppkaxyob.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lziusptc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2asgqulvw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjqhpwzn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2niknamlg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fevqysyt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nrsqvdhc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2upljnjox.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2sozcbnps.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ucwqifrp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ybpapmss.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sciiteih.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2peqxzyxr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihxcisec.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2opmztprt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bklawait.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lcjahoil.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2sojngjnb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2pahzjcqy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2hruakoiy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2whgmmliy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vftagitz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2brkdrgny.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xmkhnnia.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pksnxsgi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wasexdqo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gsbfpqle.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ifgsqtoh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ircojeon.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kmxnjjmu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rgvvylpf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tedehdlm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2eajkafye.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2oafmjgnj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bgkfutoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgvvfphn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mrgqncgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aclglnvo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rjugfwlu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qdpkoeve.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2swmlkweq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oixswwxx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hewlzojg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrqyttos.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tdjmmxaz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vfbmbhxb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2srixrfar.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ngyqcpvw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wzwikjsj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfzmpbom.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfhmpvsp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qicllxjk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2enoxoqbo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jxegfdya.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2tvjynclo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2fbhdaxtb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jnnpfniv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2sxlndamh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvabuwxx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyridmyz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ougkxtej.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gdxafplq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bhsukymw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ifbufznt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ipvlhiol.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2lsgxmxpu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2udewvhnu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tgfiqrqy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xfummmbd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vzexykxe.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ccctiinc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rdcpkabx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dtehisux.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nwrzhtxf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ijakhmhs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qkhnpuer.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2cvfnhjrm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ytujjiwa.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qsigoytb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2iolmhlzw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2waxscbyw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nvlnhlqa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tskyddgx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vqyqifik.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2lxowxalr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2efkjncih.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zcopdfrf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ojajdzel.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ibdkrbqs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2mrfdfyiy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2lpspqgep.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fnflhjmo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2kioymjeu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2krynuawa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2clmebdoi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mddkubvg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2jxrghzcg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jnebahmi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jzhmttgc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2omnaqwnc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2aaezcndq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qwoesqhv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2vwwnynbg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2tehpvxwu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxoeviio.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2czjsyzsi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2bkvcocqu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kpahbbln.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2edebvdef.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dycfftno.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ysikhfif.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tgdgnaez.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsnllpdw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2iwsqreda.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vcjfwbnb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2whffvzvl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2bhqgjuzw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dwtrzpbj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2fezkcbqo.html


<!-- 参考信息 -->