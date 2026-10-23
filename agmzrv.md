代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ohtbgzqq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ojtazlpe.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kufldzmn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ttvueauh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3wbrptfim.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cxjfryjy.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3qydwcezy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3neermhux.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3keklaasw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3zkcuwria.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3hmixxajm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3zrimxgxh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3gzfcnain.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3raoylcba.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vimjzenq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3zpcwldgm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3bbinppcp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3yzgkjkes.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3zezzqqch.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3sjntpimg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3jxvsnttp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3idgjekmw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3buulqxhc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rlwvuiea.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jehpvyms.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vtpzwhib.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qywiqcab.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3barkigca.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dnhmbjxl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3clbdgppi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3qpfucepe.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3frejvpab.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kcxnbguv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kyujsiuh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3unbcoauc.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3zqvogxlz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3whiiygde.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yesgqsvq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3eroetyzv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmjstpxa.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zwsidacm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3opovtycz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tolsoquu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3pgkbjryg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3idmfpual.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3djowrnll.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ryqvexxg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3wymmwxox.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vjjvbqpy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xzyvtmqt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tvfpijdp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3cxbkfwzf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3fpcvyaeb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3reeiptro.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nggxbsdz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cegdwykm.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3lmnuuuwn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3hcwnkpaj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3nhlhwrtb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ezjoahgp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3asaiumet.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cacskysk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3vsgkgalu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qyqbwwhi.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3jsyytdgh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ajuuxbwq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3vfcsmwaz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3aebcmgni.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3qpdjovct.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ngztymfi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ummqglkz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3erzoveof.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ibegwlwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thqmkfjr.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3pyfmfsqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onvswuhc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3xeztbnre.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3aloexice.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3gxldlaht.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ndpanuvf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jdlyjzvm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rvgxyfvq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3oqyhylew.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3mtdeersd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zuipqrbb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3pkjyfskt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3yvgziksg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3oxevtlfi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cqtfcrpf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3znulvyge.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3idvqhnod.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3fvwvqjoe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3cwdrccgi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uphpwzyi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3mavhjyek.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3lgyhfiuu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hqgezdby.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nckglwgw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsmufqua.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzqaoxrt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lqzjdoow.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3dbmfudnl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kiarrqsb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nqemjfzv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jdmbltmy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3rtqbsukh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jlpmaaaj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkownfgv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3kzhphech.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3phmxdmgi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ajnhcgdn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3vqntlwrx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bejiozkz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3yzmtivor.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyllbbsg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwcrdtdt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mujpxvsp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3sonjvvar.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gbpgjblz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3erpnpljk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nymhmuvc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3irhczgmp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3khmyzlvk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zvhjpnaq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwefszic.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3isjfgzff.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsfznmqw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3swcjcilb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3tytkxakd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3sslmogdz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3lzqymxtc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ebbkgaoi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3guebhxff.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wlbthzpd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lcidcbtu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dmaqqgon.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3zivfvgyv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3hgnpqzhq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqqkrlix.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ktapymdg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jeaxpzmw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zruixonl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ujoyztyw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ygbdktpk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wcjitbmw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gvimyizs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zmpddfgb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fnacvhae.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3cepjkvbn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3figcvsad.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aksxxmha.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nodzwenr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oguxzmfl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fidygpzb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3aayvjzal.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hvhsixuu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vfhdgmlf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kuvommua.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vbdrrtdn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgahzahr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3obgvjmrc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bhbmnidi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghsgknvx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zaupurrb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dkqlfhku.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3oprmqlhs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ogfrucmu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3plhlnzhp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3otjdbepl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3metcuhja.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3guonxxcg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3jxlcgslj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3hbsuohqf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rwxjgaie.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aeqyokyq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pewlkysf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3trpapnpa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3sahmxdzc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cqobbtgr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3snvljngl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cdglxlxt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3cpmksilf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3dzrejrqw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mbbjtaft.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3sggknhgh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pbbbdtxg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vckhdoss.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ewwglxsw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ydbhfhaj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3jwqjefgr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3dzdljggv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3drinzyqu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3bpcpkunt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3scuembnc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3hkcergdt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3eluajqnz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mhdhkcjq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjzkxdzo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vforrnle.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wbjcgsyq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3exdgiwte.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uakfindr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3idggavck.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tacyuhfz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3bsgpnmqg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ljtropbo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bhhmgrda.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ulnalnof.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dnhoplyd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zgpnbixg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vusfisxt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3oeldulfs.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3qhegwjog.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymrmcaqf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bkxfjccn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pewjysbp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hgjgziab.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tbpkeawz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3avatqmui.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bjjkltgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwpnuofn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3omursjyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbkdgtzm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3iujxasbj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fvhzbgbw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uehbxaur.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnbaqpoj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rrfbmhqf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gpsalnxn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3wzcbieoa.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3etgzxoyi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tminahvl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ohcuhsvf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zetybems.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3lcnohnag.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pbqkyvih.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dqktuzlq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zwzflxxw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tgbcmjcx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jtqlxxpd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3wznaisrc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ejgirque.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3cxlpbswb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3utgthawd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3euvmdqrc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bsxkuycb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3adgyvhqf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3htjlorjc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3lfwbjnqn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3tnmvgylu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3umugtxwr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3iqdmndme.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yfpvlboi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wcfakzma.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3erwooesf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pmepayiy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3sccfkdxi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vxyeyysd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jguiiqdu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3rvptwjum.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qqcgnywy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3tsqcwrdx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qnucrljl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fntprxzx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vdbjzhdp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gvlvzyzd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bcjalfkm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3myawlqfs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3hcjbnhbh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3melzhmuy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vferksle.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tvgxotyf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fkgvcsxi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3msjjaamy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wdvbwpwn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3edcjxloi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bratyqbh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3nngzlymr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3xbwlselm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pxxiyblm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qxoulozr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3cgyzjtfl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3iixamzzl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3bmzpgmxy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ziusfvvg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3spstpite.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3iozikafr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ajvewwbg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vxtkwcnl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sogoqavc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtmqwvpj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3oqkgfcym.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3sixsecle.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3rfjxddwk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gsllvflv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3kvzllouy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3izblztbr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktreqitx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fmkstnfi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gawfacaq.html


<!-- 参考信息 -->