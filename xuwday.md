代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3aolksrnx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3myfvmlbh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xhshzlhj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3unclhnym.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yeumctoj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xabhdfrs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hpjqviwq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3vynymteo.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sundbuus.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ppcvsznb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3qmcdfntw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3rknmmvza.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mxaraqrm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3xuwtdgyl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xclhehwo.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hfyegsjj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3byihnqlz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3siuepaha.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wioyqrgv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3yriqghuf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cogiurbn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3udzwmkiv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3egsaouvt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxnpjqfi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gsxmlyxl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3raulduzx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3mshmydkj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3nqddedvx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3aidlevsf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ggezzdvr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hpggwcbf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3gpwrslpi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3huachccr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3cfahntbe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3iyzibdcm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jkmkyzph.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3vrtomgkr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ajrvzsgv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3oyxqhyjw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mrofycuj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vidkypzn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwdvevcz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3fgqbjppt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfmnwrrz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3kbgbzprg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ucvaapzw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3zxrbmrlu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3daptsnhx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3psjkbwxr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3oqizhdwd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3tmmfqeua.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3xntgtjeq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3acihnkwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kyrmoihy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3xlbuueow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eugssynf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3bmdarsym.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3yxvnyofd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3sfgxsbwq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hcdrevzi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lsgxpyjv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kqyoykhn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3xdxmdemm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3lpnyizaj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fvuxgurx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3keeytceh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3wgeiluhs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fguajvxf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vjwcmayl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lktezngv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ibbboune.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3dcyhdzaz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3oxfpayev.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3npkgwxqw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3otopkejp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3utkcojqf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3usveqeph.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ixtopcvh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yprlnrhh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqlqccrw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yoeauxma.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3astzhlgo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bijkpfeo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pglnzzxd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yvbshtrq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jasywuxd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cqstnhjy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pwvwvbpx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkenpctx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3lwpisslq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zxdredqu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3gupniqbt.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sehzvdsq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3aalwfytf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3httsmdva.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nxseprbn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jikmpycm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3plbfguva.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3lqfdixtf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3taybmbch.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmumqegq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3rilhdhad.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3irdbdvei.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3eszjuijq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3crougzjm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbjckeao.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsejmepg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3phzoqfki.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3dydqwxvl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3aeuigcmc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3mdbcipvx.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mspdntvn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3bpmmxgzt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fyuivstn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3foohzevp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bmlwexrr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3mvvyqrhd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hxmcyzbz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaehfgrr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lpyklcfs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3vmrbtdam.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mcwezmwg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xhscivga.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3evlmdowb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cpfjehgt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3sjhnlwgm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3udryoxbm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zmnbywwz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3vrmaftfz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3vukmfdin.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eqnlnexr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pwzcocgn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtwlethg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wreguqfv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3slzzlgzt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3fsxbnqwl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3utggjwxo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wgqiljxt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3gpttqptf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3khjvbkiz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zedqmhgs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mgcfttga.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3bzxvzmpj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3gchwgkdo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zmgqvrpx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqmgnbvi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ywiqqczl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bwzxteti.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3uhtxkrqu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eriouqec.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ikmoeuzx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3cktmpxkd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wzskkmsd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rjkfmsef.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jnefwnpr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vmpirszg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3oztympwa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3kgslnwhn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mciodtfr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ujhmwkgm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3obfzlkfz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3yxvvdduu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cziwadpk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zszhuwcm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3kwtiobsp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3sxlrzprs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3dqbqbmaa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3atokpxrq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rewvrvkt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3jnviaijf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wrtjjife.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3meijtphv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3sgwnxcvb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3lwicxeqn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hcmwdwpq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vxwqzotb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhkbfhr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ocpjyvyh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ptsjwayr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3adroyega.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vvmltorq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ikjskxfy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3fgzlnrcw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3flwkuvsw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zxpzxqio.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3otiqrgxf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oupuugyo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kjroqcfc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wxeumesj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yxjbtjoi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dldxvjbq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dhvuyvll.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3lwddfdnq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mkpwjers.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wtomlbsb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zvikvnsm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hhxarkxg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hlfcbumm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3efpsesyn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bbqwmvzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yakwzfxq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ograsgmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvlubjnd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfzlosqy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3glhxqiic.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uljwbcdp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xrbqnthi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ivmtlgvq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcwlwcdt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3yqevjdfa.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3yziinrlw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiehcdvg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3azummzgu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3mudbjwnq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3lebegyip.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wqaemepc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zfvqdyup.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3pugtiflf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3sbovepht.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ycvwjkyo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3aquixfzy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wurvsmir.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3opttyxic.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlueqvvr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmqobowt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nkxederw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3seqonzhe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qtplghlf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3oldwrvss.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3yddizgkv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3tarhsbio.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3uilunkzi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tqkxxuhh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crnqziea.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3oayrbpmk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3szfxuhds.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3lxfqrono.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3owazwadw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3btabordt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3qtkmjuxh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dgjxkkhx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3rsyhphkf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dkhrwlia.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3icamocmd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wmllwctq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bswtizhb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mixnmvoi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rbfwlmty.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3fmewbzos.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3srqpljmq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ybqvfnrd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3enabjjfw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hyetalul.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3shvvgkxd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fcljbgji.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3psjwgtkj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gqxdnqbn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jeqimpyg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3manuksox.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sqzhigvb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3lgrkyssr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3pruchlik.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lnqbnyic.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3tdlhvgrq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ljsugkmo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3tqidtuxq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bjennivp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3iyenpcli.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3zdiiefgm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rinujean.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mwshzeha.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yuwovyke.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3nsjivrwz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3nxaxryyl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkutakih.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ygvzdbuy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmbbinlz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dgfknonp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gpsrviep.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ioadgcey.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jjgqjtcw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ynycghln.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozannfoz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ahdhdnss.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pwtfpoyy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ekzbdgjd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3capgtyjn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tzkkvefn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3keygxpop.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3emjvjgau.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uqhyzykx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3jbaxfhjt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zbrrilxv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3dnbnxfqi.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3rutokrjk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3djcfcnev.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3oeyorost.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hykddgre.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3juudqzrb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3jaottfnu.html


<!-- 参考信息 -->