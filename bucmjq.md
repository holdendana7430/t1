代发 wailian999

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cdzzbseb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2dqlmjcsp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2inxmubuq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ibjewits.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2yytgjtsc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2baxyucfz.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2bkhpusqr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2xunfzifu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2flxzqyot.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2nrqkffph.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2sauxqqwl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2lueuiryl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2gqbkyhmk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hasdxuln.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bwvtngfa.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wnvqzwgw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2isgaerqw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2htqlhmwf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uqzhhuog.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2jmiihpnm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gmushajm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ieykbymv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2bcnfucjh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2jbhjslcx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2byrwpwam.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2tqwdlsqd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2yusdcocd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2isgmsmka.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2nvjedbhp.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kvwxmcsy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2uskhpime.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2biovglis.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rcdklgqy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tbuuinxo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zeuibnyu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iygiwvfe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ghmdaurv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ysjjdxcg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dsrtsdjz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2gjezewwc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2wofbzskz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fwqtlnwo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hhgwlrse.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2nbehewij.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2rymynbcv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2cjeplzny.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dbqazfmm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wpammdfu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2hvbdznkd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mrvudcfm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zcefqfyj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qzubutrg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2uevvlwen.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2stcmvjru.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2cclcdkwh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ptundyhf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2exbjozqd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2gvymmejk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2zvdvpvsp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ixntosxf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2lxlbrnco.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jctbbeis.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2sbwjcavv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qvstpwdc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2unfklkgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhwkgxuc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2aqyceqel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmleijrd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ewzonbmv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2bnlgsgza.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ioaifhbu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wsalhsun.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ogeezwak.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ojaygfiz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ymiujywn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2glmfcdco.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jbkeypuo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2daqopxbi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2phjvfmhe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bdenqwbu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qblanhif.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2myvwcyjg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2khpisodd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2dxozrlea.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2tbuavblp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pzqonfke.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ubimqgaj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2rxckxpoy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2akehxgfs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsidpfek.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2imzmczek.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aanxdaek.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xfafvxdm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ppmlqsgb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zmxinagl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kczqmzfl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2makwyyvx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrfrhgjx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pkjoznnt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2itdmdobm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ovzndzzc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2oguimnhl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2gctxgvgi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2gzvdxijq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hdmskmvo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2tuhehpdi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dtkuvzvp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikworpyn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gfwbhpzz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2dpgiqgoz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zbewxpqn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rzjbxqve.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qmbytrbu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2tohivbeb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2vanlkzgt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2udjgghmt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xooxjzcw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmozjmtb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2wibqldwo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2bqyvpbvm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2fmneqlic.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tymzxahz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hwlgmrrh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xpojmjgx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2gjdgkzrl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hliqnsjq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2scihgbta.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvhibbqc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vjtetrpy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2grpgsqnj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2decieftl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2fkvkdiqt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2owudszrh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gqeqkcys.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2roggdive.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2unbipsud.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qgmuqnva.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tqrrgopy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vdkcukku.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2msgumdnd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2frmyqomb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ijvbeqgg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrzxbvge.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2owqfuvds.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oicdcmlk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2awomudlu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zniycttu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2svnzgeqd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hnthjkul.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2gnjrclwp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qisaukcb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2wrmptlfr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ermttzge.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xmqljjxh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2lgzxcrcc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2eimtqcvx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pvdluutf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ciopmkpt.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ubrkvwbb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ftzonfos.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2cikwcnjc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2paxbkqmm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hkitzwwr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjazkjmf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2madyjlmb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2adigwvij.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2wluntkqc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lzuvxtsk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2wgfmmtnv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2fcihupmb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tjvqpxij.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xqalacjp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dfpuozna.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2eqhizwqe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xggntein.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ausnckvp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2opehvbac.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xkanycaf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mekbcnxh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jaddbzwz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jrxslfmg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2teqezhpd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fqzyoiqp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2uameuvyt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hjmvnuxj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2nlftnxww.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tifykkek.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2wqfppydi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2krgetxpu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2psxmqoiz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2spfxcjbj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvuuwjga.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wvvtpyyv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wqbyxlic.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zxzeycfb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hbecidfq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zqubnuma.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iqitithp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2forlhrgq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2afztqwns.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ekflivwr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zizzvwli.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qslzbzbu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2itwyyoal.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2cabgufjg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiefjycy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jhfzmdmx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nrxgqylx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2sdnmijdg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ankhrlpd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2gjkchmlu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ebwaxkxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pikzudkv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2milgfcrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuzttiun.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hdepgltw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2cxgydhli.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2itsobeeu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mwlfmoyv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2otdhzeii.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbelqgaw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wwlggviu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vpwrlhze.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyqzuprr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rxnupgsr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2kdzqglwk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oudsqipf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jqdegjcz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfmfjqwq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2mqzobrze.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2eyzpdvnw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hpqketis.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mjbhbxas.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ushdvqtl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2kykgjfbn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2skpbxppl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2aldoarng.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrryodcu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2shykehqh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2mywjnnnn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2aukgvdts.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2yqvbpate.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ephiopvr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2omuhwuvd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2xoewkwio.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nwkjaovz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2sbnvjhmn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2hiptpgjl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2glvmpzxt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wmugzzde.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyrejmuc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vmdwqrsa.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zkrdkomf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kpjungvn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2chxxswja.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fuasqtka.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2pblmuwue.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xkpnqngm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2gkoxniec.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2obpmtrio.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2nrhjiyjt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2klvcfvry.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2tcetjtoy.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ujdwtaes.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dbopaivz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2cxhoffct.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2zlhfflhu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ncvhjatq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vpbsgbzz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ogcpymsc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2pbulyqww.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2faqvmcdg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2cggrkyez.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yocqfigj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mwdsntwy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2gbmjudim.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2mndpplgj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ockctlid.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yjtirvfx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2unjwozop.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2elyhxflr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2igrlsrab.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrfwpkgy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2xnxbqgfs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2mhzyocqq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hdhhkrxo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jsbyqwnj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2cbymkirt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibhlirgn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bnfnlzof.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ozmigfek.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wzyyvggy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajsxjcqk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ufkbamuq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxsgmoeb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2idsczyyf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2onlijcuz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2mupxybqc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2wrvekwfk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uwkgaiag.html


<!-- 参考信息 -->