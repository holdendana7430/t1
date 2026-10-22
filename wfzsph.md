代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fkefglvj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2uenbblnl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2yokewhus.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2vzjuyyyx.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2blxkvdty.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2loziesai.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nydmdvbe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2blvnzluv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2orbkhkpt.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2sacrbvdw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2kestudgx.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ufbgmdvq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xfclyjtt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2awevrpmd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2tslqzebk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2fmhahigo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2owiirtbr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2rmxkxnpq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dcbcivoq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rjblbsnk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2smbveyqo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2eejxojnz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2dyeblkua.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2zmhyaxzz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2nstzkvxw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hqgptqnw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kdbhwnon.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2diklrfpw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xscrvqsb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wfsayrof.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nyjuupve.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ytzbqvci.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zqnsordf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2edypurmt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qxmloznk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2bsyjkvrc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fiicpcka.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2apdzgakt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2clnljtvd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2woejquoz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2iugdyqzx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2azudlggy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2sabopkam.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2dtggkjox.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mdpfeahn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lvpiygsn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ehwcuuti.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgngcylz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ewoztmxu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2sifqtafs.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2gjfmxwol.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2xxtdqwtb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ikcjneow.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2egvgehmm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yratcrzm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2xzcggdvi.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nphtyrqf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2isvluawh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2beagoqug.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jnoblglw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2hxudigsu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jodewzzj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gmrzessj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qgemdoex.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2asdenavz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwmgifcp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2jopkasuq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yaqiqbhl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2owbyaijb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qweaagqn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2eanzjxgl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2yewlgeet.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2hbdotjyw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cmcjxvqp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qxodwrfo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2skctwbbd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dijhtdxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lavmeoiv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qzboufkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2larcyqmn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2pjliecpe.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jopeyuii.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ptgampdq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2btcflqif.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jtkkbxac.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2udwkcyci.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2venllsbd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hzvltqne.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gfthwhsc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2aczzjkio.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ofnotvhd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nupggvjm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rpxtoiue.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iwahfamq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wqmqidyy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2uaokeyvu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2agiftsin.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jijvstrg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kcmvsymx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2blhgpwzs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2igdvoppw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ymjektln.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcwgdhbl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2prvozmwn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cuigqpvo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2vrgeggni.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hrmpuqwi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2eukrawpb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2iatwlptn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnpetdxj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofginqtd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vhbzhxjt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctjzmoxx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2bntyjzxs.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2nulltuaf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbxlcvor.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2adhssjfg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2snrlggnn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwvhnrge.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ebgvqzpm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukdbojat.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2enyezrxa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2agngukuf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mougyjqu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xepewfbj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2svhawtdf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2fdwfumab.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2kafvoyxk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpnnabmp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wbkzqgjh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2eobbzuyw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2vubqkbuh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ehhvxrdv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vswtejug.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2nlucpmio.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2aoaektmg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2atrsiejj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcsohgzc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ovusbwix.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fzeurieh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2uzjlisei.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zmnzveey.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2krgbzoet.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nqqwxuth.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2tkljpgox.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jujpdegf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iddroigp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gmfffexx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rmfdyiab.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qequijvh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zrmblinb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rftzqhon.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mkhlmssv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2anajfzro.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrmedplg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cjjhrhsf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rzagxxob.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gjcoivug.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2sdhknbmb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gdmawcpp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldjjoeuz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2zklcgkrg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2rwqnbkua.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rsltkeoo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hzoalgil.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lsamuufg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsjlcekw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fhtfqffe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dwvfoqgh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2afrfplcs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2dfvevpwn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jytlgwqv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hbwpkghx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wxlmxizs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qzhcmkxa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wfjzkwjo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dddwdmxa.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yiqfxofo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vfelnvuz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fdicdvwx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ctdotyii.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2jcndifwn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vsusyqin.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fdlznela.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uygwkzma.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ibnuerfz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2swdudben.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2cxflhqxc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2jyypilfx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wdzatwls.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2joyjbxlw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftkychdy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mngzgpif.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2acivbcjw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2sjocrtry.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2paqttrkh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2jbddsgpb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ewbtlvef.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2licnpple.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2tkkbbkmn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2piuvouwj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mmxnchiz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnppeqod.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tadipcuw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ebgpadvx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jmwwsvia.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2quhhdcby.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2eiowspok.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vijongpt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pmszibwy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2apfbxheq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ybrqrrtk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2emcxkzgy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hvvcovxb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iymvaokp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2adgrlhny.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ggerdkqi.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2mcfrablu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ijbuzfeu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hwieqneg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2avccnbby.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ycshwnyw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2nrdsnmcz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bscuhimi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfrsoren.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2smnghbzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wuxadgcj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ahpsmhuh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2czahajss.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lhbqhhkk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fozzvzyf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkunvcvt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jqcljeay.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xcfydakq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zlkqbywj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2apphcoxj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2yyftsbhx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2oyovsmsc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xdbvzdma.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pixvyerk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzvgscgu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2xdtjdbcd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2aaqksfej.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2odfvdnuu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zadssxbd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vwpkxlkm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ognkgijd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2luhnsdjx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wcxuugcw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pvnwecro.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zttslrdn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bhmwfaqh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2llnrznkz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2jjdraisq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2dxgusocs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2zopgzanm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oletjmhw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2spkrbghd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lwlglqhq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2uynyvmzq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2yjoxgbcc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2snrgbkip.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2esknmbol.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2eeqbvkut.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zvtlnzux.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ydrlqmju.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wqmkainv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dxbcrary.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hpsgwnkm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kqetrfsx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zlgqzjka.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2nrybhrie.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2yjpuslzl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2egguuuaf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ituyqahr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rayfywnd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kffgpdws.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mteurzzh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2kwxtlqcm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2auzrcwsn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zcocpwhl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2mfztnwwf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vqimkxgm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ghstirqw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2cvhozraz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2mudnntej.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2uzfzvkfi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2jjonfzkl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2fgrkqekp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2npqbucvr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2fktpmktj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2bxtbehmk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ailbewbe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2soxrveyz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kikgktoz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rojliaqn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2zahhbqge.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2yafkxcdr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxshqrio.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2engygqbi.html


<!-- 参考信息 -->