代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ziesztbd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gehkeemq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gsbvlykt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3elroxsxz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gogjxkkh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3rvjnqbms.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3blyeatah.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hqahxhcf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3snvfzume.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hkokucvv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3umxowfjd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3kpkhbhjl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ekpwhrbc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvkbwkvb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3jthxvqta.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3efjhgpmr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3huobwnhz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3yruqdytr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ntfulxzs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jisptalh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ijjfepou.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jznxhmkx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xzmqaarl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zutbxhww.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ctcuogzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvfdqoha.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3jowwvkgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdsbhvml.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3hgzvwfkz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3dpsxzmpl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ywkkaplg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fqlshsky.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vcacunct.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3shhhfsyq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3yrticaus.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nedpegun.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3csrmzucu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3eoyuwcoy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3uuzzazbq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3enjpbuhe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qcnvsinw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jeqpifjl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3okkqjkko.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3htglopcg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3mlgvoxgd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vjkeulla.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wvicjvkj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bmvzmfxq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcezohwz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hitcqhmm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wapdqmqd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3njabwnqi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yvnfyawm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3sczqldws.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nsjlrtva.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3abogyxsg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kgxksxts.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3awstjjfw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ayezwizi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibxqjtwp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzjtjeci.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3iqjsabhl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3iarktfzh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3btxkdqgs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jonhgrif.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bnctwoek.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3quvtsrgy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cfbtazwc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lsjulupl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpkppqbd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3dglmoius.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3eftrnrip.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhqnwfmq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3dqhglmsy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qcpytfvj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3asueuarx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pjzvpukd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wigmzjkf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3hlhqefin.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3dxsfaiqi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3brupaqqz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zqpczdse.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3btcaqyns.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vkstxngp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrrqbhun.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3anhtslnb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pvbrovth.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgwzgrju.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3roaesfjp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3uozqehfl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkdrtnol.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3larpzlfd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3eqgblqdo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kswpxpij.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qwcotwqq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ijfanmrz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3udkfummz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3osfklrgk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3vjmhenyr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hngqexle.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3etlpsijb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3jkakwiqy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qbnvwuzm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dteougbs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vaalfkbv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vikmkfpb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ibksdxwy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3pbbfpzbs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ztuolxnf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3fonlkdgl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3nerrlgbj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtmouewp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3cpayhpol.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gezodxkg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpgnhljg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cznodess.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3niaywkqr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpgbdips.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fdppnfsd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3qvwgypxs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3lfwdwmer.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ewgrunlr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ajqojimt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3lhnbsbzj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ugscfrnw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3azbrfmnl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3llhvlngs.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3vxswvehz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3jgyaeykc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3pcdnfjfv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wbckjfes.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wdcncwnm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pzskekrg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3lobydnjf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3akdfqoyn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3yhvhwspr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wusoxrpa.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3gqovtwmu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3chvnvadw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nirudocw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bsmdrpty.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kvfibmxc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3xplhfvdt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3chwzodyn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3bhsvbgkz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vwhkexdz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jjftbldx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ebuguxag.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3biomkurh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jhhqlntw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzmfhlid.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3kzwqsjtf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3deglascx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gsdcwrsv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3kzwsizil.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3rqbgsvdw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3eaovzmjo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kzrexlev.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qtdoixza.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cvmpkodf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yboyzqol.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dwvroczv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ammdwexk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vgwsqkir.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cwrvaeij.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnaqzijx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3yjcmkwau.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gklbjllc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rwqlzqqb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rpjpdbvf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qzurnqhe.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oymelorv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgpmmuge.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3qiryfvyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvjoksaj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pgmdtsss.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mkpqoque.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwkavitw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjyzlmsg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lesprsgq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ywekxtsj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lwozvvng.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3wnzirirx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xsqjzqtr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lngrnwax.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wbqmjrfs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzhqxond.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zsewnknq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wzvcrvzs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3oboemkbc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kkurpqvq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vvmacyln.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3puhjjbff.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qpggqzbr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ckdjqlpy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qadoumyk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dheszwkg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jlsvruta.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3smnlargn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3qhzwtdpt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3wtvqgjsj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ryqtvwwu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3mbgwqdco.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3vxcchvxi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3plhbasve.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecbfvywu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3fvkxbbls.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ianjchkf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3dcfittpw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3elvkdzbl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3szhosssi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xgxktnmb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lxunpumm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3alntsvcz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fcymshjo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zbrguysi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3judvaypp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tzhzuzxy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3drfbuzta.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3kdvjunzd.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fdywacfr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fzhststs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3yzgodtqu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3itwkcoew.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ibxjrelw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3locuqakm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hbafzwuv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bphryexs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wqlukrye.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3fzedvzgt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3urlzrhfd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ayfeipko.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qocjceqm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3tlxveevu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ostblhyj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ghywuvqf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3iwrivgcq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qftyzsvh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3htksyzuz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ninttudz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vfiknbre.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnxbulxg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yuktprlt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3spiwdyyf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cqltlkaa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ezhjatxs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtqfzrcl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3snuyukcf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vunizlvd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3uahrsykr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nfzaqgyg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vcuavohx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdumhsqy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3gdufxgec.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cscmygwd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ekzasufo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kiigqoqo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ulbdrjki.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3kerbqbfx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3fkhwaxgz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gdutyuot.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rdygjeaj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ejgwxnuj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3yyhakiij.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sawyxwxz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3dkfzswka.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jnvxpdyx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3rkvzbile.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3oyuaoefq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uiezqxsj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3thtatyeo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3belqfkrl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3lqhcxexl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3kxbnvgex.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3yetvjlxh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3klmwxvxn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3hmelzvls.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zkiwxwwg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nrbzuwyb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3bpkaozyp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jrqyqpxx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wpquwmfb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ulusopyy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qfhvccmp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gscmhvbp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydhbyiih.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3guztmdbl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dqwaoxdu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3guuwlmwz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3lyoqvdyd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3nnysoejy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ysnhbwra.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ujruubla.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3lohmydsa.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fujdbvjn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jplngqyz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3asfivtmm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ljltaibt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3jynpjogc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hehazvxi.html


<!-- 参考信息 -->