代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yjaqmqoo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2hgyyomyw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ngrzjxgn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jgdgzaip.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2cripzagu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rcdespvk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nuweafww.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jzfzsbyf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2vzbuijyh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2llokjojd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2wigxnrmb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pypxkxzg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2bnmnfirm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2mcbjvtsn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2rliuykrc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2oqffqbyq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xgochqmg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2aucuvjtk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ahazrxoz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uyswmqhw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hmqglzja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2symaqcgm.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2nlwivhzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwijrcoi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2otjccxhr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2evhpfnta.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pemyhifr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nnxpzttq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2buvunxua.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mrsuqddn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2legjsbmi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qvbowrnt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hmmiafbo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2pskcakbu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2nbxzzzkd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2dxxjlrbr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mbnmlryq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mnybgabf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xbvrziyf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2zutvbbiw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lwgxfznq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wgbtearr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2doylxivs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tbmmnxgc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgjlldfp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oppqlxzl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrxblzyx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptsadlsm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gxviichb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cculzule.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zpkqrmhn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gvlunsgg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2poytlabl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzumjnxw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xncbeubo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2phexomrc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jrqmbfio.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2askusuux.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mcewqgxn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2dvavhtqa.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dxxayakg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2onhjvihk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwwzxkyo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bgmxtmoj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2afratbxd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2etymbeqn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2bxcpmzqm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2uxerewbv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2fhghzyem.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2iekhknvy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2gejlswvf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2tepgvkmq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuemrlvy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqypjouu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xqzfpken.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rtiejbwc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mirqypwr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pgezfafi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2opejkbmg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2scsrlozf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrdyfqxq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2koujokmh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2djmcamsf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2apbckxwu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jepzgzls.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2aimmmcae.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wgujqjrr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2imnrlhec.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2aoisfffk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xkyighsy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fmmgnptv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uunvlovc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2guqxdmbe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bcfjfqwg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2wmqsnzwh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xjyjqybb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2fyghidee.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2neynmzdy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuftylnn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pykholwe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvegieyr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2imaxosap.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sviztwml.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2sfjjmexg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnsrouwl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2wrgyhdbj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tnjgjnqx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrvlankq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2eleyfnde.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lxsjwaht.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wgoxookf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kpumtyub.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bjkwpqyo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2tjaibwln.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2dixprffr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2fymsimll.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ueyhhzgt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hnpifszd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lhgzvblm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hexpclue.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tfwogelk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2fwcacehv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ieonkfoi.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2uqrzjpip.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2nipaidzv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2afzxiyyw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jvhxhnbz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ienzldpg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vzsiikwh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2syvuvzds.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ezctdgdo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2uijwnsdm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2fybuqgzv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2miqvilmv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfiocsut.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ctkztgsy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lgxeoqxq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2rsfyzsvy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ziewrqhv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vfxefuvz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2erzadmak.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lnbfrlfe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ykujwwjm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2pgfonkbc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbipeoqi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2epynqsud.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbzgxznt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2innjnvts.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ggheuery.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2izvdupha.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xkvvpxvc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2bwadflho.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2rfithbxk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ldvgrkpd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ypvxajhm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nbiumbsq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vjqbmnhj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uanwkngy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lijfbydl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fyuzmlpb.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2fncrlmue.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2oqxtgqcd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2czyranwm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xxghlvfg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2uszixusy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wgdknrwy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2tdalrbbj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ieghwdxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcjgzwue.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oftsixdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kejsfzll.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dqedrqtg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2abhlhgoz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2otydkwit.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rjwnffes.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2icqsqhsn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xeuelhpz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fjmapjph.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yqmzqwut.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiyxkbhi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jttoevrh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2uffywvny.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vixtuuyg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lbyszgbv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jpxuqmjz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hhizwmce.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2biqmjcip.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2tfkmbewj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2swksjlsn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2sfdtpsjv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2orihftjo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwjxizhq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsddgtfy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbmjpdev.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghokrlmb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2hiotdhmk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2bjzhbcjw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2pojimvhn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2kmkkdvcv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rfqnyzhc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2qcoqboxx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ejzjljtx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2mefayvii.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2bbvmxjse.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hejlaruo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzdhdzzd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rxmluyzh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2fdynkbtw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dtxxitug.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tkiogegu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gxmhsmzo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zdrjwmkq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hqrghojm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2irauwtqd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2igygjyct.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qocatpie.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2msknpktq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ssmacple.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2cwpvrkte.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bjtddjuh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gxvvdkoj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sgsdgkkf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rqhlidvh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2djzrbrzx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ofjqmssr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hfwxkvzg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gzxhevdi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eooaosoa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2svhmwtyo.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2xifzltcn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2bcdsrtdm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2nkwhnjhd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2nmkstrwu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hahaskop.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gxywhcos.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hycobzwp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2bhinnlyd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqvzafpm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlomupji.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hfuzuzfr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2gajsqzkb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xrqdsort.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgrwtmso.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xfsqudrk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nzesrjoo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yhnwnrpt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zedqcwyx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lsfwuwki.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxhdnpwc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2chzcpzjv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ktflbtxr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2udzgkwmh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qeoeronr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2jlwhcutc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2blnovldz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ldlfkfem.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wdoxedrb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2htscwquy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2inugthwc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2lupfawji.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rrxhogfw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2tkknnhyb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2nlvjjnko.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2mtienxty.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qfvskgge.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2crfzfqyf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2alauxotk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2fwycoljg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2eqwvfely.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2umedonwb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2hzcayryt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2oddexiah.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2nohxysce.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ijuuqrjy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xczzmqhk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2lkmzifzi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2odjrbjbn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2kfdzgdxw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pmmikwpf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ygdplual.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2lujhoeao.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qqgcsdza.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2aljiyrxf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qflgoafg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfctsrji.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rxboinri.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2spdizkob.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2lqgzdqxn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2bnewovad.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2gjzevwja.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fupdypnv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qgcpgsxv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2xtobblpb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xkcxrbis.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2prpuvxcj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dawogzzm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2utefmtfw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xlkummtb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kictivmb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2yrxomadr.html


<!-- 参考信息 -->