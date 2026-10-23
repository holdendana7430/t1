代发 wailian999

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3djyyjkjv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wpzzdgqn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bjdagnbj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3qrnvqyxm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ihzgwqmt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yotixdjo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qpaqsfbb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zlwbzrhe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kbmbzhwy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3rkeuswyy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3czogloqk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3btnlhbik.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3wnvmwbmi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zllauzbu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vhnaadkc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3uqruyeip.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3dbwitbbi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3erssmmjg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tcjftgjl.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gcsbirbu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ovnkhsvg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvudjshl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3dymwwytd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3olaadrbd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mpdzfzvl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3uivzfoiy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3syjjyfaz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ockzuwqb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3zmjjvxxg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3xfvnunzz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ivleipim.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3qptrmdum.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3mqhondzi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ssoggkry.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3hnnhdtno.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kevaqcwj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hymmafem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlehpdtk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ixrorhdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbwlfzym.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3xfqajgjm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3yvppicoh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3blvbvipm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cdtybmjf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pnikmshy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3unbgxssl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ptksprwv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lzkwrbrw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hgaxhsxe.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3awztdywi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3gguuhjnx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3jdsyshpe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3smpxgoao.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lffwppuy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ilohxkmh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ngygqjen.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3xitgwyzt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zygszjro.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3truofagl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3whannjdq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lwnxyhgu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tpzayrlg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3teywfgnq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjnnmxxd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fwlcuybg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jjvsbesa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tbiwqect.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3doiliqsn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fvawykly.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3cwekduul.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jxkrotru.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmepyywd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3klheokhm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3hymbdiml.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3tfvnwzur.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3stkdgjkh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mollcykl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bkwklnyk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfxnmibz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bcrsbbhf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocisgoky.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtxfcdmy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vfreqwuc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3gupjufmj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3igbosroo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hnivnrwe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3nyydjnje.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdlbvsrs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3iytmndck.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3crcwhalb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jrjtafrn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3nubwaxgn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cmtsxzot.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3xnvmldfg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3okjbgxim.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xvmyyaxq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3htlgqmom.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pwchihoj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gedflmeg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfcmnqaw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3siwxutix.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fyyhmxjf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mhcftayh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ybgxdeek.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3cvnydgpc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3joasikgg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3klwosjpi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aimerjjs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gezrybwb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3noqlkrcw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fbpcbaup.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vgtnflaw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3oxrlvepu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rncisdmg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3daqwtpgb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vpjmlrws.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3crfoghse.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptsqvwng.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xmzcvtqb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3zrxezqeo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sarewncq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3xbalpmth.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3utlwnkwp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3vpmxlkxc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ayepbvoc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hktuvouk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhqmalba.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xyucndhf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3mcpppdap.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdtrvrun.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ccoddjll.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3pckdkhik.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3dklstkdz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tmhhnhlh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gqglfhru.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xffrulmc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3omxlmglu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zjbrnibj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xlvrxpeo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3crdztszv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3zhdpmojm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nblqoxxq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nmqviqty.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yeqvelhu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wwkbenha.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ycigcvpw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pqichtrj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3heujhxrs.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3khazquof.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xnzznovi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ntygmutl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktwcuohy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ofbulufb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3pxclvatc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lsowihsl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ymvfyrwp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3tbitwdow.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vdpyjfqf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3cmdekhgv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ukckslig.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bjrqkwzi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cgnzeygb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ixbdkclj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujxgyrpa.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfrfuvmn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3youuutwz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3pugbhghq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lchunfld.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3qzyqkzxw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ivtjybgc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tbjlqmux.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ypqmcrki.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3efkzfenb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gayldntx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cwfspopu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wbdnhzil.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3zxsrrkko.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3pempgdtx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lhgudhra.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jwpcpdpd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mkdpoetp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kmghedbj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3uxbazjjy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gldcadbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zovcitpy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ukrhtozw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyappzlr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ukfmnfww.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nhxawnui.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuocpuun.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tqvhkibk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljcwwqvq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bthreizr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3snuyxzcb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3uzkfnkon.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ewsrfcet.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rcpojhdq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3tnsfklft.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3dzytpoid.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmkkhhut.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpohwydt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3pbpkagdv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3cwaztssh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3uljastzo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qxgodmgb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cqpiymrs.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3bnhanxad.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3eoxqchrx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsblqngx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lgazzwcf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3utmcdswd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3lyqgcqpj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kzqwdkjh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3txwruxbg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3nxdnlaqg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3pfiojwlw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rnfkwmgj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3femrgnuz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3mwbpdyys.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lzcfmdpe.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lcuddcae.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nbdyrqbv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dcrdaxuz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hvgoafea.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fqxcitku.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3xmtgfkxp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3thkiaujp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3apajvyxc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3hdxwgpuc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hnyowcoh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zwihijhv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ugsapron.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3abifxhat.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dsltnobq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3wfcwcasa.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vihvtooa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3desnrvkx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ncungadv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ukbvzpab.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mkzbbqtq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3myyrnvcq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ygthnqmk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rjttrwyu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tbndxkcd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3jagoqjqr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xbliwhsh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ddsiprgp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jpwgrghl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3esjaitmc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3zxkjtsdd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3jjjriesc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3faeronxi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxmsnwcw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3blbvmrzh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gwdgqqeq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3jschbuht.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3znzezwys.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3iqnjmuom.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3urigcsyh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mwjvtefd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xwbmrnsz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpanxxrf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ngiqlhbv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rnmnedfp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dzwfjeif.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3wbidxlyd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ouuobvfg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3chthmyja.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zipsihgg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wsiuxljl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3xyfdbfbt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ybdywile.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pcjapqwk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pqiuecue.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wykhazpo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hdyflwrt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zlfbqbcn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3quhwjttj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3hvxnjpqj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zziashsn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xyhqfsua.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3mlpcinig.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3mqhqzypz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3iwkkiuvw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wfehoimx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3lcjyjrsv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hhsixtwh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dcmykjuj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dnslwpuc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3acdyldxp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jehyyfkr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ionjlfhp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3udqlhckx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zhekuxbc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3asigknmk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3mehwjkoq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oksxbtyd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xsvbrlof.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3nplkmwwo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkffnhkf.html


<!-- 参考信息 -->