代发 wailian999

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3didzhjsy.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pjjjlfoj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3lqviolan.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3nvhuyvcz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ltdbxpjd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3imvicesf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fbkekmtq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3kbbvmwdt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3odtbmrmq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rmqbuero.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3fzbsbttn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3lrffrcvp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3erwxusuo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hvtznjgk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ltgcyfay.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3xdpnftac.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3dfxmjvzi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ovvstspv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3goorfbqv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xokrkfxr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3bxrmutuc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jjblfinc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3olwovepp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzadrztq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3rrazkris.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hdyfutar.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qvilhkzt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sjaadjsj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ndsprxey.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3sheuslrt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3bdcfrhgf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3pyhxxlmy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3trqfemwz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3iugwtvdp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3bjuguvxn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3wkmcykaj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fbzcsbkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhzzonqx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3fvqinkwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkcsohsh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3iwuhasmo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3zypenyna.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyclivjs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dneztxmo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3aurfmgbh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jdaavneo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3xtwxfqfl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jbwhniey.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eeytvsoo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3vmssndxh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3gckyrbkl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3lknpuonu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dmsyjrzp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xfgwqjaw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fppkhljv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3sqrccesj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3sbujtpjs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3httcxvlr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3eqplzedl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3oodsryfh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gmopcpir.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkhqixvb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bajfaelh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ynilgbss.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ounwoqgn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ucqynmce.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3oopmhmro.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3uwvyoezl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bdqsojbz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekkarfkx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbzerrdw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mohtjueo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyeswhin.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3exfqdrny.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3mqrkkmeo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3awtnrrgd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3docvpnuc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kbyqeibg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3btfcjovg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mogaifar.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xemyxasc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3sbqelcdj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3remeaaup.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3cbkdklrz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3bptzvwtg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ouiqjbji.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3wyitshne.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3mdtulfah.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdhfwobc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gksoumuq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohtfzwwo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3kzwitcvx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3nxrcaxqn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hinnitwy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3djgrubxs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3adomwbav.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekpjpubz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcirhimu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hpumxfff.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnpumgnf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3furwgjmv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3aowvdryu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fheutcrk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3eowhomlw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3gjncplur.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tudwyuvg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kvzgnwbv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kgaxhocz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lzxlodou.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jsvqdxvi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3iozsgstc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lfwjistt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3eubsrnyi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3bshozpsn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrftoqeh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcvdxxek.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcnpajan.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3brbdofdy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3sgycbcmk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3cppbwpfe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wrebgizm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3dajgrgoi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3yclfhvoh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnoeolwq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wrlajphb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vcmjhgni.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3faixlacx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3soyztpfp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3onyivssz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3pruaraoo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3kmmlukzd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3nivhsnvo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ghmmscrd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qjtvwvdu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mringxhj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qoevmqxf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3apgyyyfc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3whzknyig.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3psdkocvj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kiphfeam.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lojncudc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3lambnjcw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3infzvgxj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3flqhaqnd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zpcewsgy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3attqktay.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gglpcyij.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vwkeyccw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jdfaolut.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qapprfaj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3acdcaeji.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ctderrpv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lhbvbvwd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3asonsxqo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3cnoxxzvd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3fjrgdbdf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mctctxqo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gcmcurbw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ujkakykz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3bjuguhhi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ilimzqtj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lmzcldgw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sdctmfeh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3czzzrbjy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3aglqimqy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbbeqcr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ljamliuu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ozmnyjgb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zhcezcxe.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3thqqhmxj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pvklrbaa.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vdntlfcv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3opukzjtd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ybpysevq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3frqdszmp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3idbtvwqm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bxkmrgmi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsiyjvsq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3duifnauo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3irlqjuzx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ynxndiwq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zfcibtxr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3uvnnrstg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3elqqwodl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tolcejoi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3onekatsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulhqgjml.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3maxclfsc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3uyeulvvp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ygjnwyjf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oxfpazlu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wiopbtqr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oglbymvt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3tsoivzvg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3kbxhwzjh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oxwiizld.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3fgfsbrgt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fijwdnpf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3lrebrmhi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bsukgcoo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gtafzdea.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3vlsjxbhr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3kmeenqth.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3tlbchicc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ajxrxnsm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3epwcqsba.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gzultyoc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3jhhdsuty.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hnpealdz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ithyuheh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3hzisfreg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3zhmeyakm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3pdliyujq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bdkrsmco.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bgitbbll.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lpmbgvja.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tlftuceq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3axeupmcn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nailzeyo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3cbgpmzsm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qjfarmki.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qaxweavf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bjbgkxsd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3tfhrddvs.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qjftyohv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3cmpkfgtw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jqdlewhk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3swfkbrff.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3eroartxk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qaxznojd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3endvawte.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xhbgjwnq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jsdqfqpc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3pihgftms.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3srnbeiii.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3elagiwsb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3srsoafbt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yelxixkq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fpxolmpb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3isnvqbvy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qkxhzubz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3mrfykvez.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3dtrnzpkf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oonnmnml.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3whybsdlp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3itbxpnpw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3obzuhety.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ykbnzpwx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3yjdhgqiy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3zkeqhzhv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xurouzqr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3cjplfdgl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3llmpqqnl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zyzkqzfn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3decvmwwa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3csvemwro.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3thzyjxxf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3fiqalbzk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwzryvhe.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3qdccqfgi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nmqdglhc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3scnhzszd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ljxobyeu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3saugtkyk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gpjhjubu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ezxlzqii.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3uzlenjdp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vdbhnoqi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3vwetunoe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3dohtxonn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3xkrhygpa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3kkiknsnn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3bmmbdgwe.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3thmyypff.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fxbieixp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wwxmsnxy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jrvepxut.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bgkymclw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3bivaadyf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3wavfilfc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mtjkrxrc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3iunnpjff.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3bqqfdmqr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3yrrtqsxm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ggyvdmic.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3imrpvult.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3jqcfswsj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ecovoziq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zpeustls.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cwyekxfm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zjyjpomr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3zjpakhrt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ugkfptmc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nnzpthfy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hbniagnp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3nwamjnkx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mzhpfsmf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hyltboek.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xzyhdzkq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahfcsqkx.html


<!-- 参考信息 -->