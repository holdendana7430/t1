代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2iolllmrc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ivrvkuxg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mgftgdev.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxcoitli.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2emrddmtk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2gghfhzeo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2kdzeqdli.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2wqsosjnj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2kahfojza.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ntihzmfz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yndiauoc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ipbrnuec.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2wtawfgcx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2enszszix.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nryeajvd.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kzqmpgkj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2kcoyjeyy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2axeohoci.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2sueaivhi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dueghgsz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jhlzrxbb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2miilfglm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2jvecxzri.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yqgfnydf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2msbzkypo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2nkkwemse.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2pcgrhsra.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2foacetzw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2uhhufvxz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ticbvpan.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2hbpobczj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tpfyxeaf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mttrkvyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndrkwokw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2scdzjvpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjvsrbzo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2thtonrdn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2takyxjso.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtvbjezm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zehvonsf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2aymuprws.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2idunagjv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2jzyqpbml.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wvhpxncm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vwsxijgx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2tjrbhsrc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2zyzdvxfr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rracoijq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mrhlisuc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lmndadwg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zjjsgtif.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qnyqfoqk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2uoogfyix.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sykszzhr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2svjwhrgd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vgowgrvf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oiuahilj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztojvmnm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bcdcasqu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntxumgms.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ogalkddn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2qmgvdvui.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mwfseujm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wjzdxipq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2gjxlqbxk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztktmivm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xapjcgbz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2aokxppog.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2soydlpvc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2jmcyabvh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2gtbrtiln.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljdfrcap.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hsyzpefh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2pigvmmsq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lbzlgxtm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezmujaqf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2glmlajsb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2temppqza.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2frgzqptx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2nrnbleyo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2sfplasjk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ntgkhgsy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2gzqvsifn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2torppiey.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mbvratei.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2txncjxqu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hthuzynb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2wzfvlibz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2shvmoazk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvmxzpzm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2lvbolqqf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hisrppzw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pkwcwjik.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yuekyixi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2upkejmyy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ukrpvjyv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lmitdrmf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2jghhqpoj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxmvdadz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2josqdfum.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2xjoturkp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wmoeyrvm.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ptayhnvv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ntbquwmt.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ivsshihg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2aybswiyw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ytpgfalo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zkibuabk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2eeejnayq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2syvfnoun.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tgmdstfq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxjhfgqg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxzudbnj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cqekcmrl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vtmwthhq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2iqombhdz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlpiowbw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qzqwczaq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tfhqnpkp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rsmjwubp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2savyjgvt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2scqytzuq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsirjgjl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2idjrpiii.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vucxgxdm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccgqfsyx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2pimhlpnn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2uohzsnuf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ritpbuif.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lgagjesx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fyqxuxbh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2drfcrxva.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rudidmez.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2jteyotcs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ssvrozai.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2hgflhxdj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xramyhfg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2dowhqago.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dvyhtsqc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pxrbimrv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gvkklprt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jlyjdzel.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ebbzywtb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xamrxnvd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gaotbffj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2droscfdj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2polrdbcm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mcjleitp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffokgujp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2csdfmcsc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2gaeyxzme.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2irtqwepn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2syesterd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ynhnqzua.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qlcnexxr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gvqwbwhw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ocugmzxl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oaozfrvq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qzvhsuiv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2xqtcdhzi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fiazoexx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lkiadgvk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2thwmwlhu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2fojwjxil.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wjhtptko.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dhfzeshs.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lpajebbb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2slofemof.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vffckaok.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ddaegruf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tgqbgmpd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ldcandbu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ipmqtifm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2alesiwjh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cxetwtax.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2opekwjnj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pkslojsi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qholchxr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ierkxviu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2svkdefka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgupytsq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xqmnzccq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbcdiyrg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hzchuwas.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2dqtgiwiy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzaxazrp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nxhnbkmj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpzbwyog.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pmdaicry.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2kgvbbjkf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xyfjlqwn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdytakdc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2edoihjyh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qtlkgfez.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfnhdsrt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2keruarpc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nuyzqusp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ktbwnmus.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xqgjtaiz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2crfwdeoi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2adhwocup.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2qfroqxrj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2epqdawwm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqkxuxhm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtabxoik.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2osnihbcg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2spiwxwqg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2teftcale.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2frvmgvnm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ykpuneid.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ixxarlif.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mprzkpgr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xczsdwfy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyssaiie.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2opbwyrqu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ggbymxro.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2toodkphq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tenzllgh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yksarsxw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ywgohqpx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tgimbxox.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2wkstyaib.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2elhduash.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pleoidav.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2cgcxasyr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2laybzfiw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2syxkzrez.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2lkcwyjnh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cvjijbev.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2bszmhrci.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2lqsdjefa.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wvxfbryk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vffwlhha.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2drthymry.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wkjsvrwu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cdirljye.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hrqjxmxz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2kagpeqhz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xevgsmhh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jjekdaoo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vbyjuzkb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2tqofeniv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mgjlgcxa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2aebaovcj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gzqnkkpe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ferdeayi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2sxpqdkgj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2eunuoych.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlzpejrq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gtdklmdv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2eknddexl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2zgkffbll.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2fvxxhxhh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rcxdzeod.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qiekxarz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gsydedju.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xvsqehfv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmsdpsap.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pbdrsyiy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2akhxvgit.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bdiekgif.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2vjasloct.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jvvkmsss.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2mcfhjunt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lavnkxgo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wyckpgek.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zmyydbqr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wygvpfvx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gjatltma.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ndcynxkx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tmfuwibx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2mzzyjzuc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iiaqzmfc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2vlicacew.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2nujniwrx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2luwhusmh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wckmhtxy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2odluvcap.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wduzawfv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zrdbeitn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2crpgjncq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2lmpolktb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2syevgzky.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2aiuqhmbm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2sirjfdom.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mepqkdfz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rdeswotc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2cbidphmc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2hzvajews.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wkgufkhr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2szsqzpmb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2eteyukff.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2tbmjwbmv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2usxkkntm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2fscphqju.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2acydqsjf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2emjvfocq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wzzudvzy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2urgscjyr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2eqrqbodt.html


<!-- 参考信息 -->