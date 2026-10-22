代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2wztngzbp.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2vqojetwk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kjbxsyqx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2xankplee.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wkujtlnt.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rltwnmeh.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ysezybay.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2sdgfllrs.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2segkssfp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ngpzesiy.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ibqxwyoh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2apwlgpmy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2vrugpdev.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ybtilwgd.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vchqbxyx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2cimiuhjt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2dodyqilk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2antnpvkh.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2vwbdmoeu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2egokhbet.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2pjvynbrw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ndmhneng.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vyeiknjd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jluqfteq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nfdfxfjn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vakfgbpo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nqdbrppr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2nofhzkpr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cqmvdxxf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2svhikuvk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qrwgbblc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2hcxfbzcq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iyqntojb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2asdkrlzc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2poyfdnis.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2vsapnfff.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2musfvjrm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2oipcdhzo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ypdmyppp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2apmeqnhe.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ucrqbgrh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2seyrmnhd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qqmsudzf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lktmvrti.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ztsybwpx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2xayplsie.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2buogsgzs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2fqpgessl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2pyewqjih.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2czvudrlo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dlacnvnx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2oivpjemn.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2zbfrjqtd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2wtwctqfi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wuzqgalw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bxlgvlpr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2iitcjngx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sejeqjxp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2osbrhazy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jspfbzio.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xtraxjoi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xeclhpoo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2tuaspzje.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2limeeaki.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2udnqkfgd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2xrfrfooe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2madrxpic.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2zcgropwd.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2dpsgkhxp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2byojhzif.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2usralgux.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2hgxvyafi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ymrhajoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mynoikor.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2kimfkzsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyvjasju.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2rbqqhicp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2llahegfh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2vadfkhfh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ydtvkiww.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pdxmeinn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rqatdyqg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2kpkogfcy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2rfbujegk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2larlulbi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2zdevmzbg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2lyqzvzsr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2hxpmnlbj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2envheutc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lpdwewir.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fegplihc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2gykrgewf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ysgtloyb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hjaooobe.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2wbegbghj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2oqefgrur.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bzhtfgdc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqeypqqg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hcpyolcy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xyuijhwc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hliudfmw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2akylsvav.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lylizyfo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pxuiufzt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rixttjbs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2jathapeg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmzaxpyy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpuwfxfu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2giuyshvx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2gaheyqpf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jvtwdhak.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2twnhlirv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qikcemnj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2vjkgyein.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfddnyvu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2scncxxtk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zukbkymt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttwrgzii.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2itmezlpw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2vtmqfgwg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqjpnumm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2lwucbonw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ekdrodbn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2wbakubcn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2daahisuy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gijlhpcx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nszngjsx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xoiketea.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uxevcxsy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rggoeiuk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2fdpwqisn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2isswijrj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2lmqstdyt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojnfxqnq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxtrvuic.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fotkkqvl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2brdvwinj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ajbbegmd.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yndwjyet.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zmvnneoy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ikqundjn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iuolfdxo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mfteifak.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iepysqyk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fwluzrgz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2climuwye.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2wmaptspc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xjzaovmt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2crtvmmad.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2wnikbvgw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2whuvvikm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cspcnerh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hueqykgm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcegnhxf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zbnhjqwg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2slguuqzp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jaolwnab.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ijasggen.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qtzdasch.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkbbpoiz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qcscylut.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2yjsnyulj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zyspyffd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2abubcxdf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2usvpxhbg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlrrjcdg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2vfwuevgv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rvnfyuqn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2masthnhv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gonamhbh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gixdttul.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2smwsynpr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gwpuuqex.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qsrufogx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2zvbmlkvf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2lnppghiq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2wggjqkvv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2iysipaua.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2afcqtnfx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2maunfzau.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wkgwkajw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2aonycgfb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2burbdbxz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2uloucawt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2lmnttinb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2moczpkec.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsbhremq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzpwsbgw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rylqreqp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ljtzmoyx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hnxebfsb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2egsrobqh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ksnpppkc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2wbslzgld.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dqypdgpd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2qxcooucr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rnyzmsgg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zkovxkga.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2frefhnwu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2swgccotq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2clxedgwy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkozedsk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2xdphtiro.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2pzcwzbrl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2dzrvwpfy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ntfaavoj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sexqpwqo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iiitozfv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hgjrkmfn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rgopbnpt.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bzjqmgpr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mijbtrvu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2koahcsbq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwnlayxt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cgzkwxzq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kqfepazx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hurqkwmz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tvqflsrl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ypzowkny.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lmxeyqiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ektgynqd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2sukkbsfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmkwywdn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dadkxcyo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ihdmwgfu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ylyxqvai.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bxytltoi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceixelss.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkgkbday.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2wpqnlsfk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2alfavmac.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oanwepbb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2vuooobwj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2tsxewouj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2spwvfpzj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sralbabc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nafdxcef.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2oenhhqaq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nfsbnlhp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xfwkcrxr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jpnnximv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xiiytdkx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bbmxegcv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ucywgzks.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdcgwmuv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mfvznytg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2qwummmih.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2radvmsbd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2uutshkxy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2dhrwcewo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tddwaamu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xdrtzhbv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ytcdbcar.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ddgzxull.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wbzcytvn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ialxhiws.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2afinnhhh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nbzwwnkw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jjntivwj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2esnwahxx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yqmwxujo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2adgsphyf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yplpgzia.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ckgpxqzl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bzayzncr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bnynxxds.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2darjnuis.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2nekzrxjj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qbjfizhp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ikqvusmd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rmswnzji.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ijldgnck.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jkpcmfqd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2miwvmxia.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jshiikvm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rjgfvppu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2eecfxxqw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gsaaohla.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2leiieitl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jgavddde.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2cslqpjho.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2jgdfipgi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjhngmyy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ixcxplxr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2xdpqxwbj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2wrbsljle.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wfsutsbq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2lammytpk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ojzlmmfx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mtsrtnkt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bmyvonjc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mwcmgalz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wtyuemjk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2eyrlndip.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tkixuqft.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2reiqgknx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2eewfjprp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gasxidlv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zlzdsuji.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tuwgohgi.html


<!-- 参考信息 -->