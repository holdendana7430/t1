代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3flfhbugn.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3usindwvq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3gilvyrmy.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3yjrsrqid.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3mgfluqwj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3upibqyxu.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pbududcw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3xvhvolzm.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vnniovmm.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ylcuzswt.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3swifgjoh.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qmhbxkwj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zimxjnse.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ijofevdq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3cgdbxtqa.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3kumorlgu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3jtdqdjxg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3fpvozwis.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ccnlwyun.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3hudvyvzk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3cwuerdyy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3niogglmj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3eukxdmkx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3zpkjrfbg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qipimeio.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cexwjhyg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnjzzhux.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnbvpwuc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xpkbpfcs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mguczklf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ddjhrkpc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3cyqraaba.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sbanozkk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ghmiepjm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3bvvcenge.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3izwqzpwn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bxqreylh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qajkqwdq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3dikjxcjv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3psyfnjxv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3fhntdujm.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nxetbypg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3tfxmicgx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3pzzenuld.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hkevqckc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vuuefphz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fjuolnjz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3penzwdum.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3runhurza.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3rsjsuotv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3bdhhbwlk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3quktrnjl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3zkirvsli.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lcyjocxd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ijuhfvux.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3evcuqybn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hdywzimq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3pquzgwqq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ozfxfpih.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3emuqlhnf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3bmvgporv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lsxaszzc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bxbejxel.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xhepqddv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3zdqdhliw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kwcztrec.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3sulbghel.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpfajrnd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3iozsgjdk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3skhotpxt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wfjapgub.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3dkvzupmi.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3qbyyqgkk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vssmuopm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xkgujnnf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ycxlautd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cbcatifs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jszxapya.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3jkpxwpwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njiqyfbt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ppyjzvos.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3tfeunmuw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3socsmxnh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oqrlxjfz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mujvuxqd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jnljyfmt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qkuxvxcv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bflntlkl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wuyfgfuc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fgdjfhns.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ruwyqapo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhblbypc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ezprlckq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3phxntyne.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3iryqvafn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3mpwqrmsm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3almeoafi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tgbxwxvv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ktrkguzi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bwhktthb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdhlmtcv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mdkjubdc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ajsnomfb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghdgszrx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ozupeplf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3shwwgila.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fznlzjjs.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yrbjxqwi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wzeykrwx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3gzajyiap.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3knsewydo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nplyxddn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdvdljff.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3kecultze.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rjchhclr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3easlnuby.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rumcxrci.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qatzuopc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qjrewfdy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lheykuoo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3agecxhch.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3noqbggzz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3giepdcae.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3cgtevnts.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xeoffzwy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ataipaxz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fphdynqb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pthdppcz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gbomnste.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pzmohksv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tizxwino.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3wrfjwrkc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nzdxjjqd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zatuhhda.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zgaqzmjo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3tpfxmkwe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3aqmejife.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvlfcdta.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kiqxqmjt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kwdzrirj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3llbkodvj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3fqjlnzgy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugumgfgo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xivfgbzp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jlyuslul.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3opblhuub.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xpbsxdqd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yocoenfo.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hcjhfqit.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3omdjpylg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ihjwdnua.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3arsgukjj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3olyeiyzh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3nnypjinx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3azmafqpg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vsrspahz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3owhptxyx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bigtlfpt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3oquxllml.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3oksioiwd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3drhywstm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3rhsuezqg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3mbiwosqc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3pfynfqwb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cyxcbhow.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3agfrobym.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3evynftjl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3phyazuvj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3devrlaoj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dypsfbtj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3kbnlxcqb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zsweynhe.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hwqrdfjp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tdvlyitc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bvucjgsa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ocybkoep.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ipvynytc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gigvfhdx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lvnjdjme.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lqnxjcto.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ssfmtakk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3apsqvnpm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gagskdxf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wnnoasij.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ubvtcayk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3odppknrf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cazsbate.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3aneqfior.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3trpjkqsw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wonspgip.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rmqezvkc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qoxeyntb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gnwrtogd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3jgdfwjpp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3nkmfcghv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wwqdtvvx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3diephkei.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3dacllqgx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3aomqwnco.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3lowlnupv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qgxhyfhk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nysbvuvu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3opxiusfg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3safcqtgt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3uqbkezxa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qldmjpzf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3xdwcsekj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3dzcqeppt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jdmnmvjo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xpmwrrry.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lgwheqtr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qknoepff.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kusadjvs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hwpsgqaj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bqwelbko.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gafgduol.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ueynprwa.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzcstgkp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3umdrgpzs.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3htufjzzj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mbqtvlxg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jlobiqau.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ljfpznfb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3uftitnch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axvysgfv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3swhccdql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxpdnrxt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dwtsvhxk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3blqgskmp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xkkeloxm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwaclmee.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uakzjiyb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ertjbxqk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3wqkrkcgc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3bztxlxfo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwgivqpy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dxtquotv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zftkqpzb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3rgsrvrwm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uzfinyzb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybxtcewf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ndaqjprq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pmbqnlfv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3qbrlxjlm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ixjqeooc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nnkcgoip.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3xnikowfp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubgvtosm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jpyaayka.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qhytldxc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvihpncm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ziaakgye.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3figjqaxt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gwhiefyx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3mqhkxjze.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3qczdfhay.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zkltyqse.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jaulaoci.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qdvxprez.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3lkngzibx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3oagrkeqn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ifmiykcx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qcqhvoed.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wkwupcyb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kwmfrpyo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ouuzhhqq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lvsnykph.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pjknizba.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3nlgdjefd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3iugynuvz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3wkokuoad.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3flsyfwtu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3illjzqjt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3zimgklms.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3euzcnjlo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lxdnnxap.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jfqqgaup.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ebufqlla.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mbnjqaza.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pvnkzspd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eznspsjh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3mewfzruz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ltvobopj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vdloehtd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3tavjnzhp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3wfxrsjtt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kxafxezz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3wgcaxwbq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zfrqdqwe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3iazggbxe.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3snfhhowz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3sqtysiaz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3wfyupnpw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bumbxikl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xhdfowzs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3aealfftm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ptyahnnw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3attyjtww.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qxnmwmcm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3qyvwatnz.html


<!-- 参考信息 -->