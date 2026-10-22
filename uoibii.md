代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2amtxdtjf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2synnvpxn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2eewdrppt.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vytedngy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fzaifvsv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2sgicdmjs.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ncezewul.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2wziznbkg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2yqckcnqe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2mjburnkq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2bppwlldz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2opaviwtl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ihhstxfa.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2utnnqmvf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2yaktlbyw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2sljomrhg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2rccoatja.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2spcrwfsa.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xcyrsati.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nutbowej.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2brrgjtdj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qvalfjbs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2eqadzciu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2vpkkoqby.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uhunvvfp.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gpzlfnil.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2mpiravni.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2bmssslyx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mrdevgkv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ostovyoy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2glihlhrf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2suwnujhd.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jnhmmqrf.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hsvkchyn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2uvdcbimg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2uzrbilbz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2arfginzc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uzcuawkz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2oanscitv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2rattetjl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vlidgsyb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ezslcbsy.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2utwtsibj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2yqfqivsj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2atapfwwd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dwnlendd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vagmswzv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ohvttmhx.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ixnjopwc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2jpnnowxp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rhvtvzmr.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lzsxtoba.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2iqbrzesp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlxdcgcx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ucudevjg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rsidrpdl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2pborruci.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bywfnhrz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2xtxwgatc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wbbwsecu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2svpgqpei.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2iyecuoic.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ofxpwdil.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2bmzyhdwt.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2taypdayp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ymgnmjdx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2pqrrxtvf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mwnxqbkr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2taezonnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eveegwgq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2sblqnuou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxkhabkc.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2tusvlarf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2sbnjaark.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aofnlxxp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ocoqksty.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yctdaefp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rdhtegvi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2negyookc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2lbyifgfb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2usqzqiiu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2yipvcopr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2qjzzfegh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xggiqtri.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pkvkovoi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2msjgpzde.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2capocpfo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2opsfkvnr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2edwsnner.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kwdutcig.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2frcyttls.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cubvjymu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jeecqrpp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdeqnlyl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ixvktyab.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wapdndnr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2atjgevyd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2bplkjobf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2overltji.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kqwmrugd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2blzvuuak.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ebrqzwgi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwlusesw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xpxquxqw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2peyajvap.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2rsfgalle.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2upgwdnvg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqrsptqr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2aypxijwt.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xwiisdbn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2nivjaiqq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rcuedisn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ntwdvipa.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zaaradqr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2abwoovhj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wrmbfbix.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsyudrko.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2idxkpyta.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2rusoqhhf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ytfuoftq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ieyjoyvc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vdggmrht.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrxxiscv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2egezfgip.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rtdiwmyu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2sttgxlgd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rxtrjlct.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hexmqkdm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2isbfakcq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gyiphnlz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2teoviaup.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rjgmfigl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2qpjhskvz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dnatmljv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sqwnbqht.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2myilqckj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2weqwgtei.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sholrfqh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fgixxfoj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jqjvjsfq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2awtzbctq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cpghdzcj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2krfkdool.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sczrbjnv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2dqopvwlx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2snxbibdn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnaanalc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjrvqhtb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtufjlit.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rupvsixb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rhuccszf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2wefgvfes.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqfybixu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2bbocvcal.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wslkjfrj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlmiokct.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bqlznjau.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gbehoxfm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxqmigau.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2hfcgaiob.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cjhxcvkt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ebgfjliy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2frhkulmo.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vcctqblu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2isxetkkq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2weyykhlc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2riakslxk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gijuttne.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2uvmpyepn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2xxcpqydr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2koagiinf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vtujfwea.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ytotroeb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ramacmah.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aapsccwe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xmrdokli.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2edyrfdti.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2daezgvhl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2zmodpeoz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2iwwjskwq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2cbudxtfk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zgnbeemq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2iqdrtddn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2agaffpjm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ewnucvvg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2npqlabsu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2oxkqipoi.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2crwjydtf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2iqmsftmp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lglncapw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2aqocafow.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2tcnqfgcj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rgfxdcbz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jptjhbfk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tcglszug.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2obomxxju.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pvvqtnoz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pyajdblv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2henxbdpf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cemmmakv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fixunojg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jnlryfuj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bvvchivr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ziolfdtj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zbyrwiih.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rkxymhrh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2szdfxwxe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gizctngk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xaqrarkj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xboulpov.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yybartxc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oqcngnlh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oehgmljo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bldamvmg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vxxwylks.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nlkbyqbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ouvwdplo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oxqlnkay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aksvavjh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2iubtxtle.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2eeogfrbz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnqhvyfc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpdodykv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmrrhbga.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pbszriwu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zrbksuua.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2byvhjysa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sisioabl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2dtldzemv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2tukdmrxi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2saihqqdc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mttcfgtf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2drfypeyx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2dalutogk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2iznckyix.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2rvkulcep.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2hdfimiwn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ecncdvgo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2kipqwyld.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2glwrrezp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2emwygmsj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ozbbhfqv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ncrrzpmo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qidhoavn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2kepxpyws.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2goauoikn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2vasjjmvp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rhkqigew.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ypysqfqp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2inzkaeue.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2abvsnojo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ptkzbrss.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2lstgkgox.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zdeztpqd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2flrpouxc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ycpwgndc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dothsupr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2yikfxojl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2slrguhpb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iugkxqou.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2sseqqmuz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2oycsxiha.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vxmygeov.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2injffdgm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2frqidjnx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2bukbdkdh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2xvbodkat.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cvitxbpa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uynluxhk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2fodvlzwj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pfhdrtqq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wpwcvatg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2urzzorvh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2avnzqrmd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rdrbxlca.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bpmfxptw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ejuchigr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qaeovxop.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2biqxjyfy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2unmgonll.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kqzxfvqe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ycpgjzru.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kcelmipt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2rzppwixo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipvhxaqh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ouequnoz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2slbfkjpc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ofvdjxwi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2dvlkvfhy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2eslvxmos.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2egjggnrz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2dkhbypak.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2taaorozq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2doogdwhn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2azsbyfip.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lgkqtutm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilqaqmsu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2rtxoiqlt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tqyydzpt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2tnqegjza.html


<!-- 参考信息 -->