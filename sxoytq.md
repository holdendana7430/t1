代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tdkyyzhf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2piewcdkm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2wrlasqzi.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2xkeuikkf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2kpuaqrng.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2tirvnlmo.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2sklnzipu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ckiosbgd.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2gmywqmuh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ljkehpes.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2voqybsjf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2txbqvlnz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vsawbldu.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2vegayacs.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2wwbnbpfe.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2gqsrzdlb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2wkpkwzlq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2zhalondc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2bmhpklxh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rgowobzh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2kimpkutd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2piifbujd.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2cgtiphcx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2dclsvdib.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2atqjcsgc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mkkoifwe.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wssdvrjm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gzqaqlpv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gahajngi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kkrwsxlx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ecsektqt.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2yglpinmp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gckgxsav.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iedybypq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2lgojpbgt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2dcqfngdu.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xdowwzwf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jxmdspjn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2zvechvrm.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2whmugwka.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2jdxvdwes.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2seipdtse.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2dmxirbnu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2rremlimp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xisybbjz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2earpdxkh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uplqqqdp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hlrxlxrf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jurvelgy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wdvwuhye.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2vbexohsu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2vovwzvvu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ohposjld.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2iyocfnkz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2czkzmbvl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2hqkzjvly.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvdaxnww.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2gymiunlc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hoeqmvgb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bvajqjfm.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xknurukn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rzvggafc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2sskmcmgf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lwfcayow.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pecdxdrl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pkuevndj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2imworwku.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqdqxwrs.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ggcwwunt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2sououaov.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2xnnofspc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2xruvubdl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2oyuywamg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kylrneog.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2lfjnrecw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2yviwssai.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jtqpapbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hoexyrnf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ucbjsyre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfdwxzgn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lzfftesw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lirzhplu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzysueyv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kqxnedpt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ztdjqejn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fuuhjkeo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2hocwzlsm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pxzfmcuq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2agkxbljh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2dmtwzlwn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xfxjlggt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2cgmogala.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zfmjvskq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qelmpxlk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ntjjdwbq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xkeshlgz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2gyfnthwi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zamrhvbj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2vipweysd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cehaetwc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nsobshpw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jjqmlofp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2czjrstld.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ajveygri.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2uajvwtuv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2trbnbuik.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hxsjqjgj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kxxbwxfl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hquuffxk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jgbtxxyo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwdpmsgp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkbdyita.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2wareltsj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2vnasdqjw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2xnhfwltk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fybbsmnl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2iaksnobq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2euveafzr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vjyxpocb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2aocvhpxo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkfjnqvq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2txcgkvaf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ftklspfv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bayfdhqu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejmmunwn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2jwffbaea.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ikfpnsab.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jclysiuv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjggrvco.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfixhpel.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2rgagbngw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2yuiqpuoi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xnduxiia.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ecputdyf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2akiqsybm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ctrafpcy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ztejofam.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pikgcggr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpchmpvt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhcgielx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ykfoyrpf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lhabcgcb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vleghxyn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2cnfgmuki.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2budaqmfw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uzjaciti.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jcqbnuud.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mvtgphnj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lroubanm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2eeljqnfg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vkpnormw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gpswtyln.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2nwqbatwy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2yvmwjvae.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tiuwvohx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fkppitoe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrizzmms.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2anhdbzko.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nwtbijsy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2wdxixflw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eifjovho.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2uzlqqyvn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2bwhtxqrc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbclyaqn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mxkqsgvq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2owlzcpks.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztbcrkuy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vniosjuf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yjxgidah.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtsbttpm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2qrvryubc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ihvgmbch.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2dcdvmxih.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tijxpjbd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bljfbguw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uawbqmqs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gshuzqgk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hbvtdlyx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hqyoxahx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eyxbephi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dmuiirnh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zbimpvlq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2akstfzio.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xxzdebjb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nghlfzec.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2bulztkfu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2klwvkqrg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hxdblioi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2rsrqxafc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gvpncjnq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2izpbbrni.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tcigovli.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yphhjnxl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2iwbucuyf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lrekpyfn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2asqkgqrc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2kjpzykxr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2kfmtswgm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2skonpfit.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rrhorkmu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ictqdiyj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnijwqtm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wcckxbgr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2komomwkd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vatsxhht.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2muwkidzu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ysikyxqj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2vxannswq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fdnpihjx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xevycwlv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qlanjhio.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2effarmzq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tevxhscn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cozzhrbd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rtwtuety.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fabeamdy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2bahxuazf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2buyhsxto.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uzijwmdd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vxgynlrt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zwnozbgm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rzvsfkpj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2hlbfxdxl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ovnweuhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oydxmljb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ebxmvsmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgqswfeb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mgvicomo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ybcytxmo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2faxtjjto.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vggclzqz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsdphyrm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwujbjbl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nyxcyxho.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2joppcsyd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2itvisyfa.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yfrrbzin.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2eihaarpg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2anxnzxkg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mqppjwoo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iulfkcxi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qczvgngc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2aecwxmkx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jdcwahun.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jbacdswx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2qemuthmp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vsnwflgi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwxwhnlw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gxgarewi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mymfwulb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mtsgvsvr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2xifzdijk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2beihdzxz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2vquydowt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2orzvhmtp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2afjiesxm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qgprgbpo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tnvntrtn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wczuklio.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zecodwjf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2cylpiaum.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2alenbypn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ptvvtlsk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dhfimjvy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2stjrkiav.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2firrgbnc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fixoblzj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ndaxfdmr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hvmyksxf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ofjtdzto.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2eryxyuxj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qnozcajr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2dseianok.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dyjcjvln.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2fmzhxliq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kcrpnvbh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bnsxzvvu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2owzskbuk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2yxhuinsd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wwdbmbfv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2omctnlcf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2wjbgejfq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2pnoqjvuc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ntujxsbw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2scsbgkmn.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wzcqxfnl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2cmezkoys.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2yoecrxcr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rgjktian.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2yviuucwn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ramwccmk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2kekrxwti.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2joskvliv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bxowmnpy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2niioqshp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2onstxlox.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2fqmjearf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ursvrocj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksbutiqb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2rntnphau.html


<!-- 参考信息 -->