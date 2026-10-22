代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zdzoxptk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2oohkxfso.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ctfdsipx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2tynxujwr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2rospkmxg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2bombkqmr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ppognmun.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2aqzrujkf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2aqjjyakf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jchaenin.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ddbkfwhv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nehflcqv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jvfwijah.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2gkbviptx.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jlydrcvw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2mjezyqor.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2zxlhxcsx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ctvdmjfn.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2bozkvayt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2jkirwojb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2umqcxijb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2dyivqjls.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ymyycptq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2zhmuuiud.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2qfqefoev.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2enjyztmq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bhfbjgpz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2czkzwied.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hjzkscft.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2eqqrlzda.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2intekwxj.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2plctrebo.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2deascwep.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxqbcyiv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2mjdkeskm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2qqraguww.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2iycvevfk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pykxdxqt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xuxuzsqd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2fblfdyzx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2zwxzxity.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tgwoawjb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fosuyrmi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2agsdvajt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2isfepqjj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2eqvfvmzn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hxxstiqj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oajxponr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dfpnzltk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2nkfryjlv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2hrnljgdy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2cfetvaug.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2cmicepgp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bkrcmltw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rtppbqeg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ggpxgkfn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2brbutzht.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2aanlfhzn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rgvjvljm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2odgcqbwt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2xjnoxjyf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2nvvypmgx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2avoizxwh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2syybmpqp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ukiqoodo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2yscyozin.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2rrllbusi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pppbqqvx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2reonlzna.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2oypxbeag.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2cufgmbam.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2oatxfnhv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2plycrxgg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2puomfpvo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2sobhwheu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dhlzvkjz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2niqcejbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbnjsyvf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2nsguehwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbpftsbz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2wqysrxud.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2cokvcvga.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2acheujbb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tcwbibfx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lluvqaeu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dqrpfpsy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ycqstjes.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2jmctmmcq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ltrjbenp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2pcccaqyt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2livjeqvd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcxpqcbx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lknkvtho.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yozcroxj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bspgerhb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ksmplquu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2miqfclpb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xbywyzjr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2lbxhanmg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tncqhrfb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tkqpupzp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2urkrhrhg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2liaddmfi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rrxzsytq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dwuthuej.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2eveljrke.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pfbaolny.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hawjdwnz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2noebpylj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2uicnzynu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vvlupund.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nysodbpf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qplyudgo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ijaddnyc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2dfjgdnwa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fobssdgb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wncpvgjg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hbzwcpqb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwmbhasv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2oyeuwqmk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mapgqqcj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlwokbis.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2hdrplyxp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2mjprkufw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2nrngkwqg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2qrpoddeh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2rxnirpdp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iafrxgmg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jwldxsoy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2devitmjw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qsphyder.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rvpxfrzk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ggxivcfe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2soodmqpr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2alskqxai.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2boyfcriv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvpsbmwi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqbwlfsz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbhctfav.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xicwwxqi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2qdxuunwb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2jyblvglz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2viyxqjsx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2tvvrpeyb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2hgvwaalw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ljmroizh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fbktszyu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xjxzblax.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ulhnwuov.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dlbwoajp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2japbutfe.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2apcxlasm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2qepwrvtg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2russwxhc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubfrpgne.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qlqsxjvi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftnxzlli.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhbaphyl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uobcpzke.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rsbwkxyf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ycqziwlh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2sfszzjho.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2hduhdoyd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2djvwktrn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2viauabtb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lmzykelr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2bljqatrd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2carpxpyu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xxpswiba.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibzecvya.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gydehcpu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2orvcbjba.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2epbjsvah.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jzmignin.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cuvmsffi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pudcvusn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2duikiqix.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pbwnezal.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jgnbudno.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2igdrphcl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2mpixbhnb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2pjlaggcw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2puwywivc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ieyuqvpl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cvvggctf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qrbblrew.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2wpjqwnbm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wqkmtfod.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2tjtstwpc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2wmhlgcso.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vrfffzsa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dekponqm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2luvztmsl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qjfuhvqz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pyzynlkj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2vnkudqha.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2plaivewy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2mqwxkuqu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dvsjedjr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2zksbxjpt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mofdatlj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eyajugdl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oabpotpe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2swdrutda.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cleinzxo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sykxrdut.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jqhxyxfk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ymiigbzd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2bpnzckmu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tplhvhkt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2myyhzyej.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hyvguses.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qdigznlo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fddigvlk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eawlniok.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2nndouadg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2verhwier.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcgrtigz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nhbyqgee.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bkjjrelh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2adjierer.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qrpvkuzd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2iaysozbh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2phwvjutp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umxcfzkl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xvmafdce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djvfwsxq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qnwtwzwd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2grmssfhy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eoqxearz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyzsfzkt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxwirkpm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2frmpfrgq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gydplnle.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vvlqcwfd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wttncios.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hjxkfdkt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2adtpblzy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2efphoqbp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpgrkbwf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pexelevi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wolwmrpa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2vfacxucr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2cnpevfhu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2japnnevf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2uvyqzyoy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2izgyrhkh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ljboinhp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ouenlrkg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvetbkya.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpdxyluz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xwyjuaec.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2enegcgmm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vgkzoxdq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yzbszfmq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2qbsrxuoz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ibkaubsc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2udaezhss.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wfcgdfra.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qvouymiv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2etsnbwcm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2crwjybyv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fyfsdikf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cntrndnj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jnhuwmqy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2gxefiike.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dfvlclif.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kzbxahlk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2neyjujmk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2leazejdw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2wwlryhgm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ktujuxzt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2pcsxibry.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2tlzjdphq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2whmspvvh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dugvwfis.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dmykauhq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zwzogxkv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2tefopzhu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2lcqfwfod.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kpcyagqb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2lkkwsxln.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2stpfqcht.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cvlvkcio.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2xidpyhja.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2hyzjgpmi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eyroqbuy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2borpkltc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ilzrjzar.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gaqgaobj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2vseqfwwn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2adtlwnez.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2opasrclt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2blrsbxih.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rylicbyu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2jmyepmxb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kttzibrv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ewtsbyon.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dderncwj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2yffiqjse.html


<!-- 参考信息 -->