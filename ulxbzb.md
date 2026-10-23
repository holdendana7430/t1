代发 wailian999

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3syzznnbh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3mfhxaetw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3flmlsbcu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3wzfbymxx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3eicejpdu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3tflpyfts.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3lzhmtteu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ntchqdjg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3siiwjuju.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3czodkpvz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3hhjzbpum.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ejjffwpk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3pchaqpus.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nrnbglwy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sywmldtp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sfmtuiaj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kqstsotb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cbxewxqp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bwkhspso.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3hmcbhkvx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pmemxbef.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3twmdpanq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ttavmbsa.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ziynkgzo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gdxupzip.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3zdsvutqm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3zenhezky.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3rmgxuvem.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fupjbfyo.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3iuelnopn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ujyxbssh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ltylojqx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ietngvtu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3aubiawfv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gtpixglx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lqfhirtc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yycsqjrn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ukzckthz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3lvhbivwx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3uptvlzsq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywsobwnq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qkjnihms.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3opvcwtln.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ksfwuwcx.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3wbmbnubt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3libnulpm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mkemopjc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3akwdvkum.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xlvikfwi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3dkgurmak.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vglyxyao.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ckzdxqfa.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ayadpwfq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3casktdys.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3veaikezw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ylsupaxc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3lhycglid.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3snkthvvj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3zdsvpjod.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ddzfgsyh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ixgdhjns.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3guuufyhu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3yyzlwuff.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3blekrdbc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hefxsqlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjaxoyff.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3eyrixylf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugbmujwa.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3cudcgygc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vnjyoonc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3gweanptk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xmseusqv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fgktkiby.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vfrfqdcb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3scdftmid.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3qrgjzodl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ylnfnfor.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xubwwhxq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3znoegwjg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3bfznkxlx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dsuwesnj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rcpengza.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cbochsxd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3oyvtzcjl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3hmcpfmki.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wsqhvpsb.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3donixwga.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3yhwdqthp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vulsiqnt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qraocwdt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwonrhrl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3brurkqql.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3conkgbud.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3gimlmzpz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hadnfejy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kclpbrtc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qmoiwoyc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3fidrhazi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzazarme.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mcdstukh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ctaxojeh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3nitwcgmw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ddcsmmus.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hibdanrb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fdfezreg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3pbplipll.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ocaeyfjk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfexzfqf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vttqfbwp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmyfdxxj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ddwyulfq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lclrmocn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbymcucw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zaxvxxje.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3pouubvvc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3urmdizsk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xaezhhhu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3oilwlcqg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjcwaaed.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3treridjg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3syvhxeib.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3njspshvg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3snmxlzpl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3zohuwlbp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwnupuka.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tgwxbogm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zknjdsin.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eazmbgjv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3exmwpxnr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3swygnmwo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3glphfglt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fuamlcjd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xjwckxui.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mpjzhpgf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vjnbnerv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3drkbnvzc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pvljfawq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wedliytr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3hckaqkfu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zcoktbem.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3xtngydcx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3hpswqrvx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ujwdwiyu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3igqmokow.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkqaymdw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zfstxsml.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ztmytwkl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3vilrlsry.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwobnckc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3izliysgw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ibpyhevy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ywahnmmp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kjlsppyf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3launlnsm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqmjxwal.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3kmfqumga.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xxjvphch.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjjwwpxe.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3eqohtmtg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3grfrnwks.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3orkvvwkh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nicwmjzv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zqvjzwil.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3awrzklpw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3gjzwxify.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ydspwxpv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ssfsjloi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3owbocifn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3zpysrpzf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3yozgdmpf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3auvafrxy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lpygumol.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jhrefecq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3nxdfmmod.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3uqdsfxei.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3fzqvkjij.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3dzkkbpqd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3bpflxrdq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lhoaatdl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhtgeeia.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hersplkt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ailxuyqd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ekgedwzv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wxqhvwiy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mkzkjndo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pucfbtyd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3rjafnthf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zpevayar.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yiinlicf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3svxxufqa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykydqxsk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pbwxoouh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xzwpckrx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ckmtpqpd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gzeznwim.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ybnbkozo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3vjzffenw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kkhybwnr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wrfmbavh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zgxviqbd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qbvjctwy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3smcrmsbn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wkwyotyr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3segzeeqx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fvbzznif.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkodjukv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dujtbdbg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3iblzdaml.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dvvfitzh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bscsbzco.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3znevrbtb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3axmxpwrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zicvhkuj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wzfidzjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idbjgvev.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3knkbwwha.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3luhbmzgs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ylwwqdol.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3juiqggyx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eifwjhny.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkltltjl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3bfonztei.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3iglubgtq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ghxdjqdv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3xibfhtjh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3pyamltsp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzwvzvnr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lyqihoyc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zxvtmhqg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gikqxzbu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3rkcrhatx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hhnrzyxa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ukwtmtvm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3uupshqze.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wbiggizq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3uyxkblri.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zuvzoogx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ehdnzmaq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkviylei.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3npzypubt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3avmbcamz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tvzkaizh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3prefaeta.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3dleaxeev.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hpaneohi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3exqtjzgk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nhkksjmc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3iksfvijs.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ijgyxger.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3csceopgt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zezppsbl.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3kfhiokqb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gatngzrd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3caocvlse.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ztbvyiat.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3txrqfgie.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3itcbcvsa.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xuyzarfq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3uwbglrmc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ficjbpee.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jruyuwme.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ntazufmd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3gxxekfqf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sdoqljyo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ekyoksid.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3athjozkg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fsvvsqlk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qtnscqkw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xgnsiyez.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3zqdsabik.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3htlsowne.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3aafcpbyq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3dsandtai.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3cannmdhk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3adrixsvt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3tqsuybfm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3zjgvlgfa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3enkrwsgn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qplombmd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3cytseotf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzmhjkhb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqqcdckm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ezotbjbr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3sbwotuvw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3fbnixohf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pbzbesgx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fnkipbit.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xbzjzrwq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3tqujjhpx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sftbvqiq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kzcioofo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dwteaotb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zclhqzqk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3guvqdhvb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3oxhztxmf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3xyuzshav.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fdjitdik.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3zlkwlcqa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nxpbhhkg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3viyzbdft.html


<!-- 参考信息 -->