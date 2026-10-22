代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dagklgni.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2mkatzdmu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fjxaljfc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tgoefkyl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bgoplgby.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rkofwvhw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2kgjpiraz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfohbsyk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2nxpaplgg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2rlkegrpg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2vhdyqkbu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2firpmqnb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2xkeztrmf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fkkrldra.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ithvavba.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hyuijdar.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hsojmklz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itpwgwpt.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2kxypqthp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2magobnqi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2bohzxkcs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2hmtfoedz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2leuttbve.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2oxauosot.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bbijtnfi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gidauact.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2umnuhftd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xiyhxbci.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wmznlqbz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2xbokbqdr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2wyqacnne.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2zmjlgdco.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nodgmhxt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xlcgxxff.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dcxsabyl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2hjmxoqpa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2dfmehvhd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yvmotvkc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2flzrbjhh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2jietwwaw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjlmtctz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxgmkoal.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2butohmnq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2msjpvgze.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ahnbzgcd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2onfvlivh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2eejrvkwh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ldcjyqfr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2mpxrakft.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2kpncusia.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dggorrff.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdlldbuy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xewgrwxo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2cwrlnfxb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ttrelstb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2chxzwbtj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gtldythz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2amlccshz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2apdyibyy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vszkdtpf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmcyghvv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdtellkp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2kbvavlwx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2sgasuqdl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2akghhrmd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2yyhhbrwo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ebielybx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzhreywr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lptnsjyq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2uxtvkyzn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kojiolyo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2kpdiisoe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ghnycqrh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfruzibo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2eqjdwyzq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mtpotuzq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ukequvjt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zmpvcfpf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lumzzfcg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rnhpgyia.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2jfuahwnh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bumfxawr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eufuhamt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2sqqailsl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2btsuyudw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ueaetzgm.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rapfrucn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ciodtfcm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nogzhjmu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mvtbkkyp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2tsoeyjpj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jzspzzfi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2rzshvagh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2fqbfkbhb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2anvmwfhu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bxrdzzuc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zitndnrl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvidvhtk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2soeblwss.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2vpdxwccc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hinabixd.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cqllzksd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vncuutfy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2xozndxgq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2uoudjumt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lqzkqlsk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2fnnhcqdc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2wxygtzfr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2hftnfgyq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2eqcwsxay.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2urvrmeyv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2crlhflcr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vttarvyj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iinnicsf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nijggbaf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vnvwkani.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2wacdjgel.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2unfoxrcp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2pbkmbemi.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zwlvglgb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2hxfkacgx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2qepxbohh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cbmjnneg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2coovycjp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lvryqtww.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wesmkcaw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2gyosfzmg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xclobnlk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2uvhyfgyt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xgqflobd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gsoxugdu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sxffcpmv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yltjpvex.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gehfvspx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fqenyvvw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wyorqyvo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rfrtqarc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fmuefazk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jflspvcw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ishtedak.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2drabfrbh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qvobyrgy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eqazjdbx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wkjtsesc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckkatlcr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cbsyvubc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vayvqnwz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ymiaylpc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2axqsxrbs.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pvgcarmq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mtukvjcy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vzymkpiq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qiwravzh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ygwmzgmu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xynpejey.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2twswqbsq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2rvtfptdd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2akfwaloz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yhbrsrvl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2infnaswf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2iduxntrp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hocbchyh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ugotywkp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ykmcmpco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obutjotg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2yobwxwvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twjydvym.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hvqatvdk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2cslzbfuz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzyojxbe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pthhlpyk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hanepfbz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2infzkrmy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jgbfwhae.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2tzfdcdly.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aewtbajt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2owdanwhi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2sbfwjulm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jljtgvvk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzipwncy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qyzeexrv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qdxchpzu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ypmnidzz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2eprnzmzb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2viftcdkk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2nvzvubav.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2frjdglkl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzctlxuc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kuqmfyta.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2exhbkmwb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2pjgqvqtb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qtlcbnsg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fzsibgua.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ihjqtyex.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qjkwvhcn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2zgmbzthj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2omlqvzxe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvqvnltt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2dlbenlka.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2isfvbxzn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2pvqyzkyw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pluclumw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sgohcskd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2norfethg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mpxcacoh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2bkpuutmi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hzhixcbi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wniazrnk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bltqfqby.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2sudseeen.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2exvecjta.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2aydzllrx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sdcesusc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2fygyxxcr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hnckrssz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jdugndmu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cexoroiu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2blstyqai.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xybmkkrx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2eubjovcj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ooydfzhu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ksbvrfle.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2urlqoveh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cjdhseeq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2puqrzrih.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vdbploza.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zbfblsee.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2kapxrqry.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2uvtjjszt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2zmjmytlj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qvjqbjve.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2nhhqzkyl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2pxxeebsd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ycdijzfq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyzqvuyv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2dtfmnbig.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2fyifhojj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ieaboczp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeeewntk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kgbcajvy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozbcsfom.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ovzmysgm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2javvylem.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ccawcaug.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xuidirvw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xvvcfvck.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dphqoqee.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2swysgbif.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uiodfdnx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2iyuedqso.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2iaubilyn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2waljexpz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2tzxpvfkb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lugbqjjj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bdqvclsi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2vxoojzoo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gskjhjox.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yudyyrzv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2rixciojk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2memdcemf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xtwrsrtm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2hottwowc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rjtgcncr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ecwxepqp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lrgpfroy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2quvedpbc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ngpnxola.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2njwmymmd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2yfiytvsg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bppdvxtk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2uavkvlmq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2nyoijyrd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2aorkcvtz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2tnnknndr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2uyszwtrz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2pnyrmkbc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yorvarps.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpjcnxaq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2rdhqbomb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2meklmoik.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqgfcrjd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mqwapekw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wfolqpmh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gnsbufzo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2axsplxey.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mayzmtkz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2shhiirdm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vifiqyil.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2xtqyjmev.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzhcdtvv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ihhhxrpt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wevowjjd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hntmurdz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2sucqiyag.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2fdfalfcx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uweklbuz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slgiwnzc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgbfwxkd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zhiauqzj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oegxuwjt.html


<!-- 参考信息 -->