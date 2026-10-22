代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2vttubllr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2kglnpvyl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ruhmmjlh.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2inhedtch.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2eyghaxnl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2izpthrhf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fvdrkqqf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xdwucimw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2skdobjrm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zxpfzprb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lxusiqkn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2vqdyaesu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2omvzuejs.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zupnfjyj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2gttkfmpl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2aljjurlp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xincvitd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tdftpkzd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2spuidlgx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2cbhivylr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2auruphfh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hpiabvfx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2udbhtmcp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2yynpdcbw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ugyegndi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ozlqnbnv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wsskqcuh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2kgoraduo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2skjvdsdz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wdsfyvwz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2lfjrstxy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2djvtrkqx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2kuncuxzt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2acozrilo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kbjrwscu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2lsvfpmyb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqwfkpvt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ajzfrwgz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mirmefzi.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vhjyacfx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2koejgnvi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxjfattn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rvhmhqlb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2teqttwsz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cdlennpa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmriurtf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2cqbqtpet.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dnkxkxct.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2jlpovfio.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ikcvdcoa.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2fsvattbm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ooghomlu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2iyjbruig.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xmsedeae.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2hgydtofz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kbvtuhzt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qpcqsoqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpztfmok.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2apiqfbhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ondtacea.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2rvckqxat.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jswaxtnt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgnwsfyc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xsnvnggs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jknneslg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gcrzgaoe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2bdzmjzmx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mgkeyrri.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2attbpord.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2egqcurqv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2qermzxbt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kxempafi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sibhjpyl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2muptktju.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wjwcozob.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2wnrfdjuh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2twgzkxkk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uqbqnwvx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2duxzeomv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2dneczkug.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oynrjyia.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ubzsbiod.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlydlwei.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xbvaogzo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2aiczadgo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2wmakbrra.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sdvbzrba.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ouxrhjqa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2osojilck.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2prllheec.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2euiedwhm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dfgmqfnw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxeuknco.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2imcqelur.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ezunpfkx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnjdtywm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cywvszse.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ogvyfffs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dwecnqew.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkcxpxpd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnjhdkmh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2vkqfveoh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2psvsbzfi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2pcsqiofg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2yugpwwiw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qybizehl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2tnzswrmg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tamgskzb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bufvstam.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2poaabcum.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2uycfzhks.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2tjokkyqw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2phcubbas.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2naligzuo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2labonozf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ulyktxjv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qpqvlhpw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bydewvdl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2epdwmgnn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrwlnswf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2yhzjtont.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vyskbrsp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hjjslzjd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2gabimiho.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2sjphguqh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2btyhhzck.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nobudvob.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uuttopmg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xltsxwur.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xkybphzh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2pwcdthpm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2psewtksh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2dybkhjnc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2zyuiszzm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wngqkbtv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jizyxvzn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfxsejnl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ijltdklx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nfaddohm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qxrlcmet.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljnslfnu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2snlfztpd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zxnmoqvb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnrbhkwz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vntpxdkr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cuyqsztd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2qlazduzb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2zxjwvtdu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2oufxdvim.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2htkhljho.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rcazscpk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2oscjiihf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rzpizkhv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kaybgtrw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ptncfycu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ahhyczwv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zitcydfj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2evpkltds.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2viifuhre.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jofeqggc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2sqccglon.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2iophovfk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gljknenk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jntabccl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bxxnprwq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2advzjkky.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rufjijgo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dkdqxzcf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gownjiff.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qntyysbt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2aoesukzy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvtomofw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ublwhkbu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qmmdggxx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2xnycsuht.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2cshckwqn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2weizxzzz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2vemykwev.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zftuqnvs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2pluuuzsl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yuvbljnc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xxszucww.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cntpfraa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ilqahaad.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2crgflhhj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnxmbcak.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ipbhfpqg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2bjudelsb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2aspvzcht.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gerwrhxo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ajggyzmk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ojznyymc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jqcgvwcs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gscjdaws.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zczoyguh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fksyuups.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2fwwaqzfm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2grtbruan.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nlpbkrjl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2eejgvhpv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tdfreoiz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vzrqdhgf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2uisuvnye.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mbetkvgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqvbycgw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oaqfybgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlokhtkj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ctpxqvob.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2izylhcew.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qhbkfuah.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2evuytdyy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmnlyqjq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bexpmqly.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2apzuncll.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wbgvwbzc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbgvwebq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jtfgyeka.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ifgywgxp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rqhmkdba.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cpomvygy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqkjqbrb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2huagxhux.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2rwlszvsb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2cjddxveu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2meovfiqh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2slvqtipw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2syduszbg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2fxhsmeaa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikyraikj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wtysurvd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnwvraof.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2fkvgiciq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2vofgrkmd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2auicoeen.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tejwmwku.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2oapabyvi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2iedenuxj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfmkknjl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2prudlflw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2tfwwgkti.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2uiuhuruv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxmdvngf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vkifgrsc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ktqnjbrr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vowslmlr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2djvkkwbb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2maeixisz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bqgilrti.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2zdmrqoyv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2maznwdvk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2iudawebs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2cocdsxcj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2osqksdqo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2lfzghnli.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2aauvjxrb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wybewfdp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qpxkqvcv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jbnsfcea.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2aqplxlar.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sydockhj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ohgsrwwk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2wulegibk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2bjdwjvvx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dsnvzfne.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2njcyiuha.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2oiwlnomr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uwvrehet.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2zwpjzxtc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2uokaesbo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ehqzggxz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2cnthsjxc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2fpxppywo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2hqivjgnv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2poqckkvj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sshcdqyw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gmnwrxhz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2lsmuqjfo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2xbgkheqj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpgpqumy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2zcpezpem.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bapbrpzq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfvhjlea.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kefqzxhx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2skblzgjv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2krdxnmxo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2gdpsjcjs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fomtuthq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2itqptiwb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wnwhfvcv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2srbvcrwc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2nswtusbk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2izclymfi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2qobzzzph.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dddtvfjy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rjopgjin.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2twxvxlqb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uwodmsex.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2gwropelp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ywfzdflz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2gjahprvo.html


<!-- 参考信息 -->