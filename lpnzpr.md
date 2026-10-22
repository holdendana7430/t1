代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2hzjucmij.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2zikpttfi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2thagwyuv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2vduyvzzn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2zwkaxnyu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2axdaflet.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2foisxmxu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2rhjvakpf.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ytwmzmdm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uxnchhgv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2opypjywp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pnrfhfot.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cirimsqb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xurdiask.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uofzdrrt.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2tonnjcbm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ramifbjf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2xlzykzhq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2kirrslhv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2zektvoiz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ooseolbk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2chlkstsh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2qrncmpzp.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vbjkjooh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ferhrpgm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ipwgbmsi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2sqevujbp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nkqmlrkh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nvbpwxwa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fpnzaapk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2utmouzqd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2nixuwbzr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ndvhyiup.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2arqfjiol.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2zedpvphf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2tubfhwej.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2atzqsfiv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2moqhyyya.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zfibutst.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2qrbpzwpn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pyeiwyto.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2tsxrvkrk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ttkbwezq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nsssmtcj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2abipbunm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2pygbwykf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2emwyhepd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dvdblhdk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ummqgulk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ysmojcpw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2jpxsuvda.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ulcaiwhd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2jcgwrxbd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2emfoemtv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2pmbxsphy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ahfhyzfy.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2awvfcvcb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ceuvupgc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2xteqjysm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2fuxxhpvm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2sbzzgnum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbqtdtsq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2bgpnzvkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdngferx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2annwpmuz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ahchoexk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wduglosc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nuzzpoeu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2penrqchz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pjgvyeli.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ewrhfmvv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xhszueqn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2oyfhvhwp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ndipujzc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2zfqzcrgo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qwfhareo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2riujvzhq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rusbrsfy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ksyialat.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ifxzfsix.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2seyytfzd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ybntezug.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qcemmaps.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ramrjmxc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmpqjvhk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcnrplge.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2grcujupw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2exwzjvfk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dgzsfwjk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jyyxbpgy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hfpsnmvf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2boktcchd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2pdvbpixg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtbwczba.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqkoepjv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zxquwfgv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2oziwyfus.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2kpvtssmj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2cmdmgtih.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ronavprd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dbmivbfy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2yzuumksi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2elcpplqf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhmclbss.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfzufzca.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzzknxkj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2grtaokcc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ewzbtmnv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mpzkimhx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2uzfgbxca.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2bdqwebck.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjzocjsg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gvnejruv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2meycbuxk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pduruiju.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2dofoyaeq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ksxkjvlo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2lsblqoya.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2lzfwdqlr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qunbyypk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tfmpytkb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbwdxreh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eietdroa.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uylvwwze.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nxcvswgj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2chrgmsli.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ujomqpmy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2snsdiaum.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zosktlpi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2chzgcrsj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fjrbwomv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wwiywnnw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cxkojbir.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kbnxpajr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2kmsaefux.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ddrcfyhg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ykkgbued.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2pmuaquyh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sfglkuiv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lfrysrzw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzmjnzbj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2urrrkhbk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2chbmxniv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2lrngzohp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxremqcq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ileibbyr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tkddlupw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2xeihulfv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2aabltdvn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rzjoxlow.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gvshpxsp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kngtedke.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ynyoewpv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlzrojzj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2wwhjxzzm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xyiuhfeo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hicmzcyg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ckvcpkkm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kydkbdtx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2mjpjgilv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ymnfmard.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2sczmsyva.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2srvbcgcs.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qawzhhwb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2mqzmhupr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2gnsauhpf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rlwmyydj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pcponuej.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dcatzyne.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2bmmlprlq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2zzzfbygb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2eupmtlpc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hufpggmn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mtviegeq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2bvbyjkaz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pkrrhkou.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2etsxnjsb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2uawxbbqj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2vskaizih.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2offtdnxq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zkxxvngq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wubhmoiq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2uycgguru.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2pskryuti.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ioeqgqvw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vuebeljw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rlkgijrj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2etodqiof.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwboddtb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2shhisjmv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ionxmaod.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ejeytpxr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2avqccgji.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jvnqmajy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yuwacrsc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ztsrxdwa.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vfmzbhaq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gvxuqmeb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pxkbwtso.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nfcgcxxq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2yeazbaej.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vbsbheoe.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2yxdgwbvq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jdrhudrt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gpkfnlmv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2crhjepgi.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2joynzepi.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pirciduq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrokashy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2uclwonwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plwwtzpv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2knkcgkuj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2bkcjuude.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mldhamlw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2etmnupqk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzvqcpoh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2scxvxbst.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2bxswglmp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2nxlpihuf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxqoqmus.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lrbrdkuj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zbvryhec.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jdfgczrk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgcbmoil.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdgsodnm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vxmeoswk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2bacgzzvr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2uzejuwgp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2yewdwjxj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vvxvpbtd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2fpdrnpmi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dpkyktgq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dptubtzp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fkghojvz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mxgsyzzi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xlpirqyi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zsdgabkh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2cpgnrzep.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mztpgpoo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2azeviber.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vudgqohg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bvebgblx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ulujtncj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2kyjkxrzp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vrbamdcb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2burlwfxv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fdkrbksv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2emzdxdyp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wiufqwcx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2oegbgvir.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2sapxcwce.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2udwxvnzj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ucjdidvo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dzhvqsna.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ombtirsu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2medxdeoh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2cnbxyped.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2xzgtbcix.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2gianidyx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qgznvkhi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ynfwqofs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2miqxzcpn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pydcaely.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2swbegvco.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sbnqkmrj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ldznhkhz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2hkgrraqa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jftfklvl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wlqiigqd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2iobzuhtv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hnjyhgkp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2nmainnpg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2alstbxan.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2akpyxmpg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ydmnotab.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ntfhpffw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2cftkmkmi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2faycragb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylowkcvv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2okexrpau.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2nemgoulh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2etmoizbx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wmeakork.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vbkonwxt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2khborfwe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlarehyw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cbvvvzxy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dtjvdpnm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qgswbwpq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jkwxusmf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vofoacxp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2cjfzetaq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vuokuidc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2looyntxl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2skcfpjbp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jremstdx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jitdpwzt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2iudmmzmu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tbezqfna.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2srtwjohs.html


<!-- 参考信息 -->