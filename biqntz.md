代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3fbdoaykk.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3lbnivwui.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gmfrfyyv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3gjewmvlu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fwztouzn.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hjtqgzfd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3qrusjcbd.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jmywwrep.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fysafcmj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3qjkhvzwk.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3dujgsytr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3hcqukfrc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3fohacoas.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3rmzruvaa.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3gcgambjs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3fcgymgij.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3oxswwhoy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ljkfmaze.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3cwvhhgxb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3wpfoqsmt.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3pffhmtap.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qlwffodf.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fbawfkmh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oqfdfpwr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vmwwqawt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mdbozece.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mquktvpe.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ubdkqhtr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ibdryoqz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wjpivffa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3gzkqfpjs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3qypfmowp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3rgdcsjyf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3lyhhbngu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3upezddxc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3feftjwbs.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3gmorwaaq.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pkogdjwz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3xqnazqpq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3nshmolsx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3yijkbfds.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yoicyszq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qoqxtyhf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3xiuujywe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gxxdraji.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3hdtbdoxb.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3tmquedqk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3kxqxvyju.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3sxlrfyjr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nlzbgsrt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kzdnokhm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3feqvkecq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3pyofpejq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3zqwsaimv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gwzkxxqt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dxzgcncj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3bnbhhgdi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qazfeagi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3stvcgiob.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vyxdyazt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3pnnnfoas.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kamhdwup.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3sknzceiz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bflkibfz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3iqxrtczu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3maolwpvc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rrxmheug.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3orsheqkw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3mgloblpx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3jiwikmoc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3tsziihgn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3izndikdm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lgwmockf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvaatpic.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xjhjmace.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdtikgsx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3nbhfgnhc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pdcydvzv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3gglpygbv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3inasvdeb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hvxjbdpd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bjpwfdzs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3bteenwqd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3aatbyyit.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ahofyeyi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3wnzznqhw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qrmgjnch.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3zbbhxyjt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nanemqtq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gsjuejny.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dytqvjqa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3fzkkcefl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3sdgfsrbw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ksrnxaey.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3brxfffvm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3tuczqlxm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3huafqaow.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ikfcqteu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hvqujsig.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhktauab.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3iguzgpix.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3qsqggtjt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qhrngmtt.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dgkgwdbu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vjnfshjq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wtbdwuks.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3huutccmt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3odjpcild.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbufkrgk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ooblzoba.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hogzjbhy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3feqfvlxv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3oyzgpguz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3hwrsgflo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3zraxzuet.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lpwqpezy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sffwmpmx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckkqwacl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3hpzdnpzt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3wqtiqdeb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewgpaboi.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hhvdczvo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3sqguzfsj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvncgdwz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3oyfpcvwl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpjnadtv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfiycasw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zqddjenf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3atawjfdo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3foitbemi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3llmqaekn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tnsnrikg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wubsjafu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cguyswgk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvsxzcuk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wgifuvda.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ucdrmrfb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3dyhsrhpw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqepwmri.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3amlhuesh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rqudmxir.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ftxgtkbj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vapaceqq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ilpbethd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kxovynpo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lgtmoybr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3mjfutcvd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mnezqdkt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3xaqpepei.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3pepheumm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wyzyuagb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3utcsumva.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yevxrkrb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mljuwrql.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3grhsyfml.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3uubwkhah.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lehsmwdu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vyjlgaqy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3azadycsu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ahxpimog.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nvenlhll.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mmkddjyv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmklzpan.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tbnfavxf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nmokhung.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3sibspddm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3lddvwkpg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3klwzsfyy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tiqutmtr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jwbysnvw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jcgraeqx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3eksxizum.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3wvtopchk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wxozgqzz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3iwqdfupj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ipnjgojl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3cjnktttf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3gusnkapc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dfaarqve.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xvcrghhj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zdfyibyk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ukfxsjhd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zzbvemnt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3zrikalyd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3njysaqle.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3rfukfvtl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3koedirxf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xhavfowh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ujqedvoi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qyqllbtu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wfonsrht.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3nesmwlei.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3nexmfvui.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pbjbwwme.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jythxpxy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3uhzfgrdx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cxqkksfx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aigpwqza.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3siwvgdqa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3caenhpoz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dacgslnw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3awbhohmz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3uzrzqtxe.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3detqbaen.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3yavhfqfv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3razwyfhm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ucvijzxm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ebuemldl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kpqclduc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qfhwquuq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sbeliunm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3qvyiivrd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3afcvakzd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3bobjeqyj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vkspmiez.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jhlksjpd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tujqqebx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3emkxghnz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3dyyedlpt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cqzdrcli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtirffvg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3icljwetj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekeszdox.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dlvbugti.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hdhfztgn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mxodyvhg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hllicuzf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lapsikmr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzbnmjka.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vyqokvsp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3tulotwwn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zpuwsmrg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3erovlnsj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3vlfjlosn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3itkgqkgf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oiubblug.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bwbjoeqd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ukzhmqfu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mamgxrin.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hflpbfvu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qibrlrpi.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3bozxiupk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3atheqfcg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3yltjrpdc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3utdxdqbe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvvmkpwo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3nyejlfzs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3umynemkm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3jlwbifiy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3cimpdhgq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3brszyvgq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3okhiccpe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ippmeuje.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hplqhqob.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ydbteiri.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3jqexhzvm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3infcumee.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ofmmfyak.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nrbmanty.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3drqhkvtt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vdkkshqt.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pubwntpj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3glwqvxqh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hcihrawo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ystximpj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gsbmagre.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rzylawxv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ifelnagw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kvwulqph.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3gtafobnr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3tobrqtqj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ubxxdyjl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xlnnidga.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yblbvwau.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3kagactbp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3llaertvs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3stnqmupo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ilyhibfw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hczlhnxz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tjvvxrsx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3bjngqwen.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3pmkjhehz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3abetgbki.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3xsqipcae.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3mhrbhzhx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3purfypjs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wzlttxlm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ecbwcrlv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3yxpihztq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hexdrnib.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3alwjnguq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3jrgeymsp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ftxdolfn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3dehmubri.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjqxhlxi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xwraryir.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zkcibxts.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rbkzuokm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iadsveeu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xthunjbv.html


<!-- 参考信息 -->