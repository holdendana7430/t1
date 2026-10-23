代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3usfkwypb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3badjmwle.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3fxplhtra.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3byrjiunw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3xzqvloxq.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qwvebpix.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3mnatomxi.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3onalpkdx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3wsldmuwu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xqgmjais.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3emhyhxvc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rikdxewf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ppifjvuz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bivoampf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kzsfljoh.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3kkxihlbl.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ujjawzdx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrlvccqy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3biucqgli.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3tifltgmm.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bocgfwdq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3bemquqsc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zisifras.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3rlscmodf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xddlxiwv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cduorzzd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3epxxxddi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3iomwgoac.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tjwjflci.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cocyaaoi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fhdjocza.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3wcawaodg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fpyyvsub.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3gkcxjyzs.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ehrbbxxl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3irbhunvb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3chazjgof.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tjtkeift.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wqppkuhm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3pjkuaptk.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tffdfoei.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3qhhldxny.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cywluauc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fwelrrhi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3smgoijhc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3nrmzavwc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jwzjusta.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pralikin.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3hcrdfizx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gthuskby.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3opnuluej.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qtbnidot.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wtamqnsd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wswnslyn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3mmgykahr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3acfcobzi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3qwktllxw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gmoctfml.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jjqesiui.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zkznwcxa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rttghrbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kncffxep.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ggfqratr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxmddtzb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3sjjaewfr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qabkthxv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3hmxeukuy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fppogchn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gwiqyssh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vybtxhed.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3lwmnkaxz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3vqoxmgsl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fyhoqwst.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3nqlspoac.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3aqoaiwrq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3scopeibe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vhojrmun.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hfrppqds.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bjofnptl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3hhtxmgus.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3squjtiha.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sreafysy.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3dksrmpuq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3czbzkzes.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifbfbkio.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mutkowvn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jmhnawem.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3swjfezkx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ljsmmvuj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3pxkrhhju.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3oixjfejy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kgwaflvn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mfmjhhgq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygsjyhsm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3yvfrppnf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vkqaqzfy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgxintue.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zuyalfhe.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3nvfecwub.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nyqvlfvm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jbukewmn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3hbaeswey.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3topfszug.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xoberqds.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ezbvkjfm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3onovjetp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yevidbep.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3miusvace.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjkwarfj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3fjoahtsb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zlktzula.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3xmkagbcg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vtxtijpy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fyagydks.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3brdagvxw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3lgyxwjog.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3eiimxdnf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujxofsfj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ehzjmtqm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dcuntgbv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3nbdbrgfj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbobftgm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kxoifrak.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qzwriilk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xbixdvql.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3cthyxaar.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujgcivll.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3kaxaoded.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3itobmxkh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3svliopou.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tzlezcxz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kavldutp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uipzllpx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ngsagpaj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3tlspqfct.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yefnuvba.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dbgxawjd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jezqokwa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mbuhjgvh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rlnvbtwx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwisorbn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aebzktdy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kzxxdtkx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3wisfoltd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuqabcng.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3dmcnihcx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3bfpiyrah.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zltotfcz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3cigrjuri.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3sbmfeadc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwbcpyvr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3icmsorrm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tzkmughw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3yfjvxhvp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3xoondobr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3byssswej.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3juabmagm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3adqgofax.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tivzqlpq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gegppnap.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3wrgvtulg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qmoedcch.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3mtxwqqci.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3uzfcwwic.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fvhuzyuf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bfhfuecs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pvczlbgy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bnermlrn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zomukccn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vvqkcpar.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3fdlttmhq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jxvyfiwy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3naftqdug.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3mkxyncgc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3opiaqjkr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kjnrnrii.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3swiwtljz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wbikygou.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3knlpllla.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hahkcbcl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3gnivnvcg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vhnwgkoc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3prfzufck.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3caoafhwh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tizancwg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ilhckihf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrxkhfog.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sldyunek.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qwnrkwdg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bjlsrhiu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3pzhjnocu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3owhyzcnt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3csndcjlf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gfrekygv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cbwnnfht.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3manmlbcn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vvusngwr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ypkfmbvf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lwqnzwbh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3tgsokjlq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3hhzcbddx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fohhqxfx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3akrafxca.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zynrtvdv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fgejliyc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3rsznshfc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3iqfdhkhk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xjkjewtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcfassds.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rayntufb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owkfhlbj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gnvwiqkh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3echizacp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gojkarvz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3suzwckvc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yzfjbsxr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfqifjbd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3pcwaplnv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3maqoskxh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tofggolx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rglavxhm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3bahfvmgt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3taddwjrt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnfmooco.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tvoirxzg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3jfgcyzti.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hhbvdxeh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ouqgrnbt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3nbbitmkk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mgbzoszz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3uelxpsls.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rafyjchi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nibudubi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qncnchfd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtjyuelw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3motcfudv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ksdvazdx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3upnvymcz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3lmmwyffw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ytkwrrcf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mlxijyiq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ektvgzal.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3czuxpbaa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3bjichcez.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mpcypumr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cqulwdvo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vsitzikf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ipkssoln.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3javnchra.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3kgxeblcr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wnyewtak.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mpivqcrp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rbezmgvq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hnwzqvqo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bzosozhk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3spqvzqwd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vottxojo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3xdvcyahu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3umhqoahu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zsbrkwzk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vlvjjijx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3gdceefjq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3oeyepgvg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lxbpcnna.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mfxblrqd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3gpihrnnj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ehxxhroz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3knqsutum.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3gaskyzxe.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3rjaeknbd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3njyedxfk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ajqddscr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3pnpxlukc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vuybzmqq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wbtdzgkx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ritrrkpz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqtwhftf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3axaelzrs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ithjnuuy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3nysdgaob.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3yianvmgf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3cqaxrkqp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqvisjqr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3fmeqcjfk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfbtmgdr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsaquupd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wmwjtrsg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qddnttph.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmmuczii.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3vykctiid.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ighximsc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3sugsgiqa.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ndgjvbhk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qdbetlqc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3xpzneajk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wtwgqbwu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ycshhaim.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tzobrfoi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qoflqvsj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3fvaamzix.html


<!-- 参考信息 -->