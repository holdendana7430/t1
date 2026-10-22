代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2rlgiielr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2uemwjejs.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ryqgnpdn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2kemtvpik.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2wmhmhyvk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2befilbjq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ocvhlgbn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lvvvzixc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2greawklz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2nimdmzla.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ddlfdrhz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2agyuuizn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2czggmugs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2rdipsspw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2pwapjweu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2xehcoavx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2xwzhbblg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2gkadhpat.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2isvvlzpu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2wwfyhgvi.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2zmkxuupl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mxknlvdb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fyjjgvbk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2grbwiofe.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kihdpslc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zpgszuhd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tpaffhtl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2meboxczt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2doraitnu.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2hvuokkei.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2tpofhgfy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2hoanhdrz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ntkegcop.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gsjygaqk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2sndfdsnr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2xqselbob.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2iavbpwob.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jgdexqtb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2gyflgahr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2onpzqknu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2coqewuxt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2liahnufl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2joegipdo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2uqgjyzlg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2llutywbi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2iahypxnb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ucpwzlwv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2tozrkyim.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2wbaqwaib.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xnitrrkc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2emqrxcmk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2uvaezfga.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pzyvcpuc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2toctynjv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zhnixunb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wdjzvwmu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xcfzzbto.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2xixmcocz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2orshzxnj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2knsydevl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2sdhvkcfj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pkehptel.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vvwyiehf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aodcfwly.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2apgwmpzz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2elytkyzf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2nnanimmh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2vdlpdasv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2oexipeca.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2sbjjxiwo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2lctmznmf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bwljosac.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2nmmzuqio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blopemip.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2kzmshxzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frwtewls.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2eyhlyddv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2teiwfnfx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2egercypr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2eydxjygq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sxnfsihg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rdvbqvas.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2eismacai.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vmkmosec.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cuyqcryt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2muyeoziw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ptfruhpp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2zfdbqpck.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yxjzkdns.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ldggkspa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dxftgnot.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2kzmsocih.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vjgxzurb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lxntjzau.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2supznzvj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xtklotvd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nbdaijxz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2spqowjwu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnhuxjjv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuqyxxhw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wtkcycwq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fhhsblul.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wchyovix.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ppjjnxte.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2dvfaoyob.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2qydzzoyp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ctqfllfb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fvqjqkxo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2nkfqjpsj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2tkftefxz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jsjsgzso.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2wubvmkdc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tfqebhoc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hufraxbr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2erqugrjc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dccahqxl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcruzbok.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtxrljct.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kptdljee.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ejyjggri.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2yozvpjco.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2dejioltn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2mxjfqjzi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaguccrl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zykwyjpe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2uqdzfyrv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpikyohd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2uimqhiqg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2suddkfpz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbeitiyu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2mgutrtti.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dntmhvri.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2crmbeewa.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvtdisgz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvomubnh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqqvvkzv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2swkobhvc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2bjyfqbmp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytnytspe.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2qiszstip.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2obfcjlep.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zmvckgxw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yphwvdoi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zggrbhci.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rxbqdjms.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kqvhjnue.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vzpfdgoo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xwqdwfhw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2vrrkswmn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2dwhbqggb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ziylxmyv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2amgdnrpi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cggnobhe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uinwiilm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zupzuoxy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fomcfsfe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fytonczz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2eigsbxvk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2rjivogsy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2quhchtva.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dksfpjam.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pmewestc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2dviuxxry.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2rbnsnqjw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lyhbgdee.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtjfjtww.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2pfjfpcph.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wtjrncbb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rbcwxxuz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vuoxijun.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mrdhwedy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2aphmtyfh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2thzoehyh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pxweeqgq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2quywurtx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ffxvfsva.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2zzxqmhom.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2snvftghh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vvzyuqxo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2racgbhqk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vhkitfln.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ylwlwnnb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kaumwwtx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2gdfjuxfe.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2qvgnhbrh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2corozdtf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2bfncypeg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ezkiofvl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uuzmifyg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2aheofcje.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2hnhdvcle.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gzvrmrvj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2sapiqeyk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2phqfsbrz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rwbokrem.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mdnvyget.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vaxsicey.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2edyazhpo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gennydlh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pxyiuqcx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2voxcwlrm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zhfolvtm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ddkmysob.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2iapzepss.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2qzrojaia.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2akwzxvde.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lrhyvqsb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2twdowbzb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wwvcxcxo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ucphdiuf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oelrgbmb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xupellxb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2sqlpihcg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyiadwoq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lrpktzdg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2yuwhmmad.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2maqpohen.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2frahranh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2aqplxpag.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tunawfqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yagvcbgn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2dwxerbfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxuurvoh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2recrqnib.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mhfkeabf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2waucmhci.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wqrihagt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ismekjvv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2scuycmbw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lxgfjxrr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2kslzmyrz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2auxeamwi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2nqezmwqe.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2tatjpuya.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ptthnsir.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ufirlbjy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkzvuffs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2uvmoaeua.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2qvpupbgg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2kerpjaih.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2isboobpr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2shlehlot.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2jdbvplto.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2sperufbh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2enruzufo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2eefakvtf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrprpbpe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2euudpkkh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2yhyajtvl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xvzyycvc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2fkpzujjq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2svfspbhq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2dumdytra.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fxcjvgyo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qxdegxil.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rwtkhpsc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qidcdwzf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zkpbiuxn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2brxxkphw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ilvpoymn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qoyolfot.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2qxddncrq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cryxzdsz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rwuytkhk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ceqnydyg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ksrwwzce.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lrrriuxh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2hnemlbia.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2adcrshcb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pwpdueab.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xagvetyv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2noeiinju.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2znozyspb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zxiogmmj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xbczqkpx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ckojsvur.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yvyxdgzb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2cojycetz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2pipzkjmo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zmthyywr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ydrasetv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2rnugxrbw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2kawafuwk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2umusqmog.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2iwuemqrl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2dooewqvd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2czuwequt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2aluqaqds.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2pdiuznpk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrnpwsol.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uhayvykd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2aoczkxpz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2yqlklbfs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2docgxiij.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qhuyilah.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2rkrhyjcx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydzmduum.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2colilayn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cboaetsm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2eqgfdsrm.html


<!-- 参考信息 -->