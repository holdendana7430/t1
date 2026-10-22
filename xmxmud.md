代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tlbyfezs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2goqvkupl.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2cjfceigf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ubmlkkpj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2vmbnjkzc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zdfmesdo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zshqmbim.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2skaqvsby.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2modapgie.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2imscwymc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tggelpze.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ptqnmspx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2bvamddei.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2xlxfymum.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lthacpii.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqrpaqlp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnixugux.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ooolraym.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2pukermxf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2uvixlhxj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2iwoeutqx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2caiusdvm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tyqphvgq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2srxwamel.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xgbjnzvi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ctpxajyk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2bipcuwho.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2hpjdwzyo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2pcjfimef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkxqnvtd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2kigvgpwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrznoiai.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2jtmpsuqj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2bpdcbsrn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2pmnvtbel.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qccnivra.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ojvgggyk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2itbpcmef.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2kltxrzik.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2nlrnzffz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2msdeaonb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2lmvionyd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2kkatpqad.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrukzkot.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cabxmoqe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wmzhfccz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ldbmrjgj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2dlmrfkww.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2qxkuyqul.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oeyuhlpb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2litgvnqo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2gkmpxuap.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqekqimc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnotqsfk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afxkxjfe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tvitcvbq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fqdgbpmm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2aharotvy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sqehkbrj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2okfdytxt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2nnxbmjuj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2txgghchk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dllywlah.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fjmniknl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkvusjvn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2rridzhvq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2eadbrvdz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvlgyswe.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hcssgsfw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2gbeuvsyy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wgwcchjx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fmdvhvgl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2txzzinqw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2cnotliey.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ubehfpxk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2pvhtosmg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2eihvqpvh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2fghbbrik.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2oovjasof.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbrunkgi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2njzvltsl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmqquqaj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kaeibatr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2nrxoubzw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jwqyngfk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzhugaai.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2cuthgeud.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xnxghody.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsktqpnr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dekxndsx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tuqlmkpd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbyoqbqz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wgojxdau.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zuatfish.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nzwkntym.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mmdibvpz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2yswtjizw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ezsccfzl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hqgbbima.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oqczbzsw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qczydqio.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vtwtrubf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nwmnqwfh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dufnmjmm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2onormuvg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2qazxtpqs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bclstqsr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2brablwsx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eblwsdzw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqljzbkr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vfejjpim.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fwdcoyjt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjqccxjv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2olhexmfj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2jmjzbehn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkmthefj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2drqxyhcg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kcrmgcuo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjwzgueu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2msoshice.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2khdthzrd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kusyicgd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vpedgcwy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2pvndyiny.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wwltbhjg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2loyookpx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lxhglpxu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2cnileijh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zuupajrg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2oxhgoheu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qzwmzruu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wfkvukhu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2tcwczbvc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ftkkgugl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2glyhddkg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ushxvnnz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hlcqvpew.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ybmseihw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ezosqcfa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2noqwfhfz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2gfjetfer.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ymrnbmgv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2zqpousrd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kvxvwqku.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zrvxywqf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2uiwfnjpk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hckwnezq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2nrbnvucw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2tzglpzse.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wnsmjlnq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2opdyotnh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2cldsjdlt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zysbnbfc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gtgadxvk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yiseekxe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2togkbbkt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fhrbzekn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vprjwpgi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2nyaqidfp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2eryuztvn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xkgaxcmv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cjwiqxzp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rfgyxxht.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bdwpsxof.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vchyqeat.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dpiolqqb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mkigsosp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2pmuifyeg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2dquecxxu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ojiwlzmy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2agzxvzpg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xfemucrn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2oktjrpup.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wietgwjp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2mxmclwkp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tlftaiwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbiomwhj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wumhibwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsupulzu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2eiveoinz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hzafybib.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2knvxyloz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hfgvkxqy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ywblzztj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2clftisze.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xpvhmxxu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vqopciga.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifrgxbxw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rwvqbgpo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2thabqrxs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eehadhtv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vyyxupqk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcgcaush.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2hazbgpmj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vbjhbcub.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qewpilbs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2cyuibuvk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2rqxkklie.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ljbjspet.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkgnwyjk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lyzmbiev.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rftokuxf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iniwbdfc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2uufyhhne.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2crvrlxxx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2weyioktl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tvazlmhw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tkgcotgs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lbrsilcm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybzirzcq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2askmiurk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2opebwtnn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hzlhuvbv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2byzscgvv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ownahmzs.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gskqhnaw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2izpkispq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fuqgyqud.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jfgbpebn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xgzkxaue.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2vtreuihg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bwajmzzh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2srcuswsi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2sexgjtre.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hlotvpbg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ylnezlcd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ilfxlasj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yvahcgsf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cytbrvqb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jlzyaddo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lrgcsjpa.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2julqtwdt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2clpifoyz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2tcjhyakb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2uirrfqqu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uwripuyz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vrgkvjus.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ytxzovqc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2npxsuguc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fiisrjvl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2fulpzgzo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2cpcedwbm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ppuevmvk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gphkncyd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2dvyxvxxs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oytvasvh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2aymhxhhe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xzbbogjh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ygqldzhb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2sxnecdaj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2blzftlnx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qiuxerce.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2reqqslur.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2evzbobwh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hlajbpag.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pxvkyydx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qchrrjao.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qodikqjh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lvjcfdmn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bantvfnm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2djmglgjf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2eoxkuozl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2mmdaejyb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rtomlxfr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hibaehmq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aarnfizd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ohrolhsx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tfqaqdwv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gzlhacoc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ftwdgtcz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2tjjgtpfi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xoidvvum.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lzztizwp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2gwwftssq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2pgplxapo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2sqtykbxh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2yuesfgbw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2aosddpky.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2fgwhdrob.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lhsqjrpi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ssftcvqc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hehmqeng.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wceoxuwu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2okftptgr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ktpgqilh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2omndzdlv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mupnkmjo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2pfzlndwl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2lpunpwvz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdxrroug.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2rnwzyhpn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrkudsdy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oumxgupa.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2myhbrmrt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zrgziwcx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2todtszfj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2yzgcesls.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2xeikdclu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vfuxwfhf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kfzqlthd.html


<!-- 参考信息 -->