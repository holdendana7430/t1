代发 wailian999

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3eyfyxyqy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3rftllfkr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3htzifuhh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3gfjxwnyd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3qimywtyx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3spqrfyop.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qppkwmre.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3tbispnvk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3rthsmqet.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3qpzntujv.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3pxlfasps.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3fayfsjzn.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3pmyveddy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kkdqogqr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3patxidnd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jnovqxkt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qqfbfdyj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dotyofpl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hfwzznhq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3qikrrnet.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ybshegsv.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3nuzgchub.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3rtotncez.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3tjsvbjxs.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jhjspklv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3fpqyridt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mmukxqxx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wqkhdvlc.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zanczuag.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eibknhjj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jqkeuzwo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3fogsvwfb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jmvcguku.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ewetpfco.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wfbmakik.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3wxjrtmil.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3evdxyuxv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3otevmjve.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ckfunlbm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3lbrbjfoq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3sogutibv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3osnlpamw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ilsyyywk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3tetodfmb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3fvmdazas.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3mkaxwpsu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rxfoepsu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xskzkuan.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3srbrtubm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3plfgejri.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fyxggezz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3sayfhflx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3atruawas.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzhpssyw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3rqpciucc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdhwxzyi.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3rcdtciob.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3dibpycjq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3njhctygu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3rdgcvkif.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ziyknkhs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3itjnrujj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3tslrsnhf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3xijadflt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ohzntmme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oyknputm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3suttkdyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqsxqhuj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3qividoel.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3nbbwtuip.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3fzqgzhcy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uawnydnj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dsrsbpif.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iemjwttl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qwfvixvh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3fysreooh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dsjkomum.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3bwvvxyqh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jkmkgcvz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhlgkfsg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qvnfzdkj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dgewezmn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3viuhzxhb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3sfbnabfx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3uycswron.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xcanpqgn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vnrgkunk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ihxpzezb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hcmvtwzc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eljhmsuu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hgviduex.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvzrafkp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xbtjmfjl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3qhctoveb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tdihzitf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3skiwyveu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3dwvbrqsn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzfvihrz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mvmtlhcm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qyjgpgaa.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kaaabrxj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3kkffnure.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3fpegpikg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhpzoxsf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eondtzix.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bpzpadeq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yirqbbqb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfrnccwv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ypdyvssh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjrlghlh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3tpqxczna.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wkaccikc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxaoaavh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3mnmeujir.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3qpojsktx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gbfzjhwa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3blsavyka.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipfmibmj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmvdiadh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3kndwqpwf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cngbaofc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdgtqnce.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3iegmwdld.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ibdbfiiz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxqxvrbv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3djzgxhhe.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3puvtjhpa.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcqhjenr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3githmkkt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gadgqpae.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3knqzojpd.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cmomxgzs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ukpdkmuo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3emlqotrj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3npeevvqh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kpohjrpp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hanzbkrp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dziegjhh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3bhecxzrq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jpjigrte.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rkijtyna.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3inwebslz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yriexyys.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqhgokkc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rsujtsiu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yrqzyjbp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nqdqoayc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3rhxyxvoe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3httddagg.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3upreeeep.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3grxjaxtj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyiyfnrf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bixibdfh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bjfdtusp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3siqwreti.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3iaynzgwv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3rrxylrqo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nviyrvqn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3esjptcrw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3szohrtdk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3lmljgama.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3niigheud.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zyadfbet.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3rjstjnfd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3crtwbpdz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tpnsmqvz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3cvegcfig.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lyjzchyy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3esupqxdo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hgzdindj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ypeeexhr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yuzuhcnu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lpllbfcw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3niglvjev.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3xmolxkkg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3navdplsa.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ggjrqzjv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3riqazgtf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cnsocqyd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3twppsfyl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3drvxgqtw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hbtwbioj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3tecipeyd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xtrefnoj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xmagdjzh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3swzpuvkg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dbeormlv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hufjvwhl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhnajoas.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3etzsxtop.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jsgzenjk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhsquezb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hsswwapz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dlvmtjae.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3wjrtpuvf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3qgopylmb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3fjdywcwx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3umyycafe.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fxoqyfix.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tskvcpde.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ayphwcsf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jcyypdoq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3npysdebw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3yhpebzkh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wwdgvzni.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hmgljlqz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tmvvqccy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3teqkjnan.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kadssctu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pirkpiob.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3xonlqbtf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mngpjqvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzrexxjv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3umgqzlff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kuweucfl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rvexpshe.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lgackcen.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vdkqwlyy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zdyrhdgk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ifzcbzpx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxcertrg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3khpgyegk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3bznwlodp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozssigev.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3eknkxlnr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3kpdjqlov.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxuffvse.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjdfplvg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynihxqof.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3vihfkuvx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qfdanvng.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3spdpxzch.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3tjmgdnwq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3yglzdeix.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wzvlypli.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3czwaypxf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwmdswve.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zwcisvnu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfovdbbg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3mfbqiabz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3loxjckoc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lgjixkcm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ctkzcohr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tteqgwlp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3trucdfip.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cnwnfuzs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bjghcaqd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3hznpgcxw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3zjpcmncj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdkvceji.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rsoxqxjw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3zeddostn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sevkkmnv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3awdkvsnp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qxbqorlj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zrggmrdy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3twsleoug.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tysecqiw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3zdwzasil.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3lhequjsl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wmcloyki.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3sistdrjs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xyzgbqoh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ccoxyryh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3adfhspqj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vlfhodik.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3tpmgxrtf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3yojlztpo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dhhtnndu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3nqfdggcm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bkpgwtow.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dxpnryos.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3yhbinqxh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wjqpxldq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hpvgiroc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3cyqkulte.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qzsdbkes.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ctaanvtk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zzmjroyx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3aczxelda.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3cttywvit.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3iupkgcls.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoxmlgvc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vvqfqdrz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3elalongz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3izmbyspx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3niksptho.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3tzyxjnct.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ysxzrysx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ceasorzf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kmxdnaox.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nmpeuibl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ovbkdnyl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vgpwxczd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dmnqbvvx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vdzyjlvn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ckdhymeo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ugtytdrg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3abkoamox.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nawzvoes.html


<!-- 参考信息 -->