代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3nrfxtqbq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3aswjdyes.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ymveogmz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3prnrzwqn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vihczdxi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3riqfuwfm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3onzxgywr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3wpnxxnpb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fxgqqmvt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3kgpvfbme.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3loygzhjc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xuqsrqlr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3zztksgkc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ihpgfpwy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mggsgzkb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hyrnsand.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbhaugdz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uowlmduo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3wcyqcryt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uyzlcevx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3lrdcyncd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xgwrqoqo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3hhllamxp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ltvzdmws.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3egvlcnmp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yesjvoqi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3lkxisrrg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3urbeodmn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kmsruoda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofonspio.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3nkujzbdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhorqbht.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3snauetuw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mpyuzjtz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3kuzfkhdc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zmwzmlds.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lzlhpbbm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bttqggbq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3tyifdtiz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3uletboul.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3awhyjaqs.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3sctqwese.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fcmezkbh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtraswmc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kqbclaje.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jhlfnxgl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vzpcjeoi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3zkrifjbo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ssxybdzj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wbcztheh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3emwaengq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3qtcutzrx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utdfzjqm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zienvcui.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3asqltjgi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iqccsvju.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3acvvyenu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3dlaelvwo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ykvgszfh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3uedobwvr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3rmtlelsw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vmvqcrvl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lvulzjpj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmvrhajt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wuaujsmi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3idoudnlb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dzjjjgoa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctphsjzn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tqddvtgb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3wgzkapoi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3kuxmzimv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rkrzbayd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3uidjygtt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlnldtne.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cvdwxmet.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3clbeuvwf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3unyncdtt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gmbfskvw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3sczncina.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3hqvegoah.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wjnokejj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfacdmso.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3bgbyasgx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3inqdrrph.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cwsplwlc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3difzmiqs.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3qopveyjx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vdlvpopx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbcsfbsn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yqdugmfk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayczvubk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3srbtcaut.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3salqjvqi.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jvtkxvqh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vimvyipt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cjaurdck.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zybcqtpa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zfbbwhit.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dnjozbtp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eejcnebx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kutfxylg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3fhtkyxyw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3prtrkurx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yppowsnm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3tvfmywig.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3texiqwcw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wuxiaarl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tyljqqjd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqhrvlhy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lnytvhhl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tilpzvqp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3zuzplgzv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3onylyiji.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mvnozmmr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zdhdohwj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3khrhycca.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3onhglgze.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lhfvxzwe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3gjjrgolg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3wxwolvwv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3llnmdsbn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jzubmnig.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3cuazbfes.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3istbvhvl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3svroynuv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tpnlvint.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3frjomooy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3elrgofff.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3dcoclqzo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xjdrhqgg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3bpbcryko.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mafowyak.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ztcqqbbl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3wrybpirr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3goarqjhu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bbqcjzug.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dwbwtdbw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3twitvleo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gwdijrxx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vcwatuhc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3pcrmzxvv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3pnskzgcj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3usdwobrq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cygfskxe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjmccbhe.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3cdamevaa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rwdcnxom.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3saljumei.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3jmvqanom.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3plyusshz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3vgngzlkx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3kfuhrayq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yrlzqnkl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pqxlrstl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urjklujy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwczmqhi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3laowaoad.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3edbvoobx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ijprcems.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3irrvnnnp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kaedetfk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vizjglkw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bspghjsz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3msjdyzue.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hkplgqap.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kxahdryj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zkflvqfg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3erfxrjew.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3yrhzdhma.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrtekiue.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wgjzpwem.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3edrvdbqz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hxwevbeo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nyviwpey.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3oqozkkpw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tnxbsfjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmdbzmjg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3sqxeflzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eelbgysj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qmqjqzcn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3glzytokp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryirjicp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dputhidv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3msxhswbi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3orbnndod.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3cughwydh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3fxswuvgh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3icxfxmtz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3watsevet.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3zguyyvmz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mcethsby.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zttgshob.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kddmvomf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3nppeqfqi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3qzacpsmf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3txsfiuuf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mqgbhukf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vmwxjett.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3fopugeaq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzirwcaj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3npqvcucd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bduqifzm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3bbnluimk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3veytbzkt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3wduvmfhp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3vsddhseh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3xlshmgjk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3kakafcdr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3fwwoekfg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qikqdhiv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ycldewsk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3khxhobgt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3yzijnydc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gupvrmkd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wzkrkmyd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3tlthcjps.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3duepefim.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3rerogajj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zfvbcupw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ejzjvdhs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3cnpdhfqk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3sdzpufzl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3umtzjptf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3tzkoybgx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3rwcmyqco.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3utumyjtp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3aezxktqr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uyxecbxb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kqvahnlh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jhftgdwu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ztpkhhfo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lryhtsrb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ghkidcuf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3nfqacetz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3xfjwdref.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3oyjrmuqm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3oybybtym.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3noxctcac.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3uhclqejk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3trzrzfpm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3keteumya.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3shkrjdbo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3gryneeiz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3bvkcocru.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3izyqrfxt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjdylwde.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jzhsvbxw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pncqtchx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jrikafjc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3eoeeuumk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pttudmiy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3baszsqac.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wwmndufa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppmfauvk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3anveqzft.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ywudaiti.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3aanvfxpr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3udyrcukp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nruugcbo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qtvwliuu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jaldjiqd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3miwhqtys.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3hkqawqco.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ediyyiwz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3sbnasxcr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rzbcaqjq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3voglvynb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3unoedfch.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gpiqawcw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3qekabzei.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3eqagocbl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3fwltljps.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vfpnosku.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3zfnscxbw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3pgmifius.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3jvbsdtmb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rzewjxre.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bwnpbbie.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3nvazgiik.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ohjjddmp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lrzfwiln.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3swvyesct.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uxalpdtw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3jttuzafe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3araiuvjt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3vcumlpyr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3yhrkygbs.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rqfltifv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bkzfzami.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhryqcch.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3udcqswuq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jufwbmwi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuixcdog.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3yxlpqous.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3zfcrrvul.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3sogyksbx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3pdybnyzv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3gclmhdoj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hscenvsq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vpcvgopy.html


<!-- 参考信息 -->