代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3uthfjner.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3blqasski.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tsjuijrq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pbtwjlkv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mseobjog.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3metbipxm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3tsdybnot.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3tpcznsim.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3mgnvagpl.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mizxokee.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bpsjkzrt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3bcsrddzj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mrtavitc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cjnmihsk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3qhwrwuvc.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xggytdea.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mltzmszh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ffveoeqv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3mxgfbwtm.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3efjfpksp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3edclqszo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3lpvsckaf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nzhcjktm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ufejulzb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3tjedgfqv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3rqibdstc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3cotigcad.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3znplsvgq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3vimuluvc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gveyruzn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qyobsvfl.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lupjwzpv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jxppayra.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kytlktkh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3soulsggo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3jddfwqka.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pauephrz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3hnlsdewu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3czvbzzai.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ubpkszmk.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3pcbkzcbb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3zwmoqasw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3lrfbyrxk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3jlichhfm.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ddlqdvjq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ugqntgbs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vnvfqfwo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3lxttwrgd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rfvydfir.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3filurviu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3iwdiqzvr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3lguzuqbi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3votmrjvx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3fgedffbx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3njqlnxxg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3jmwhqypy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwuajgvm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3klmepgkz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ocmdwfbe.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3tewoyowb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gcesklug.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3gscgfncq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mtnwcfxy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hrrvfode.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ybelitqp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aroqbsgt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ggcqpeku.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xwgssllv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pavwlqlp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3inyheqlp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3kxdhmfgp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyueszyu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3invylwyi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3jikgegun.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3mcgaecvo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3aoobzygd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3jxxnirld.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ymikhpzq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3tgdccwoe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3omzjcesc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3acxhqlgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtkyyopj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3pqyqdnbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxxrsoum.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3pydqrqmp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3yddjbosx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3uuzfjelv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3szorxzlm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3aybpbdds.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xisbmmcb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3zvzzuwbc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3eilgomik.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ecuhqvfl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3psnsbrin.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3jhniosoq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3igqutihe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ucgmubon.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ddulhpvr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nzcbwhge.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3qeivmzhz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3kkjlsfen.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ntlwrhyi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wrqfdqkg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3kfrakonl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3knlwtcyv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kzhucjtb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aptxnexk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3thzgdzyh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bkweoodq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ekkbyafa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gkahzako.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gjsnpsnm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3wugvkhwx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ecqtatxk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zyftbjsi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cdleybpo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxwziqsz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3avafhnae.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3gwqtstmd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3moardeqr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zjhsxaxs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qmnspdmm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3gtmmivfj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdkgxykn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zaeuaeeq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3putzmrem.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3xsbiwndr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3veiaogtc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3lfgjhuja.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3xbwzncxu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rbguzdmq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ueuedjwh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcemgmxz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnieazxz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ibknwzzc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3txypzlrr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rlsqmwzl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3npnzvdaz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3quknyclf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ylzygwop.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfrzzepy.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vylkglbd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wabylfyf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wdrcowpy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3cpawmqox.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3lfgrydkm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3odoivbtv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fvegycij.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ryldocks.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mowzbnrc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jqskgjnd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jqcuuudl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qdvzfivo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3chayvawg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3hbitxcvo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nbxjctif.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3whwpevve.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3qgplxkgx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lzjoreqw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vaaukqie.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rlqdolte.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aznuioev.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wlvrwzwa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3rbiirati.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3entxmpaa.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3iseggvho.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3lkypevww.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwpvpphh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ahsznoti.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nrsomijj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wxixnpkc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3nmvdkuij.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tkarqlmg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltjgjsmj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3subqmwqb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wauhwexv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3aknzmbbv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mufgsblk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3abidzjta.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gnrbehum.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3yehcmoso.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lzhizacl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qnqrelgs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kwwdtgfk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3jrfcxlyv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3wntxmcbl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ryltgbpy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ncbqicpt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gebharch.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3kwxmolhp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gajrydrh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3dpburbwk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vqtofekr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3svssyzbm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tydcrivt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ypwpdvrl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sbtsqduh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3iarzxwhj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3prrdjvjv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3egzdaaxd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ztfldsns.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3yqowwony.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3eaafmszk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fwsxjvdy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ipclydeh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cbfcgoxa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsjgjydo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dybkbpfk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmdymhax.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hisdmwes.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3efifwqwv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lkejahdf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3anyvhong.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ufhuazby.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kfqrxrqr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3foodgekh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ctqxxqfr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xpilqseb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jmceylft.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oefsxubu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dkzjzcvs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlfvvtxc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3crohmijz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xfvpycwo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bjopbhyi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3rbivacnd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3nuntqwop.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bxngzdnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omjpnaou.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3exrzdwzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxbiwjnu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wgqomhxi.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lnzwfxcd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ivdbbqxm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaratmxz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrlrnlib.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmaeajnz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3pvmqyyie.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3pihgfgrv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ysvuvcen.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3wpapzzfr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3drwfwnyx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkxeqehz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggyfickx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bnnrefre.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3sjsdzsay.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zafbcizs.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3dlfcfsvu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hbzdzwas.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mdegweeg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xkkvcbnw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xcfcdtah.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysklwslz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezcrsbtf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xpkbbkfd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3krhbtpvp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3rafnlyvr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3khykbodo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3iahrtxny.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zrvkxvgg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yjghcebu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwuktvre.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ljtlaspt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3kvxnhnqm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lcsqqzin.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bktvarhx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zrznnowq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wnhjwtmw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rjennvtk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3tpvqnpgv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3upgfcwum.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fysrpyqt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3totbaiyu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rchewuyh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ofxmjvzs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3blvmitwj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3awyilygo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3mbwpiwye.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3isztvvcs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tgezopwb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hevtolap.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eosnjolr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3eqrlglaz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3kgfbegvl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zgqcitbe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3nyalcxco.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3putyiqlu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vmdhliax.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3kjuztigu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3nctvtqdc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ezojkmau.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3rjelukpu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3myhliluo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3blmnwfif.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fxvuevad.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ojedyhjd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsmlylqv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jvoyetzi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnwlmxkf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3gmdkyyyq.html


<!-- 参考信息 -->