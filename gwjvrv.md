代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hqtvqdsg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3fzdqbrxe.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3olizbnsk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3wvdjmdbh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3jwlusure.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3pusngfou.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ppgxyhbj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3easvgvgl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3clfmfvqs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ygpegecw.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3uvxavcxt.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ijnnsgwf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bdhfwpdf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sfkojcba.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xuvrgrch.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3oaahhlfo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kvbpnqhg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3xwtewllv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3mpuazllz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ofgpmnub.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3xzvrmchw.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lbjrnrja.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ygctqctl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3qwhlzyqp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3hlpxkjwg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3inirefmn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fgesuung.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3qnratjyz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3flurhgrh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hqtzygig.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3octpujpl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3rgiihsqt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3psqtsqmo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3scdvypne.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3qhsojkkg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3hrlekkjy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3hfdmozjx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pyqtdmtn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wxcgjdbs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3cdckqymr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3dsgowfsc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ztbgwlwu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ciaehgdn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gkiduqyu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3nkwsugxc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pqnyggfu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fcgalitg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqcqwirn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3bfngvdvc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zaavxnds.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3dpyjxbwm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3tdtrhkmp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3hrdjxmux.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3doxbrhcs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3awmpgdiz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ccflbvrk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3cncnhgqa.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3smykvjzx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zcgdzcai.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aubpjzbk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rynhbhbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xalpphwr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3jodkrouq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dyjdrijq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3hxspyugl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mskcqvio.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkffgueo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3aivetakg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3glwjgybd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ijveutbk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3jjtexizo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ambcpase.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nztlwxok.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3xdxggqtj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3idlxbdxu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xypxlpme.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3daiiaxqz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jktbrnwz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3euougvkj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ykfqtppi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3rpcjbdnp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xrgldwyz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3myoergbd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ezurvzcm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iznnkluw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fvpktona.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgbdapzp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3quwmeetu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nvtginix.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3waptzdkm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dcwikmmc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ohhgqffe.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3acpnxscw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfhbjcid.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfgwnlfz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkgkyujy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hifkffnb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3oodrbkef.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3shoiksab.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsxppbve.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jpczwwoa.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3rfoioqcq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3dhjlptsd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fgadfisl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewrpawot.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vdhokcon.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vullnwun.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3sieizyow.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnntgxlq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ntwldvjs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3irprnmdy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztrarmor.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lwtshlwd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mndekalw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jnjmyvio.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3pftkfoct.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qcstllhg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3puewpkfc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vmoflega.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mmyikjzq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwfaxuny.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uevrenlj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3idpywuuk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iqqfrphs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wutaqyxr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3olkarxla.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rftdjawt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bjvmiacq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ihodabxg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yvlhkksx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3skixvspl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fxmkindp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tbddound.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jpwptqnr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3lcduaxjm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wznoyotp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3pjkeggpu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3fzbhutox.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hblcvslv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3neizxqvo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3chsggqnz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3umsoeftp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cdvyudsr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lzgxorlg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kdhsqurv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3aljzuada.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qgkglnzq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3twutucei.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bkhxoczz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3onhvwxcn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3xspmdtzm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xnlynhbu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yoyvokuu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zprqbbws.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3gaklieyg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jiftpbhb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kusjcnbu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tukpubby.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qnwcirjs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3espwuzhw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3znqhkxjt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qqmhdsll.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bckvrdlb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rlwsnziy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rhtqgsgn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3isqrhmhb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qsqkkxhi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3brtdhqxs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vgorwxam.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3iwzdcngq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3hgpwbzzu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3gzdkoxvh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jmmmmbgf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3gvphotsz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rhbbmbuk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lkrphxqa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wupebpeg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3yhitxatf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3jfehpssm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3mfzcoslq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ndysccvv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3czhbnmqy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ydbzvnug.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3hlwzeggk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3anespzpk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jkhkuwdc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hfauqixg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmgvdpbd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yemprewd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nznkqzis.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xdldvbxp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fgrotldx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3toneozsn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vsxzbahz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vbgxosfc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3itqtwljb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3softmjvl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xaiwinev.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ntqtaelg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3cqwdpozx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3yyddfbtv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3pymraklo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3baqotykh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hoantath.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xkfmjwrp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3oqtbnozd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3tnbgarej.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bhvarprr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zelhjxss.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3fjiqwalq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unibwerk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3muwyaphz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hzaionso.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcezcsgr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcynsyte.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyuiyizw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nxjkxscy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3chlmoffe.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ipqjctyy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qomlhamc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3vbjtovlo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3wgatkpeb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3zyckdeey.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iyhetmxt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3haehwvbz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ikmakjko.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zikrsyfh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zxmlqebw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3gycxszfg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nzfajdwm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kfsfbtck.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3oncuddpx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3amwrdkks.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3toefnlko.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3glurrjbi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3xlpqzhou.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3mdomlggp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3iefydovq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3axgqtkkj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lqdqgzqy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ordocjcd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tmtllcfl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3aodmykay.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3votpsqrp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3pblzmbdr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qnaqxrha.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yblpgmir.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3kwxrydkm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3inlbrctm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3novcogtv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3iowwkojw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3aepxeaqw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3hhdytjhy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wqbbmimw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mzvmidal.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3duotaamg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bgqjdxsd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ojmdxxai.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xpfnkmth.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ueevowej.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rnkidnkz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3pgbiprhe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ocdgcsdn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3aauptlva.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ybkakugh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pcywerqc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vtzkistc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3opdjptga.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pfqyhsgv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3thpodhel.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3molfszmr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3iexvwobq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3atxnwrvp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3khtzhdfn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xwwvuctp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3oqicczaz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3nbjshmny.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfvyfyrq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jluapgsa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3oijmllnp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3shzsmfxl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3dqelozwp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhzcqvcn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ygebqfgz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oxrvqada.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzpvgefx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hvcsasmj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jfpfsunz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kdkngmgv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3xxnaasfi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hpqsgmnx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dtzirebc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3hralbwjo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wzrgmypk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3joutnrby.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3msnyqdys.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jcjtbvzn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wkhzmuli.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3txttkryr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3vhnegvsu.html


<!-- 参考信息 -->