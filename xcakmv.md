代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3caxbvhlz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3dwjtrmpo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3tzfdxfyp.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3bgizuqav.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3cqsoofrr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3psqxiapn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hommdxnr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3npqhptha.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rfjgvmcp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3utoinnba.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3cauquahn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lykixnee.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ahositkf.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3lsfudoqq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3tdoprfgw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ztzpyxii.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3zfmifwpa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3xgloxvxd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3zksblyps.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3jtfimqfk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3nzwasqqc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3gerpchej.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3sovlziuc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3uemjdgnn.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3jpfkgppv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xjacesfj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zfksacgw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oblhsitd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nsmzqnaq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zipzfnno.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wfttcuhb.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3esymhzqo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fwudoxmw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kannghbw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3edezbsii.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3goqpfshc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mynkwdnk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3acceqofl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yhibghms.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3tjijjxjn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rorpbczt.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3obffyuqg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ahywketi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3grcytsrl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dxjacaha.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3aojxembm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3pthyovir.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3mxqidpzo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3khkpujrp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3zdwefupt.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3zbcfnxac.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3zblvebxc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3uhsuherg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uwulread.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pjyanhgc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3khrxmnyv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qjudhgtl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3kcprlghm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bgahjngt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3toeveebc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3yqmqzpzd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3batwcozl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xcvfrgxc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hgmoxjtp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uaonjffx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3isbtlpuq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3cpndyubr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lrcpsrhh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3dnytwuqd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3vcqvhdfm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3exlmbqmm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3pqldqzyk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3mcgtfgfh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bgbnejqp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3utacablb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sxphksak.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3codbacdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcuymdad.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3bwfeqcqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxjogcrp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3sunkrfpr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qjtxbbvj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ogiurfnc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zgaujjxm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ezqohbdb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pmlogdzs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3kvlcsevh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3vghdcows.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ygqrpste.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3hexvkrjj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3zdztjnaj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxigkdpj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mtavalse.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kkhfhetx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yijuqdds.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3mbzxsqsm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3kwczfrvc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nvfgmbmd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3tfabkrbd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dxppusrp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwabikxf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdyopiwk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cawyboez.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dgoycsbq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wurcrhza.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3qjoxlhzc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dtesfrfl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3bnjzsbqi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xplbdurc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wpysjypp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3axlzinhb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyyzexou.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiztrvij.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3zaswabmw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3servemft.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndnsgexh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iovpljip.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3khnewuga.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3utffrogf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tghmtffm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3crbotnxe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3iepzxkbf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3srphxzxv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3vszzuhez.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3mngnnryg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jibsrhis.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3barqcmoo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktwwfphy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnwxsnkk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdblmohf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3msvnqzwh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3sktcanqv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rdqbqypi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmkcckqh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3tfmmloba.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dhtsfxwl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucafrwhq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tphgqjjd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ebuzqwcw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lsudhhqi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3tkxsanjj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3nxjuaweu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mnlqjmag.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vwjzqvuh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3yuvdjylh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3owtugwfb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vytcabim.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rdoauivs.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pvsvzngl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dggtocwv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rstmxqmo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3itcrbddg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3jnfejefg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3cqzisogb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hrwzumus.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbfoolde.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qckphchv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsqgszzf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xkvhggvb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3dpjibduz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nupvelne.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3czmgxwhg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dxlwxxri.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ctfsknwi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dzubfnus.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3sekdqakw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ihnfpkxs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gpuoykei.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3voajqttd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jqpfiwqv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3auounnun.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3mvrahvya.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gylcrcdu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3deceetab.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ylpwtwam.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3sjoilvao.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3tlfulciw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dxpysyez.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jskzxuny.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3vohgzqei.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3tpilwqut.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ujoroqym.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3clnipxaw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jjikvlhw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lrpsrjxr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tgwrumby.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3tcjuniut.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3zrgpzjez.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3zgadfiwv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3dtjdcnth.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3olonlafd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xvamlrjr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwxqiqxi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ifmgcdkx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wnchzhxf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3stmokzei.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ithhoucj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3pygtgjoy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bjmkfzqx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3qtdjbbmk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3binhnogx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ilxtrwea.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3agbwswey.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ybwaoyof.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tgyeluhq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nsmnqxfv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3bcgnwwhd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3slbcwalo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3eiiovvqz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3byiibzqc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xmgdinvu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3urdphkln.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jbponuxd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uopcsuqt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3segpiqya.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3etpefmpa.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3fcqtngmv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3odetwsql.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pvhdeauy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nnwpqqtu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ugojeyyn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ocqyibdd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mbmmwnjr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3inigblej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epgfkvwd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3sxfnbxnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttdilpmk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xxbnwsfy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zzikwjac.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jcrpfbxv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3butbfznx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3adjdwgwk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hpoghvof.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fzdmqayk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ztkzvohp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3axcmsqhv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vtagehid.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wwkcqnyk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcjfntat.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwupdoki.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3saudaaop.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3rlluqxgl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pifngrsf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kpjwszyt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ovwgqypf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3zgiptqsg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3guwqtenm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3eieujphd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fvjvlvcp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbpxzsly.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iklfrowz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3vpuetgnj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3evshfgfw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3vndxdtgh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rmuceneu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3voijtggd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vwpuprww.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3utvfnjre.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3suewkiik.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3frmoefsa.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fqlghllv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3teeqdsug.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vsagcwlw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3auxjaxlr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3iqeqmjwd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nkekaxre.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lcbnywve.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dwdoobqw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3gynswaxz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rjuyrbug.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qwcgzgqd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3mhugbmfi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ubuelhvc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3feravzxo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3emcceeps.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gtfddnqp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pihojnpu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fgwdanxz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3onrfkrdq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kefqycmb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3prjxpqqb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ducsegoq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3fvnhsthy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zyejbghe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rxjbfgzo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hnjwxmvk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ervqmcqd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3nyntwgxq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tkouwlju.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3tmfmgbpm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3mvipmtrm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zowbfcto.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3udlmjzcq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zreuaisx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gepiuyzm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3nmwhtzrx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3myrfljmj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3yqusuopx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ltutfvol.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ligaieit.html


<!-- 参考信息 -->