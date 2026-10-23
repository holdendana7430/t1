代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ztfixxnd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ujhqdkeh.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3acimznij.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bfxxwpdm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nkyizznw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3btroteof.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3rsdepftk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3vygxrzwc.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ixxtxbai.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3fzlpcozx.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wujpvpqu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ssdjssze.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rtggmmbt.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wijxzgfz.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3rtolflph.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bojolsug.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lkebwhxt.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3hgkipfxl.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3qpynimyx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3agggqwnt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3hiwcedci.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3fogokumt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3zbggjthd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ibptavhr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3aqlzqifu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3jjpgdecp.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3yroydqzp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3rxnebegm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ltvndakv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3slsywpes.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ppamabtw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oeplzcax.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iahgcbpc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rbaealms.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3njtghonz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3pfxwbpvp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zrutehxq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3znckprxh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3zaqktazv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3agdakzji.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ajyzhwey.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ybhngnfx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3iswlduug.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qnmzjszk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ybtyhbjr.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dhgcgtql.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3cpaorubr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3awukbldh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wldzpstc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hkjhepsd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yunluclp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3jjhnlfsf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lvwaqwgu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3pnlddvfv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3kusgckgs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3hzjtziiy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3zzusojtd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hxbznrcu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3aekrhild.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3fdkogqrc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntgchvlw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lzcuvzhx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3svwiunjw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qeprrwoa.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3azfgmvca.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3kxnjstcu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mjkjszjp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xlvmpdbo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3johebhvm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3duhwveds.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3hpjbzkbk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhqexfay.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3efhwdmba.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3uagerfxx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3fceixtcu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3obtxmxzh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3hgcftldp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3apoyxnwv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ccmecgdx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3zsrkgiai.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tadqzqij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yanbizfr.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3tizvvevx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzxssckg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gfanpeqv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3lyxzvszb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3rrmmxobu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bggcfsje.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3isjisxgu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3adwkgvex.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3vjhxupkn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3udforsrc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zkqkawry.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fagxxopt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3cvzgesvn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3cziwkeux.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vohvdfub.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3raiubdar.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dtntbcdj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ztfunxgs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3uiwkkfms.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ygwloxoa.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ewlfypcb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3vpdclpso.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylohhmbg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tflpdrhg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uiruhrnz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3guitfxxd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zjzwlivi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3xtbybvmw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hkuxklic.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xqsfeujt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqruggt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3overtngm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvqdpowi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hatakobn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3lrvmsatn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3igwzagyq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3dmbmpraj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3qwvkgovm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3opyrprdx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rbkzuwoe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yteosvbh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sypcbqsk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ijklxagq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3wdiemral.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3onfwjjkj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3pqnnilsu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3aulyxzrd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3iazsrbjd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ljywwuyi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jrnfddmb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pwzmbcxi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwudinha.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3uosttnhv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3trbfyonl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3slyrbrib.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zrljudbv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ymwdxvob.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3urmrhhnc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mchvzyho.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywuhwmgz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ycgqxiyz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvaqlpil.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wvuzhpkg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vczsfgaf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ncegdsoy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3hsrnxahk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3otjsgdpr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yekntjkw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3evptjfey.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3anryuurl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bnkvjnqc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ydutocqh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vcgpcymk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gizcyddw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wubnmwle.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xavzpfpo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dfizgtwo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ffrysydp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3doiqtzvr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cctsrhci.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dmmsjsoo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3daqneawt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tybfetwp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3jnwxpevq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3uoytzlbx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3sajeqmqf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ymmbuale.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3shwnjszz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3lkcxhitp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3resoyonl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3sevwgepi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pymwnukn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ifwzolty.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3czsjtjpp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jmsvnpqm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nbwvoumg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zwgwzzks.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3dubwwikg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jrdxrtpo.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ccaeyhcb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3oesewoox.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3hzrdhugs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3oxjfqhrb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ifxqfguz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hnjukrwy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ntvgrilq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zmpmwtrj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3egfajfhx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3mscoitps.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3kgfouehf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3usgnuyvg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3sgzrxcsx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hgtqsebt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hatuldcc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ytvnlryf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3knlxfjfy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3qpszihwy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3zejgnmts.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3qmiqrebt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3byejrnlo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3rjpdhvpn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3alpfsxbr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nukiixgz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xezykzgz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mfladbfz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jsqrusit.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3togfvvkl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ywlnckyn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3dghguqxn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3evljnplp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wqrmxdnx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ehkbfhyn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xmkbemgy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tznlifrw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jczzhksw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qwuuimwn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3glvmmhtb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ruocsyyr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3iqpzvxll.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3dovxlpoo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pqkdfuao.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cmmhxotu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jmxixuln.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ypcejdie.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3xhznqffy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3uywyjtqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcliwtgj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3prfkvhkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjvythvn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3luomxvjm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3auhsieko.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3atsevapv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbseqxbk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ychconoj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3usbdfhjc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bwaihkme.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3clbyzgev.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrcletpo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3lvliectw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3kkohkvxc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3muhtdhyi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwkyrhig.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hfgsjjst.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3iddzvhao.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3hjlwslgj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xxjytsqs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3cgrkeypn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mjspinok.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hhmxdzpb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ncpdwwwj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wtlpizva.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3eqigvebz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3llkblcxg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qgfhhmqr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3eyruwnwu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3cjbztpkl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3zrugtkdp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ysbznbct.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lldswkcl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tqfmevgw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3abrrpjxu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3fhtmpfhg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rejqqmai.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwnjkniu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mhutkfbo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mwqvyjgn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hobogyic.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ujbtgxyn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hbpgrryy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zdvjzuug.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zpbckqyv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gkaymnwb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qghouwtb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3mgecwqpn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lfprpaxn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ppnjyhan.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3uiqgebci.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hkhscbgf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3penbgmbz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3qzjdqezg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pahnwire.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3gtxtxvil.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zapynqca.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3pjizgrzu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3znvwuzau.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dokwebko.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3twzlsnlu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xpvmoheo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kcyfyloa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xazcjkzo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ukkzemkn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3zsuzjeeq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lbsfkayl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3yzbbiark.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghfpspni.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfttarno.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghbkcyvu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3jeacqzfo.html


<!-- 参考信息 -->