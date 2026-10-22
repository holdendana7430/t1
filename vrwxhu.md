代发 wailian999

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2fsiqqpsg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2jbkhycaw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oylqocjq.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iayoayqz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2hfyzbmcw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2brunoplw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qpplkwyc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2shpdehch.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nhawjktc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jzjkihfp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lqrpkzas.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2znobpxmc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ednfegvb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2loulwwkt.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ppcbzdgn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2aetaajzp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hwpnyoco.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xmvcfgon.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dfcepqwy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2qhyknzho.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2jgitonrt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2hjxboxjz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mzcdcvml.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zvsjhauu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ejxlpjtz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2bizzerog.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2diewoppu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hzrzfsdh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2viumyaxs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jefbsdgg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ksrhbwkb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkucbiem.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2fgcxfbvq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2kdrtjjzf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2pcritmrg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2banckjho.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2fdzdbfca.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dtrettbg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2rovjmdej.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jlemocjc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2appjyaan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guztrdfn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2dkwrcaws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqmiqlob.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2wcqeosfj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ldchlodo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoajkotf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2beuqkzvt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2prwpcuhj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bwhsaqqe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2qpoeutcw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bpentbof.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lyoyzcdv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kuvzukdh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ldgkwkdw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qcuoobsh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yqngtaky.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2axdfqcbd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hjbpiqnd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2dapoghyi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xrrkczkf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hyzzvyhl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2jcochvyz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ygmrcaxb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2khhxnlyh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdmwddjt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgcqkmko.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zmikxkqx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zxsdebkv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2cmbhubsp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bvdeaywj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tgsicxux.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wluwmmhf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2evmydasd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpmngfrq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kgfobbbh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmynfbjs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xhruggti.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kicqgwgi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2yytwpuip.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hrzvkdsf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2yvcvbnkh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2egdaejxs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljdkigjq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kqebgwvx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvbprhwf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2arxvpplf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2vzbmnhvb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bszlneuj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wvoveusc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2lwhchgux.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2dryxyybs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygcjqyee.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ybpuvqff.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2fgsvawvm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ylaxuuvd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2awerugol.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2wcaaavta.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rlwjsrte.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2dzrpuvak.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wvgaaetj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wibvzfsr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvgkyeqq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jnsnfady.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ghfgrbqq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xmnkbezi.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2muadyuyg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2nhbmwyrc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2phvtqcuz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bfkskaqm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kblwifnl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qqfoobhn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lzhsemfd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ikqqjafb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cvmyfrxg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iunqpbqg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ezgrrhdi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2qtirlvhv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dbxgmjlz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aqqhhvlu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lcslmmvo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rofduzub.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2iisaidgy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2akdwwsfb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xfhwgdpd.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2jyvsnwhw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2abdmpncc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2depdnyrg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ccpwwvzj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lvagwvfk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wuejwsur.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2nnqjtflf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fbygcris.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2klnygtim.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2cwwrstpk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2knqflpvb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eovblvsx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dnxmdjlb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vxgpuknb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2idzlxajd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2yccqqqcf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ilxnmegs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2lczdmnsp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qsopubgv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2eudmqnhk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rbpzkdcz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jvbggiov.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2eqxgfmkx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eitzugnw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xncpzkga.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2snzcbjlg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2uvxlwrpq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2oxmhyayn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nhihbgka.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mdyieoxq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2styqriuv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tybjyctz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ggrloplo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2gpipnhvh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2rdeanlak.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2sfvpuxyj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2pfobykvi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rklomnsz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vlfjlldz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ebboijpv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hejgkcmt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wczsqobs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2smclomrq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ymlqztyn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwwmlusi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qojextsa.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2teqhlytt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2rkzafafq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qwzxudkz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zaciaqxf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2emuzwvkf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hmnaotuz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sxsmgnws.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fwmbpkou.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2wuhddqlx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ongjvzea.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2obgxjkku.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ylrgtbuk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bnvmpdtk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wcmydyaq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lwiyziyu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qmulnvov.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ewceftbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dljpzrgj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nehjthbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vutbnshi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bbhwlaqq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lgcgiiry.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mlmarmkj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2casigidg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aoziijfu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzymnall.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tnaommfu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xwpcuypi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lucsfobw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dtdyfvbn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2sfdrwpaw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dijrblrw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rszjbmpa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdlqoqrz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2hxagvgof.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2syvsdhhe.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xaifymfa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2fkpezdew.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2wazskmvp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2arcrorot.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2thdgtzos.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rffyhkbj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oabhuebh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyssiftq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2wteiulpn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2czrtvbcu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ibxrjtro.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2gyylfozt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2unbgwgdz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2asmqzhos.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yruqhicf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2stkznyuf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2kjqsohrr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jyocuhop.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlrkeczc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tiwcljsv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ussdpbim.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nddvasfa.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qqgcnvjl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jzctscch.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ukwiesdh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2orpznffq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gvmowhpu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qsktohxs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2djfanyig.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ptlpphmm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kvdexsme.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2mfunlead.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dltyvgxr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vwqxbzrl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wgdahzpd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2sdurufhj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nioxwzos.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oiuuusey.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2fgmdmour.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2pcqyujyr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2imkohhri.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2aeomucks.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2prqncwuw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mknmoekd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2yhwxhlvu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2mmacwcbv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2xrovayav.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dxcyrozd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2wjogvgab.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zhaxfsdp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvvfdncn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xatlzjdg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2oxptzyyq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2lusobppy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jpbzvczi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwknvcjn.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2wkebeqiq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jeqgrcby.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hlifyxhx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ltudtmgo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rmuexuoh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxrnrrsg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mpvdafsk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2euwbrzxu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rgfkprri.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2bspxvpye.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2whuirict.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2kosxcsgr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xwrfyweo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2onstddia.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pfnhdbju.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fraqeiyb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2hikhyfux.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lffmatmb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2cfipbkzj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jbwrwojc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wxykewhy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rgbimkae.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2dszsstrb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2vqvxoouy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2wtgjyciv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vfvaannr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fostupuw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2umykinbk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lwsnnhih.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ktmgfbbf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tylookbz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2elugeath.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bopkxfdw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2buiwzasa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fokqipei.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2pflxxsia.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2yqypjeov.html


<!-- 参考信息 -->