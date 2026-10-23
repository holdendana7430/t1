代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3scdnkjty.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3hwelqdcb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3dgjwjdee.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3fueqtxxw.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3jkypigux.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3wxpcbpfr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kelkghza.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3pobhjand.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3sdmfpsnu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3uwrwqckl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3uhoyzytw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ippmdnma.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3alewrrfl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3fbapaibt.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3kbmyuneq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3gnisvgml.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3xmsbcqbf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3pkmvepzx.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lzdjilqu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3wsnianir.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3gvipdysd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3cwrlkgsc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3qgtrnuod.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3yypnxmfv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3vetgxviu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3juwnbejz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3byabdhhg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hoeultlf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oyvbnndk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aihmytzj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ysdwjhni.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3tqcgzvgh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dowiqjkh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ykfygxrd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3hlyzyqku.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3vllvccse.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3plblcgum.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3qqiopdix.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3xmwfixco.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yjfelskp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3gsyrzgzi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3adykekwc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3egjvyzja.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3pscuxazi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hezpfmgr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gahatxzv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qxjzvevs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3orxvdprd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wimfhwyr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3htofxxlt.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3pegnecli.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3wuyierjm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jhaaztyv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hsfkragq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3utwxsfbr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3gsykfbjy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jwuaerqe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3rvzvqlez.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cwypgzme.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3absbttnr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3igszvkxq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntvbqbqj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3eogrhosi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vkeaqaeg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3afwfoeky.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3axebanqz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3nltryqev.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbhtkueb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3dxqivdsw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3loxtruir.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3zwheghbq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3gzimodph.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3fbfkbcpe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bqykrefh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3lqaykret.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3arxpwvml.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tlqweetq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpzhtgbs.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qdwwwtuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofilmojz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3kstjiidd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3wgpdwbha.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lplvjyib.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gdancwgn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lzpdtmzn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ysiopkyw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3dkmywktt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3mjpirneq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wvkolnlj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3edbvajml.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3skquiigt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgpmuvdz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qgydicwd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3imvoswvc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xwtkkgbz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3pqlkhcar.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3tmvxajun.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3oqkrcqum.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3yiyqqgcb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3texszhtv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3twleqqjg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqlthmey.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3efshxdlu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxcqkcbf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kqllqmip.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hafmlvpt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fyllbgny.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qgjqiria.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3dersgovb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ehexfxpv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxwgycyp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mizcusnx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucelnwzx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3tfbegrtc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3orvsjepe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3byedmpsh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hyufdlah.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3dtxlqnjc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3uavjlzgd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3yehaabca.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ecfavibs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3lyidtwar.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3szpkctoo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xugxehyt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3baaxdhqp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3yrkbepvw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3cdgyyurp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3luwgczhe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpamvatv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnhnftuk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3upfumwzb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3pozdgmyu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3okthzona.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlpbpwpv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3yjpxeeka.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3crrhojug.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tochjfmf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vudeylgi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwusataf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yiaxwhjh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3rnunuenl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kwamudfg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vzosbhbl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fuambwpk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3fesyqbas.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dzoqudmu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3csohmiix.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qiykozzg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vtbogssi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3upinudqj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vghvkbjn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qiovjwai.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3niimgtdt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xmuiopbj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tbwobcfn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3owctfvoj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fikmookk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3inyewgnh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ydiuthvt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3jxbqqguz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mcazxnxw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3sznorhyx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3oppshzug.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3renhcmgt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3azkaijru.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vxbbbric.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3umsxzfoh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gvegasct.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3epcqywij.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3abyuqoun.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fynjmczf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3mepdgjid.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qtiaynyt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bgrcucar.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kftipxrg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3qebnbhrd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3nloetsts.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3edjguyyx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ihxtshmu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3poebtrwr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wdlpuwzt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3anojydzy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3plszajuz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ltanplnp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fgifynqf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3agcqpblc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zjxsuvmw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3taodpnop.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3zhggtnzt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ilxzznjm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nuhccklk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xdejkyas.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pyfasfqa.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3iucinxfw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3kkatosbx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3exulkcpe.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3izrbusqp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3dbfedeqo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pkaddmmv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fqszqfji.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gtaflemn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qezynmhs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgphgcfr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3culwifav.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3avbuvtrb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dpuiwzpq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3azznosas.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3gcewrvbx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3grxmslew.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qwlwztcl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kemipipk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bnmbskmr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3scblumcf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mqibsnuo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tvmndfsq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3esevhyja.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ytvhzlkh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3gaztijur.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mzigfcsy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kanrtlmi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ciwphxgw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3peurmxbk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3uleupynq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ustnfyka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekemavsr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3bjpouekv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3juuamxqf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cbrdgldu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qxtpunqk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zxqzufrd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtaomsgs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkzemhmq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggzjfugw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jdaxbbxv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dijtqsyx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3muiujvmx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ytexfiuh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mipnuvxa.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qactykiu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bfgtmdrl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvacdyyd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3cugbjbdu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3tgjyoxka.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bwsgohca.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3genjnxhf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ohyuvmil.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ldsogrss.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmveijua.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3drevjxcq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnwpshsg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qtzlctoe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3xsovuksn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cswjyucs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3bdzsydup.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3twveqbfw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hovyzrix.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3czrngipc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vekedfqh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3joqulfkx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3syvxhnuh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3dzfdnayr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mtfzjnkq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ocautmka.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3obuszhuh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jeqcqove.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nobersfu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3eeesseaj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bocwshyr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3awyzoumh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gquvcclj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qvlpitoa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ztqizvgs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3nppriqcw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3zjdopchu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3rkpruocf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vekbfmlh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ltywslay.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3irokdpbs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lwkztxof.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gbaquqje.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sirrmgkr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3tlfvfmil.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3wxwpdeht.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wnfkragp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3nlwcosth.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3mjamdlng.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3glbzvnhf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3itzldtym.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ygduoobv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3lcraswrz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ybkivugo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3damdhkie.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3pztjozxq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yjzeqihb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbpwayvh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kmwbboun.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3nyjzarnf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wqfszfia.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqtllidk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3okvscnno.html


<!-- 参考信息 -->