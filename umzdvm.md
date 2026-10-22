代发 wailian999

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bzppybqp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zpdnahbb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2xzbreegc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2trwbdrfg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2twtcbrgs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2aqtyvzqg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nkmjtijt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pwsimnqd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ajubktzk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2voajzkcu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2slznkjwo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2tyetwlvs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2keywhcap.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ocnjfpiu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2liiwlgkv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2zddqeycm.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2wzsasxaj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2jbtaqrbx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qgjprgau.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wagxcebi.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2hodtpcqn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nijzlcel.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2svmocvkm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fddezyuu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2eitxggqc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ywvlboto.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ywyzkgxn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zjytkoqv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2jocayrxc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2kkvmyigv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ulwtgkgq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2qnwtanrc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ezqyjaex.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mupcxuvz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2tmpwccto.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2tokqpgef.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xgdpsmky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pggqyrgq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2rzzdwzla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzrpbgem.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2xytaeteq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2cqphlwwu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlvwuivo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nypeyosy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hwcuchsl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cnreylmw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2hcbsarha.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2xymvqmul.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qrlmgkdl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ruxmcfzt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2cvvhuoah.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2rayyequv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cffbjnqk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ncxdkztm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rtsixlaj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2maycdkxa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2qzcsnttj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rxjozmho.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2fcbzayrk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2mseppetf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oecieyed.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvjdarge.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cjfxrqgh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2firoznsk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2idpfpugu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hlpmwpsx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ujgjmoey.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wjvohwxz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qzrgwjei.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2qybvdlfz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hcoptkna.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2baajavii.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xaybadyx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2rcvfxwdp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2mkpwtmyy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2onqptjox.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2uwoifhls.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2iwewqgvz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ontmbyuu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2owvlqthx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yquizcwa.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ovmggbck.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2goclfumf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2wwuugiru.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehxyetan.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2peicmwlz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2hglkigba.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2saneppkn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2trhhmcpl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbqtnfdb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwagskiy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2eebenhda.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2imkbmwts.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2zxyqsaeb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2aigdqnwd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qmpmhzlv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqamnpsb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2oorxfrfp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vsonetdy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2owjoerov.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rngefppi.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2yrdtxvfm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eejbxhfo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2inggoild.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2cqrvpzcd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qmcpuhue.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kecppjaq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2phvxfhmd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pkltmwxr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ksexeoio.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2uxyplyns.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2foztmgwk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2gksvtbsb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2flssyots.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrkzbvxe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvumpxaq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2reufnhvi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xlaqkgjv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2enmciacn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2qhkfruta.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqtlehdp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xkrogypb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2tfsjqdew.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2jufklllt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2hhmznaml.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ixmfxxfa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2urvxqkdv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nmnxenjq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xwhdmojb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2oqcrrxuw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ucrwcddv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2oofyefxu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2tohseixs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nhlexsbn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kytxtthe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2shgbxnjl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2qnkodhgg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2dtpxexwp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2itfzmzpm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2dedoiukr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2mntrnmmp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2oracttrv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wbrvycft.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2smxjikpu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dexwdvqq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2pbpbqxiz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nnvcjamj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2plmfeubv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hqmkwesk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hcidhbsg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2iaqdnbmu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zrgrjvhy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ucldclcn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dttcxurp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2hplqstyu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2aouizrac.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2sfsjvwbk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qkocsbou.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2prjrsjfl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2wgdznvek.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfgccwmn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dmxmmvcc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czbggidl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2edmbymbm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qesqajbp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ddawvduu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rwyrbath.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2idvbiiqb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2afggftkj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zlnsafao.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dgufphtz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2egeojxqb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zgxcoreu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iifmkems.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wvcjtbvo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mdqjvtzk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2cfoksgwm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2yxajmkys.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2euvvbqlu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ctzgpyus.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hamigkwm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2evesprxe.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2uuzzqchi.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xmgphfgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dudbxufy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nmsgabgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntqaxwse.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2aroclffp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xprlwsqy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jaujyywy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ubmrdenl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vphjohbd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hntrbggo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2tlbivtcm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vktgsaek.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vpenpsdu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2qlyzhirq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2hbpnzpuu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxofyfid.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uobbftyl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aaaxabki.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jaqbjiuh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2weqjswdz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qzhgcuxj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2xooayclp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pmowmgcm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2cyrjqsut.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwndbevy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2msidxsuw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2aggkgfds.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2acjotxtn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2yhgvhjnz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tkdxptyo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2stpinebt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ksgjmsdu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ljrsxbgv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2jcbgkooo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hogmkqjw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nfbcvgnp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lrikmytx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rcfrvnub.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2myzikjpu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cnsbacqi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2tdefolbr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qrhfffot.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2xmuoacdl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qvskhoev.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jdcqnnta.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wcstklfg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2sggoxrxm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wtsmdbep.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2nhgjafrt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nsvovwkl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ltftkscp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2uuhkaqsl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cvevucpm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nytzzzbq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rwhsmsst.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vtaxjemb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pubxyutj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wycxkyfm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2xkatznup.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2mdimppah.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zmiaipex.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2bmrnogat.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wepzqezs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xpaisykv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qdydlbwu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2odojonsz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mwmdxqsa.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ilxdcxdk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2eeimspwe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2uuhryvij.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xeaknnkm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlgsisrj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2qbzdrvgr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ahrfdkjt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2nkqyudzx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xwzklklk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kuapnovt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mivnugub.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2viwkfjou.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hqautvkb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ithvpxea.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xhuffxhp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2hrqlayah.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tlfweefc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2gctyxuyr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hwtllfek.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2egnxgjzq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2vsiasije.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2effrwehb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yulsfyvc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pjuspbij.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vvdxsvfi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2bzpnltge.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xtemzlmm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2hhisprdb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ezenqqsp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2rztovazt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zrdoopxm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ifxwyoli.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xyadddev.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2vkapgdwq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2cgskoklj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2kpzcxwmx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2accmqwrf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lbhtqjtu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ikbsnyjt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2quscdpwr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2numxijhi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2xmpmuhvt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2iodebyxi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ipuipvrs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qozaswql.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2cactwajx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cngkooio.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcvvayqg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2yoxvvquf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2njbshpxq.html


<!-- 参考信息 -->