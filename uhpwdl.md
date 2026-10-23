代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dbbsupjg.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3wnuttaht.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3dsvtainq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3lvlzvmie.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3yjjyzght.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3crxhkwpl.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mtbriqks.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3bvitzihm.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hxddozac.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qegzzbdo.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3tjihvcmi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ickdxatf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ajyseywe.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ownvidst.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3oqcgkoqt.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3rytyfdgk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3dlegieon.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3jvavebaf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bvmtiwfy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3aednlqtz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3itaowrhr.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tckqfewd.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3xkywmoep.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3hnqdepzb.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3tnzqapfh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ryltptia.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zbntebaq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3skkfmbbl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wbpzistg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rmxhgejb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3htgciznq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3vpxmyssu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kcchvfmj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ymcszmzh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3tybofpxw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3qjgprtoi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vmhcjirv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3khqedmmf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3arsyuijv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3rcccyicp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ifupebpk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xwqgnttu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3alttkyha.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwlkxpvh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hudsuglt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rojhdrsp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zdmdkvrc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3valpzyyf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jrdoxtwl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wocblzen.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3yitocsum.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3jrsbixrx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3vcwufiie.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qgtlruqk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3itvlkqze.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3jznhpmwa.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3infzznbc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3xqgbhowo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ehyagbyy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pxhfxwll.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jxwrkqtl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3qxpqiyvr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3gcngmegx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wdaxbwzm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ngkdcyee.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3iawroskb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3jpszbavp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pfhpvvfv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3axwphxpu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3vqoyukpo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ypqaentx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3grtyfkzo.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zffadbbo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bamjulsm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3kpsgzgvg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3qxzyeyts.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tltxjvnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrsuecid.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3zrhbgqri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icwntbsr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3rwxmijnp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3anbyrdwj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vijoford.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oxxidogk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fbfubpmg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wqhccplu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3whbzqmac.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3arqhuetk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zaewugda.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jnepnjhm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3pfsbwtll.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqypyvvv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3opmuqees.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ekeawoeu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kmxgzlum.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3gotxebfj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ywwvzpkf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ozqfjjbp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jzrlitcw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3fzpuqvad.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3adcsaphf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3krlorvve.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgtzjbkf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lqlygrib.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3iocpqoeo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3mckllreh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mlifgogh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ajajmwhd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qzwiadqp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3eypknvlf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dyxmrwgd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbojcmcv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3nbzexkcj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3omudrriu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3wushsite.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyiulcsa.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3srcpnidg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3oompqfdl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylypjayh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kmlbekep.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3omjzbinu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3szrazfgx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3cabnvcoa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3eyghlvco.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqottuav.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ousnmpkg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ixbejyak.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3mkxjnyvs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pzsupegj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3sphwzyhi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ktrorjkp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ppfmuved.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cjfdldbb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdolakin.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ufajiilb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3idcetezn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jatwmnhn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgjobjbf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jbdewtgf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nbqgluee.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ciadsjyh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qbkcqros.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3btctcdge.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3eyjvpnbb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3polykrem.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ktnstxeb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lstnxkqw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mnrsezcw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ixdclyra.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mmmrbebk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wruukhta.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mcqoazfb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ysvftueo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3lalpnfhh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3khuextvo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oizjpjmp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngzusfji.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zzxzfive.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xvjatdbw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gkjpwhla.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jscosqjx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3tsdewghq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ftmzprpf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zsxlauoa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dkxmtrts.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dowmdaav.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdfpvubu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3evgzzncg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xihzxftd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jifmagmb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ksatpkqt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xkzrubmy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3hvzadcbj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3opegxxbz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yyejiaiq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gnsvkjnd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3prspbrmw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kvldasvp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3xapezdut.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tqpsqxkj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3furzgsnl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hmksllpb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xgelunlx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3agblleuv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fyxghdeo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3iyxfxiiu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3fymjmuvz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3eyiwkagg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3qrnitepv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zzvxpofn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzkppzil.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gtkpyjya.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdonmhix.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3clifdirp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ezcudsok.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ilericds.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3iaohpaik.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3nsyyodds.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hsbomggy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3kktaorim.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lpypwwpj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bhwsfwui.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xftewber.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3aebycnyc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gqogvkxw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtuexwro.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vwnjxory.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3znaxnkbo.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3qceaaaxz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fjcimypx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ckqkscph.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xqhttoys.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3opffifcc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oppgqcxm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ltbfsyzp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3welkxeke.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qodfuevh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjvwukcf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qpgzopxn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3csowixsl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bilnhyky.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ayyemsyj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3dwjgqtji.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wkltpmtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpyzzyiw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3rxblhjfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsurcaht.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qkfkttis.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3qxhmuxrl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pphsxfoc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3loilboop.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3evscubvf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3stbfebrh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3yalwrkuy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3pxqupvsd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3swskkkaa.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zkyuivwk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3axkobebw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brpzleet.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3togbkjzy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lmfxgsoc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3nzrorwms.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wjjkeixb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bbfzmafm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3urhofsog.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3daocbvnj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3vhgyultr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3fyufoaqn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zobgntcm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tcxeybxn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xrxpefes.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3qdqivpat.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xbacsyvq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3gubdbtpl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3stzholmv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wdguavpz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tlgdtvac.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vlfgfqmu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uvogwbuc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3colicenv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3drlmjwxk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fwezmgpz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uegxaoim.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3jcglilra.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hktnadpp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ovktiyvs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yddmivkw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3egqjeviu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ckuupmvq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3priehibe.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ealiyhnu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3limwlrsz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cjmqjjjh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3pbubmqfa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3syyfczav.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gyzlgusi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wzpflknj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3yspfpkzb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vescvckx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uqhxfsfr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ccovayyw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3odgsjpsp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3qpawvbjk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qucviklv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rldazuta.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ptyehcvb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nsoljzob.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ibfdplzz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3nxjocbcw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fcywtigx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3wctpeozn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zzpoyunm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysptbwvf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjgaqubn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uxdnkrkp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fqraizcw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3hqhxotdt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xyazezbm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3owruvqiz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3haxqowih.html


<!-- 参考信息 -->