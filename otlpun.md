代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2diedxbih.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2rvxslnij.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2tztddsnv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2afmqlrcw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xrwjlwgk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2rqhbpjjo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2itkqmmyj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2vzhbhunz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2oirrgxnj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2npyxnthl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tjgfaylz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zmhdndrm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wnlbytai.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jzzmmdzb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jlijxzkr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2gzwkphcd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2aiprmfnp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wetgbsyr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2seqndvdo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2bzccbofx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2adzxzrhe.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2akkdbewh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bphelaxn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tkeixjbm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2nfdrccab.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2stzwxbzj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2eopqmert.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjxdgqgq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2capyxlwx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mibssoqt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jmphrnza.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2yzxxzrns.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ubhvywxq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2guguqdsm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jwuvepcm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2vrtygsnv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qvoxbath.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ddytmdfj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vsamocus.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2assognue.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvlzrtou.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2brlcooat.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2sbbdqnuv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fbhyeazq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2hwklvylj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmpnlpfe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ixdwvudz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yvvtiiyc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2yjeppjfb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2obijzynx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2fkhsfiif.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tevziynd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2cqhprzgi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2zmbgujvs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2sxxzeyqu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2gxjixhbh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ycxxvigd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2eehmbypo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2tewduizh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zcsbzbfk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2drbtigte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsvwdjfd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2gafkahus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avkgfboc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2wiyttllw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qxcdhopg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjitjglq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ojjanqej.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ymiwfmmq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xuhzlcrp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2mepwvqao.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2cpzzowsg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mdtlhgjg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vejtsjgd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2jokkhhra.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrnqqbfn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gixuimyl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fnglixgp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ekeyvpou.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jcatctku.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2qdsqsqkq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dcvskrfq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2esojafny.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2bhxaogur.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bypsxzvu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nepihgqi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pnuavaty.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbrsdekf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xrwvnwjh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2myhakhdu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2corqhuos.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zgsbwcmq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2lagofgja.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ahlrdzjz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fysmputv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnekhrda.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2qymaxwmp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2fmvujenb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2tobzxlfn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2erthhngo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2eheqnxmg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ctvlngyl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydnrjvlq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vhijqyqt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zysubqee.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqvngbhz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zmtqgtip.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2hginwvad.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzjieffu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qazrtjkz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jacdlspm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xspshzpc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2taaxzlob.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qszvgvwy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qioglhlu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hfhkkwxg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yxquzdox.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ytfnkfgn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xwgzwasn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nprghlmb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2seigonhw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgqhzlcg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fusxkhqt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2egluevjw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2apqiwfhw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2crfcogjk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxkfrdod.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2vachhsmu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2taiwskwa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2itanfgvz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mjcddcuo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hfwliqbu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sxmczgef.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kykwqzwe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2uwdznwkv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ymnnetbs.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2rjyagxju.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2akaqcuej.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2piblvhmu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnmrpwmh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2meprqfgy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hqldpebd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rxvdtequ.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2bltrahtn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejqgcenj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2vhpxvpqm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ttenmtjy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qohykrdq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dhxanrni.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2uganrhba.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ybeizghv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2huoygadl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fsavviql.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2uhfzlmhc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2hcdhbgnb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zpgujgxl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qfkwevuj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jbukigop.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qmyooacg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cqyfeqlp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2seiujxwf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2feucoemf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ttgnstbp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vrbsfpnm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2oczkfhmn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mxrbmyim.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cbxipozj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gmfxvecm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ovfnsrcz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2yhkssdqg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ecpogcaa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2yrzegrcs.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2rtccidfz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qzbpzfgs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnsuevbm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mvzkdvtm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2begpgntr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2pmigsrrw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2mxfocttq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2uypgvwrw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2olekuaza.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fmqteybc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2shozpmjl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rmrwfsqg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftjfwmvs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2icxibqda.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sylosvzi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wlgpkwrm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmikehnh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vtevgzhm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2cqrjebyp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2xzkhipzs.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2skgxqpdx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zrbddgdl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cncxwiny.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2balbnkyi.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dntbuhsp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lhjlxvhd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oggfmmam.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hmrihglu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jvprckle.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xzotqrcc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pbivejae.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nnftdifk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ohhrdpje.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2frbxzawu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nelljwff.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xlkrdamx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbnygnkh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uneyjxln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxoysmlk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikemuqqu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2nldtmsun.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmedrerg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmzrgdlp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjjcudoc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2inkodusc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jzhazijt.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2viormwox.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zsjnsvpx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2kozndcxu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bsgoyqfu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2tfrttakj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xlgidzuw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcqssxtw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kimmsjhi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2rnfxbkdg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xzvxrmkh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2vefoidfn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2chsiyzqk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cqjmglgb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2erovzrnb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kfndiagm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlnqjxvi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2frjiydio.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ehswjwvd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2afxhhekw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jtfkijun.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ymynnyjp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2urcruifo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2dowkvvep.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hveqcndo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xjoukhvw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xsrsxmvk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nnjnquka.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eqvufxob.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cxxiawmm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xuhqhhut.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bofeqyjj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2qxanmujz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fqrejpbs.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ptumhsyg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2oojridjs.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dnvgsrfi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2puvuuxcw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qbxbyjmh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mtxtsdmd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2phrmbdbm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2izcofkhp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yczzlujn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mxmloyho.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2bcnqqmun.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2moxvwzsg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wxacfvzr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pbqyofmf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2wzqwqftk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2tctngicf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2osgwserl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ngtzgveu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2fqrogfcx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lctpdxqu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ugkzblwq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2bfsrxvls.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2qkfyvwme.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kzhtenua.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2sjwzshas.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wpthzopx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ubjiebxv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ntixvnma.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2lxqoxcts.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2sqbhxctq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2efdxofzr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ikgdhhhq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xsotlrbu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xcdzlrbl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccxpsrex.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pfwkfzwr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dkjcovud.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzwwhpzt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2tuefxpdu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2iaqutjaq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hgyfnokg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2wdregnxt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2hhzjexdz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2kdjvqtqy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2trsrabai.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2duprngyk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2icwcovhq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nnlpggxa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2sdncrvnk.html


<!-- 参考信息 -->