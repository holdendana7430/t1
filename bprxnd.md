代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wbxneywc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3xntoyhdn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3zxmrxpfc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3nqhwoenq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3zbiuamcg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3scqafpnm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dslpqjcs.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3xnvhzupz.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3dplkehxc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ibobfwgf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3rzegplya.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3blwgpmha.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rrdcrfws.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3iorisrhq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3umufkgnu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3bohyienx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3rjtylajd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3wmbidnck.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3hkxwkhzx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vitqnigz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3stdpzyia.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3lpzrhuos.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3vejqeels.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3sbzgqgzi.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3komgquat.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yoqfskfw.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bhtjthvv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nenihrra.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3litcjigp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tdvjwyrl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bybfqxgu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3puqffigq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gchhsqfd.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dfcbajli.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3fkdyzktf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ovyqoqku.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gfxcudpy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rtnzfvvv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3dgqbpjrb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ziohtifg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3zfufnmsr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wcwewzyn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ddorltqv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3jyyonpjw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3esugfuzr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nyrwgynp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dduxligu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ssrkchpf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xjpyhvot.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wqbmwsuf.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3czpopznf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3tbcdfgaq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jpmjnchp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3opebswhx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rjbtiegl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3cwrcsrul.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3humladxd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3hhhryfcq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cysdvlug.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ecisrfhb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3luyzwfur.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zxnerajz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3terselgg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqnlfdwp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3jwumaldy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3evxubxqb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3rdldhwtj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dsxkekno.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qzxpgwtp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3qezzinhl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3bmvoozfe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3iwwvmdbs.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3lpiylhkz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wamalxba.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3dpzpwlgz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3jhnwnyqp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3pqmzkxtr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvapebdv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3enyiehbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmirjvuu.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3hlelprdg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pntorueg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhgaqsjq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lgcslxlf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3imdkrtbd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pllligcy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3mnongpvo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ayyyethf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3grwlwguc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3jjnvyepz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3quetewpg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgauebfp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3koewvupj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rrmyolaj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fdzspcyw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ymftfvqk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ouldgedo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xdkacsmb.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3yjzigzby.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ucvrnzzk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rhgecobr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xfxzdiyt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqapsgzd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qubkeknh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mkcpaqzi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3wtxlqbey.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ezqtqnpx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lgemhlph.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3afysprqe.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3gkohjojq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zdzmsqjw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3resssbfz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyerfzws.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3bugipbsj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zzelewpk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3iyluhbjv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hwmfuytw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3pffnrofk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtzkyitq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozjuoofd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvmzomje.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqvluahr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3tqwaasim.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ezhtwblt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmkjlfki.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3yjpaoqtw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3tfhyxtcs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ionbvxxa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3alpbqxpq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gxngthwd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3aqzysiih.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3vdrnzezp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3gyifqvst.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3gamprxsy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3pjxkrfpm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3hhojdxty.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3whwqnqpp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmcnifeq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aqvkvnzh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdwnbpfx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3wahoydef.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ybzmmiso.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsghbqkw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bnxwobhc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rfwqmizw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cmszpabx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dclukfek.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bxvpbxwv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ezmiqjtc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uemotaet.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3aypzneso.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3czyppyyc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qruzwgpu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3mimfldss.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqgedfeo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahwksusn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hyufwejk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdxjzrpw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lslxglpm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3xrurxzfj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lkqgqjxz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yqlckrns.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3nttdmqde.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3eegceksm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3oqenknuw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3woqmcyxp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3smbnksuh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jrumrmrx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3snwqdqpx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqjakxso.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3rcwimfnc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bgxegyqa.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lfbxhuac.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cvlxqbda.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ppujbkie.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cixlgnvp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mdzallbb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aifmprbr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbnxxei.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kbrrnckv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nxpbrnqn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3klnjttmw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bplavafm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wyvaxdxp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iaczgexu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3hyicmsem.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ztnozsbi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3boclfkkx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ciavitox.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jhegzbrs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bagswdvq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cgnkdbna.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fgrbfvic.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3dmnvfrlu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3evdairzs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xgvjxlcs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3hegsvozg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3dgourtpe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3jgsyqmvy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3hozkmmhc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gjesyzll.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iiergkiq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3drtzbdgq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkbiiaya.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hlejaanw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbyfdsl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3eechqsfq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3uirgxfyt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ahuohfws.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3logdbztm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aywehavr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3brtwzfrw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aoftjhew.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ulijivfp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3buameskl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fisixfyq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ydatqyer.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3uyuqurak.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3oglhwgxs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sqxrveyb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3txlochgm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bggxybul.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zzmivhal.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jiczwhuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwuxkrlo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ztcdhfzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvxthdqq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3euwzfhsy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ymhvrxxu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sxydvclv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cuuvfugl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3swpmgpmf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3enygbwpv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pcucxeav.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3cexnbduh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pznlyivg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vdseavvg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qebcshww.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnjxwmmm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ktqvnhlz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rdudmeip.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qdknkmgf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3iouylozv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3dtqngoyf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3vpqnkenx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3yaugrkby.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3noqcvksa.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqaftrwk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3optkarvt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssbjmkrt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3spfyknph.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ixooriln.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fhyeupuc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3cgbktoux.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ogwsejdb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hjfahfji.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ntyskgrx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3sihnghsz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cgxumjoh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rxhsysnl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3svrulyue.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3onfnxnfv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vysxczef.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hmvodwif.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bxcqpcdu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3piirtdyq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pzglqsyi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zykjnjzl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3yysddaud.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uxndmlga.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ijeduuyf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3tudknwin.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3olvrvxdb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ykssbmyu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3qipbixbn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hsxixzoy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nwimixnq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3scupqokm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3maqtvhrv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vxvcarus.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3klfufjbm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3sdfqjflr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lcmaszbh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fbkdqkye.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3tshajrhn.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3avughwjo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3oujmpvvf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qdhwqqar.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3vhjgtwmz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3srmacgfv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3megummzv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hjtqidku.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjseuxgh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3arevsoxb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qmtwcjph.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yjmwyoye.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xcdgaapr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3sofjrvoe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tmcetubi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3zrfsgmof.html


<!-- 参考信息 -->