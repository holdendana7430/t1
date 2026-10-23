代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3afbdoloh.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3xvclsdfd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3yxupuiyd.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lndjbqwn.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3wstlbhot.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3iqcfywgw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xxshhdah.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvpcbloi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3stcijvde.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kaozpewu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ezofuefj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3qleymjln.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qekmiqvx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3tcnphefa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rfgqhkjf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3kzszysdq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zgnfeqtp.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fmbwbqsl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3chugvfve.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3cfldmiqr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ekcrxncy.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bphieymj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3owlgbdrn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ssxozybl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pcddpzzm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gdzdxbmw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qbzegdmf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ycarvgww.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tzyreyds.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3pzxozsfp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3qevohzdq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ttatdpbi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3kfxzxyax.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3sfagktdw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jwpntesw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3lzmqmwnf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3fhtpxrvp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3nkqifqlo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cogvcpiq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bubpiezb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3yohklqru.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3hoiprugx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lftzspfs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pqxxbcwu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzqmisvt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3miqmkmyt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3bpdmjjfk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3cvmoyxib.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3iulzpnjm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3vwirourf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3pnhudjfh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3czbdkjtq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3jztwhejs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xddxcrun.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3iscjisen.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3mvjfvdhh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3quwrzetq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcdphqii.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ehacorqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fizjqmxt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jmcqmhrl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qwujrnxh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ogthfohi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lcsleicr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3brbhfkdc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nbshrypk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3lyjipvsr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ncdvtlsn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ifxtxjlq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3hbfuzhdb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3cibcjmxk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ninmurvc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gkusgcha.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zycjmyjo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mdaiwhda.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3hyveavoi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3fqulfemp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xqipsfax.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vofbecme.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3zoxovfbq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwrugcmz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3soyveula.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vhrxcvkl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3spobzcaj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hmlrmvqi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3aqdsvjzw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3meevpouk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lusgspkt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3urhsffrl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxmawmwu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3aaeaelpi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pfyteklq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkfvchqr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jceffwwj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cwfktdfw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwsqnktg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qgedoyko.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3hpgahoxo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3glbaeuxb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bljjdyzr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3iyelabzz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3tpaqoqqw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3hmrpfbpl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3yqwewevj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxbxebov.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ogknvvfd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wnvmajun.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3vtcoapad.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3goaltumq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxjmbyfu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjgkalhf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3kiawymwl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qzdpdafq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3gtdeqwqh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3lrhzhspm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3bebmindr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfmajnbl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3glbxiwyv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngtraxyg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tcbzlhfx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3iiwmrtao.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3hresajuf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3euvieucu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3feptfkfq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3arwcjykw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sqgrxdyg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gjnzfooj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nxjxkblz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3utbvcwcs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rvmlonht.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3cwhstswt.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kdqohzul.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3cjvqxwan.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ltdnvagm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3obtoixlk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3iewzkbgb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vtokxxdc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3izkcnaln.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wnwstxdv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hnivlehb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gvduqalr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3krfgvvlg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3mnoiaesi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3brvxppau.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jsagydaz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3adoxfbct.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3gkyntxdw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3hkptusqb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3bpppkwxj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3xvebmjlw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vpdkhgyl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3gfsjbbmi.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3bozvajdu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lnimoggv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xvnpauoq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3blmtnsze.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ruwfhutc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rstpoahw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3awikczly.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3eiizcric.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zanaenrz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hkgtyjyf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3unqxhhsr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nhqwzjsk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ddincppn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mreujlsf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3swlwpcee.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3oggijcax.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ssmwuvjg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3vtbkkvpm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrsbsfvg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3berxudod.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tcnjhzww.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xccxythf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gnvgilwu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wsrjtabl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wrtdzdww.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3qozjoksw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jcqrbart.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3gydyeafn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ffhhayjc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wfokdowq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3brvtnqev.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xjizoykh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zojoferc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gdkzfqfs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3mvmgsgdb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3drsifosw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3kvimtrxu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hykeraqn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ttuwgbqt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dnmukxuq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oggmwmbp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dxhqrxmv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yjnmmnwo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nfvvncfy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xzqzdbrp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fprvzvhl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3owjsmbdh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sqitqpsw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qgmscadt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kwmlexcn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3radzcrqp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cafukbyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kczwasmz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3zipsecpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ioephpwn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dmcnzgee.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3bmgyprot.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3swqmrhxp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wdgnqhck.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdptssqb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrwnfyta.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rndrkxxv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3bezsnpqy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nhqrbbim.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ntdafpgl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3dupisiwg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3fsnjeqyc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3exaokapw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwbqgxpb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3mwhzfpyw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3xitplxtb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gurmulge.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ekpqeixs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3stnaaail.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3tuyfnlwy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3cetfsnan.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxkcdzwo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzfktllo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3fjlmswlo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3slkmlees.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3fnhtrwgy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qumrgjgy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rnybnhuu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3xctlmtcx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3zwmpxptf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyewlffc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3zydoonhu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nfvuorye.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ssdyirxo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mtqowsjp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xlqrglsj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3svcctesa.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3svdnbcxz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3txvvwlhc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ewbeujot.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zjeloekb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3elwjbmog.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bceqeymv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3elkuhfew.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rlmbxpcx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hpzmndxp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fntvrxaq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xzxgicng.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3flfoivhz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qoqfqicx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3kqvuptim.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rcfrnhoz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dtqiqski.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vqxmbnkw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3lzayonep.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3dhvubtuz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ynrqcbfz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3dobqhrlt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3nupeqgva.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3btplfanf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3qummlerw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3elwymjhl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mnggfwfb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kdvlvvqb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3dfkzimdk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3mglicofi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmmxpmjl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufvdwsaq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3tpinuzax.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3sskibvks.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3teinsvtb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ahxlcrjs.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3cqbuaiaz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3iwofmmuq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3puhcqrqp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ppqtjsmo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3myuuqsrb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfejhfes.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3rkwidpll.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3klvyrkcl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3gutiktwo.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rfimipsw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3amwxvgrc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3glgkzvmf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3lzytgmxz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fjxvkypm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3enwbvzah.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wszjoytw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3pyxisfzr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bkxxkfkq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tsliwbbl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3lbkiuxob.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3rmdpnxfq.html


<!-- 参考信息 -->