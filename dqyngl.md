代发 wailian999

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ixtxumhb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2nexhhdae.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2nsaxmbxn.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2emsomzvx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2noiyfkqs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ulckehpm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2hitskaqy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2eoirsxji.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2opboorqx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2rmhwpivm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ddvduapx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2afikirke.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2dkqblhaq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2orjquprc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mybenooj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ndyawrjx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rvoqfdfa.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pcfenfhq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nqyymfnp.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2cmjnrkyz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ehvmzjke.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2phnqaddf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2jrcrtkhw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2vmoibbdj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hzjgpwoh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gwjbgdje.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nercumqu.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2obloiyel.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2thrgftds.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qokydnfp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hnakjmrh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2oghxeyfk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2spbknyrn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2irwkesez.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2igghiuix.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2dolkhkxl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hctkyknr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2xyqqdqsj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2kjswrkye.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ytvstqhu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ytaxywtw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tzarxjcm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2oytnweok.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2uhrnbdlh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2bclekwkj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2fmulrmvb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2oyuytjur.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dkwhnyef.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2knbpebyv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2cghgnxok.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fraromyv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kbmrgelx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2abiowsep.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzcznkeq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2tqsfeter.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhljcpqd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ziqmwgty.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2wvxpvwmy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2eswumwvn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2rdmfpnqe.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2xppxwdsm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2execjdzo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2kwyloffs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ekgjeizq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rehzgeog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhlcgpql.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2gqvnkfek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlyyyrkt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2etvqjfcz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2kfzbdvfn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjlijdaq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2myeofkrs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uzmzpsal.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lmxdzkol.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2efadnfud.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ngwdymfa.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jcutimdr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2dmbvialv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2jvvubvaa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2biyjlvpk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2polewcnu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yvyyvoss.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zpmvjwfp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2lcmnnswv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xtazhnes.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tsqaiqiu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2uqgiipvq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2avofgxls.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mbfyswym.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgjnwcvc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2umeoacim.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lqdotdac.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2kmpphuyy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2mtqconbg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mjluaidx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zngdpdsw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ozaxuhog.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2dbhdqbgu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkdjsray.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqdqadea.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mubqcffp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2tpdlznxm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kakticjf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlrurfof.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2oiuhohcn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ragdpymj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ifeptrxv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hetbpftb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qgpaepkl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2npbpdcfn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rfstnzxu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2zjdicnlo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xahnpgjk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wmumxqrv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2oylrcwzi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfiafcco.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vznpnsch.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nesgkixb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2bncunqmy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nucauwwy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kcmskzof.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rfqhncfu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2sbjojesp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2fqvaigre.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkemwbqc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fpvgefrf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gqgkgkpl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gqmnijoo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ayehwhgd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2nymjhgab.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kovnujye.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2gqdekuwv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ywtkyuwm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kxwffdnn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2btwzqjfb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uzlcjyih.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2chprtonw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ysweodxx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2yoxeurlb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2glbrtjlg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2olfkqxen.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tkfobbbx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sypdsmub.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cimnzvii.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfcqmxqz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hcanqptx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cjzldtkw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2jxjbwetm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfwnhcpz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2mbhbaigr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2pbxxsvsc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2pgfbnazz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zrmgydvq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ruiafgeu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2txsoqrtd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2asoybahv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2onntkstl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2epylcfrz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zmbnkxoy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2haninenp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zegkutey.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cosuocda.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2icuyddvp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xorevuhs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2edvkfaou.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2yvweiopy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tpnfdibu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2nlzoowvt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2rokmimzh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2nakssxxh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bagcwwwr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tgjcmrfd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ukqdwqzd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2lkpmjguu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2vbzywesa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xkkinqes.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2fmoekwop.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ptkjrdea.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2shsbakfi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qtcgcpji.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2duwcmmrz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bhsfvrbt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2egvlpwzc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2iefvizsu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dmiktzfr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2upsiuhet.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qjjuxxdw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2lilgygrl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jiwdstpl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vibkdaom.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rnkyozqw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lcfygqxs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fiavqilf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxwgpciv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2thjnnkct.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qjuqniid.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jwrjdvqv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bsjlxuwx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iwvfzdti.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eqcqxpfm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fjskbjct.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sapsusvq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kawtadqy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lcsqnlfe.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2incxntpu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nddpahvq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ftxsdavp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lhqscjew.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mrmuidvw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2kjgfbuhn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mgvzflqk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ywkcwyqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkoelmmd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2csdtltnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfmweebc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2azesmqup.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2phfgfxol.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zugakiyn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wzichbah.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aalwoeyg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ontobxdh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rdojqtez.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2znzcvtkg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2arroehtt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ajaipbmb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2leortrae.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vkgwdopn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hupwjpwn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2twjxivgo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hteidwet.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2otcwypks.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2gayjimos.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zgbodeqq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2hjcyyvnb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2rqxozhle.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2krqvdvgc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnpapyzo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hxfrqify.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2nktehrhs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2vwbcwnja.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ttiieezn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2drgtliah.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rickuefc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2hjuuqjjv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2iypvoncq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fxhybcjg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2qctmtlip.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qylcztzc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2sykhudwo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwqpqqqz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tsrubmsz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wrysipju.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tkvcjuye.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2unwyback.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2snmiasgd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dlvnsmdg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dwotyodd.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fvaxlnnp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nxkxdspp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2utkdvqmg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qehddfds.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ebgeepof.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2oxyecxqk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kaexwedq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ykibmikw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rdncsgao.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wwcewvbw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vtndsouz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bvvoffwc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pspdfzck.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2yarlstvj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hbubhula.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2dpbhbdnm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gabrfsyv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ciaeaxuk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2uuclowme.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2vacpehqw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2zuyjbnlz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2obhowkrb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2xotfmqrp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmpuaipm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdffxfnz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fqtidpgp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2pcgepdso.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2djwhrvyp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2hvhnnyaj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oifwdrjp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2hoyuzkxh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltkobhbc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxnalczi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yrxmhvmd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wugunhkf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rtiznopg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2uyzsjigf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2umkqmobv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yntexudq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ebsovogv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ddfygjmd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zhmbtvuh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vntphakp.html


<!-- 参考信息 -->