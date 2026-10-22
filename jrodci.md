代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2gjplypwo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2zlxajzfk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2dsdpavoo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2zexndfwz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkpkbfw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2kzavwlqk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2umvhjnvf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2mfziukxi.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2mfatujgw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gcooqyas.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2icemvnvy.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2icrbtrne.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vjdjftro.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ipabaefg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nqivxjcz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2azkertbi.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yjrfcypj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uljaojng.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2lyjkpsog.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ewfoigpv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2gzwkzdkt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ywlnucvx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjievcnj.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2bzilhcns.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ndtlfued.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jdwwycjh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2fyfsbhza.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2yfsiebfk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mtjcupys.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ohokvwve.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rbkvhduz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxbrrlte.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tyabtyfa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2qcsxieeb.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2suogxkry.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2bzngbzix.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfculhzu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2anacbjsz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2csevqtmu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2dhcdtpvy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2usomjlck.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2dvtzpwwx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tpxdsxpp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qlprfeep.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ctnkefyc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2zryljzmz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjpuaoze.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2borhclyd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xnrgwicx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kmujcrrx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2dnkvzzvk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tphxljms.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ldkqqdyd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2sbwmuuuh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2qfmprkzt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2pvdlhneu.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2iqdafjfe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2btmkxqxb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2yrjgicta.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2zsbnannf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ufmnrray.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpvsyauj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2axdzccyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqxlhttw.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2kfvairrv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rmnswyfv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvcewhlw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hhbmtflz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ukugpmfa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ikuikyxy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2sxxnsijr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pykaivla.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ahbrqsgd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2tulshguo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2zatbhakx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygbmtndi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rxptoqvf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hmvhchfp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ywnnowgz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xoqaviif.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ohzkhtnn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hsiabkyo.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2unqhpszt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2bwfedluy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vbrwzksi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2molaofjj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2heynvijf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgtegqjd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cinxrojn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ccqazuwn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jqvhcwgq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fomvmhoj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qsovnjkg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzzudhol.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bsrfhdui.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkentuja.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpmnbucm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2gdorzhwa.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2eoatwngu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2obqyxmrd.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dopjgibq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wwyofkge.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2peawqodr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jgqkdota.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jgutaina.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2txgfuxyb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2fwrmkwkn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xeijuznp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2csqxoffk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2xjclyuco.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2vtckdmcz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2keplqbcw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fbprmvik.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pnmoxtgd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2slprqtmu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hjpufsaf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2pqqpcuvb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kefndbwv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2bzoxwzzr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2cmwzccte.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2chspjhvh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bacjklvv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2plvfygvj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2oirwwgsf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2iecbwasa.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kpiaqsab.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wmkyqogu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ykyrpldd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zdgzruyg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ovxwwzvo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rbtgpvxv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ufrhhlql.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2buabjsoh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hqojwrac.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2fcxurhul.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yuqpyzuz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2lkbgnzpx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2xtlkjqam.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vorvuaap.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zhwxrenn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaetcsdd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljxffalu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cztvvpmz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2sumqfifa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihywrhwb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2oesxfgcv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2pvsibzhk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2wsvimnff.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xjxswdny.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qlurtumi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jygmrgcq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tittvsrf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2isjgzowv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2iulowghi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2gdehykui.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2lzpxxqri.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lkekjypr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hmpyldcn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aptctenq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jyudohvx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2wfrhwndy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2aejrjjuz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2jgucctae.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2rsmjuuvo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2caxpfqkq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lckeflua.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ljwiobsb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jmaxvaap.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2anoddsoo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2kxwnjbla.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vtiiduvw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2allgaexc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2apyrtviw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gwpnjwjt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2llulfdck.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dtvkylel.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2psgwzcqi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qmzaxvnf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2teuhbmxt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qxbuwpve.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2nyrmbkya.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tykfjgbk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hhnansxv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2chohitga.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2skkhvivx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gumtyucy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xczwmluv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2whzthell.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yjtaxwvj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kehohmzr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2fqfiehck.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2yvmlqsuf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2lldbtplz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sgilehan.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gcpngpzi.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fptsrxek.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2edogrprs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lnorpbvn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lngplfye.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fzsbvbcw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jxirgyez.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2wqfujmdr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ehkzlhls.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gyczdzbx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gihhzpje.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2yvvybeom.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wxxzkvod.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gdhiwaiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldzdqzic.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2fvjwmrgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdkrqplz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2evsenrfj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gpqhxavc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdwjwksm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ykqeugbn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gckfxaiy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2coqpoyga.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2dnmhnfag.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2lhzvcuqc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ixpeiins.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hwdclcgn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mfkkacjp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2fpyhzydk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aruxhuuu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mmsnbnls.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2zevjzkce.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2etykctvq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2atguhlzl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zhxgirtb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2omjhifzi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bxqjcoes.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2byxfhczw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzhturrk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwkzpadu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrrmgwds.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2wulluztl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jbvqtwki.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jstwobta.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rggxpesk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2jydhhuzq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ruyptniu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nzzvrajn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aeonqmtm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2hzgmrhaq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2sqhomzub.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vamnsmmb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pyagzpbf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2aqqqkblz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ypklekqd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2hzmaxnav.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2phbwhtwi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tkgvpsxx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2waorowgm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2islvbjpa.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2azjipdho.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2gebebggn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ignnlgot.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2folanrzg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2mcfutvop.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xtlfpurb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2srjecsjy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2patypgla.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zjwqaqlk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2qdlnxqvy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tppwtniu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bexsvnkg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2eestaoll.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pvktxpxo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jdrhcvce.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2hamuukou.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nrydayxm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vpuiysxt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ytqdmqhu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2sdmqcggb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ygdfrntq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2cvxqsyxx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ncxhdkuj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyjkftio.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eigoymtf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2rmbuimpl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ekormwdw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gvygsdxf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwmkrjha.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ocxsoxwy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cljcoepv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2eyrlqlqd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rngzkave.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fzjodukg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2czvsccdl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2rkfgdwry.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zaykhqgl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hbzfyanp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fncnvcko.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2dffvpvfp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2qpzjrkoz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cbjsktwv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kmcbvvsi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jiglpkoy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ptnqnspz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2xsjmvted.html


<!-- 参考信息 -->