代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2rrnucjpu.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bchnihba.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2qgmlbnxi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zkvspfci.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yqmmaqfd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2rxcgmvwl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2mllnosnq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rlkqxbhf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2axitdpro.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2iomwvwbc.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bbolvyvn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2kxsrjswo.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ktbiuffk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2yqucevje.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2zcgeepyv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qhuoehcn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jdwxcqdj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ahdhpmmx.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2cthwvwlv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2cxtylyal.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ipegvhgu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2maqbavqr.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mwjmdguj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2xizcsdmn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2gavkvcwt.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2rixcmqfg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2rlwtmbua.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2cewtemch.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2lyrgnbqg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lkzzvxjk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nriendgj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kskshlep.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pxqdzvoq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lgzkmyiw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hnnfufsj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ckxeotvs.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lwrsgdyy.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2hwptnmyw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2vxogmdps.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2dplnubgr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bgklrsls.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2bvvjesup.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bsadnzpa.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2kbcyeqbj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2rjdqdrib.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hpfgrnxc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2uvlvkeyj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qwmldsje.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vqsgqrmr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vajkjbkm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ncxyqhqy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ugcebcag.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gszgaodc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2jlyuuife.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dnovrgcr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2vohbslih.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cqgvuvzw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2sccdzlty.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ykehhefn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kloqdkyb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2horfutfc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2kmvdhncj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mabitpem.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pdgdxswb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2tyonzqbn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2rpmwavpr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2txpneqnh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ltmhopgs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wsnlsegg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2nyrbxzxl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ggzpmvdd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mfeitzwi.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2yrlblkxi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ckbtduzs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2nmnbjizy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2iwugngjq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2enmhncgn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lsohwpqp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ziqjemww.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kkxnlrjn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2snarnstg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wabjdloy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hiucbjcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbqulubf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2gtpjzrbf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rdzlkayr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ralyxswj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2utvzaymp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nkvgtmmm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tpkgtuna.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2xqskmcel.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2xcobpjnv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vsnvdjng.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2muagnohx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2fpxxnqiz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbghavlo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2azzwhuma.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rjqaajag.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tygbzvfk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zkftubla.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2lxxtfhja.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rzllicsc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2msjuubxd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2lhljlrnt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wzekiwbm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jwnowvcb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2usqnalev.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uknuzmhf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ztppxywz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2njteiopu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dhilltbr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2iaivgjpg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yeafpqgp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2pkhlfegm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxscdibm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sntwpjko.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mxfpwefj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2urpvqfup.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2hclkkwng.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lihosygt.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ltsjpejv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2cnlpclrn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2cionvfep.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wzugxnvz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxhuilqv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2flqojiyi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qnpwofzc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2fxhpxuwc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2umqfbtvd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2xxikojso.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2njpobptl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxafzkcw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qikcqvno.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zeyrrfyb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfzkezfp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yqisrnxo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2zulbyjyt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2sblnccmb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2qqlnsjql.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ynkacfhg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2cfzblchs.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ymtagsaa.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jejhexpw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qlmgtejf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2pztnhmlg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2nmbjeaby.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejgobejp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2wcsiuzpk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2mrgnolwh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nhmmiccw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sjpumaws.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bluafqtg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2spdgvmry.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2udibrwjt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2towvdnnb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dmsonchu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qtescolt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2zsothgye.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kzzwvhbb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztltsctj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kvwkqvgk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ghqnytio.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mjcvrvll.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2vfdhjern.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wdydvjqn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2samizvhp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2yyjpirzt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rdtgbnlq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2miuxflfo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cyzlwtec.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2dazkpmqn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vsqybbkw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2gkkpcjbe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wjnnrlds.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2izelsdqj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2gmdaanvr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ijnygyht.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ybfrmdif.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2msgmupgv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2liqmqijv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jmjszidm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2vaosjjmp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ygbbdqhy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qakayumt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2acaatchc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2yusxtzes.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mgbzbbos.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eknbuqxs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ijqiopaa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hwqnlwwu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2doyuudlj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wdyvrxdt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ozuvdgub.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2letpxowo.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2knzroess.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wkoaevhn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mngftyon.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xdwtokox.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2eesumkqa.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wqfkcikt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hisbdbnw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ctwkhsdg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2bwlpkgwo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rnqiecmx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2myrgsngf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oewpzwev.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2twqbbvro.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2icrcvjxe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mnxmfecr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mbrjytlw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zpksyuvl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hwfkfgsp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2yvgzdeto.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vzxzrmpo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2umuogsti.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zckuekpc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ejsavzmt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hjeuyyzg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bqcljfib.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qornhbls.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ifzzdqmo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ouecgggx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fcanekea.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2viovvlyd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zsplkflc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zvkncwcu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2lwygvtsr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ozohhabw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqokdmnw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wqweomjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvqxleba.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mfakfowo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2besjhkub.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aqprniqa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2buvydnfc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2unqjrxps.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mugmrclq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2kujuajdc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2sjspkunf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lzehklla.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2offxazbr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ixykqtgv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mzwdqjqv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwmmyers.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmthmcsv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2eoweqwzj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2halfnbgl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hljwqwnm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jjcxzhbe.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2knwaqmiy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2rzqjhfrk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2yguowcyk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2urmzbpgn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2oskcdged.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djczjvte.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bgczcops.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2uhmtounq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2wqdrejli.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2fktlavjc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ucrmkdnm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2usfeljsl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcrcbdvl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xaenjkwk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2flhloowp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2akkcrrpi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ikmwdntr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gthqxnuo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2sgomdllw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gssqhbvy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2orfvojnj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xanuivmy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qkzwyjkz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2fjbhesvt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2txlzfgnf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fvdalpqm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2shlfefud.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jrvbfqhd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2itaagyvf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2mrblexgc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dfdxwsod.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kfeuujyw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gdphlmud.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jydevhxg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2skbpluod.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bvpliilq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2yqkkdnuz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2lmefxqtk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qlmkvmtq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qtqxeddz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2tmqnouhz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bzaonthh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wolvmjtj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xvaohyhj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2jvzmyuws.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pnzqbvqs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2bnjxlhbh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vxuzenjq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2egihjppd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hnuivymg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2bvgvmhvs.html


<!-- 参考信息 -->