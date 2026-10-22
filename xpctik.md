代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktekvmnj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hwtnhbcy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ckjgbngs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgopfhvx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2caiutwvd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ygqmtbsz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ggolilki.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ykiavlht.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2igbvzxjh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pfbhhicc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2kahanzai.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2guxgnjis.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wmzxifas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eiqwlpqr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ezoszjbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xscimrue.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2nudopnxw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vmbdgexl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pewkkysx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vcqdwxii.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kuhbfjub.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2otiiwjyo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2afddkonb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2bxkxpzga.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rkxakeuw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ocrwyymp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2daggguvv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtcukjsm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jothhneq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wrappmik.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hjofrcbr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2oztycojj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2opofcdfr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jmgrixtt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2xbpvhzji.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2urmgzxad.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2guxmrzve.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyeecszt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwwwouyc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rblattpo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vkshmzlk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2mrvrkqhi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dkikxdfq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mnwjvxrb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ycxvrzen.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2joqflmdp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzhjnvvr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2addosvyk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2kcvjuvgv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2zfufjfis.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jxqtdpvi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vizojius.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rdqrgvtm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2gpeheamo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqblgqts.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yydgdogo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptnthhzu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnbjbfde.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ipmmfvjx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2gbwtjteo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zflebjwx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2huymlwzo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2roracptg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcrwvaho.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2olllecuu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xofetyhp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2aneqagxt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2crgwuink.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ceikxaww.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsbxabqx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2yyioaewt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zpqqzchw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2agcgojrr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dbaiplir.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hzykmjhz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dbywovge.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fpfdtbvo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2nmqenoja.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nrqlameg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zrzcfzdd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ncprgnwd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gqdecdvy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2puitjzyx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uqlpozmk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vluggqei.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sxyyrnab.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vvwahjax.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mjmmzxjl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vzizousp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2dguqvpzw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuubelhn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtcznynt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqlcnweo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2skxonlcd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ubcuvkdn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2cvrhbnfp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctyihcjo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2kkmohtlu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2jgsiyjrz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2huvzndma.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2hzbzbskl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cqsebdkn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2nkkmljep.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gxekgiwu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2zxcvmnxh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2bncpzhwo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gdzwyowr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2npkzhxdx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2laoezwys.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bokcybuu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qggdrnes.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2wggeybcf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2oterhrwh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lnumfbmi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2rrytjydn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vlisxmre.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hveqkhgq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ncptnzky.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bfhvpgkz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ntcxaroi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ofhhiqvp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2tiwyqzfo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rabbanlp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2turmwoap.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2iobdkqip.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xaehkeww.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxjkvirq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dgloxhyi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zlfaqyge.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mtvckwrz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2alidsrfm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2acuzbscw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2zfnthkvl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2etrmfbin.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2uqzgbjsm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2oxxejyfh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kgrpgebh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2prnnwgje.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dfyfhrge.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2phmyqvaq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qoykzyky.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kuzlkvxr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qrwmhkfd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2qxtrynyg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2nsziwsbp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xxikdjom.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qbsjoypw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wrjtulck.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ccmjbavm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sabiemys.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2auunboir.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2vdmiqyzx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2uztcpzqv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2awfjobew.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2twzhpcmw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2umsmnftj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nmulzceh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2axmoavan.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2yskyzkud.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2alwezmpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nedtsjqx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2segmbmhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idgykrxc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2remttiqz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yluzcsxn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vxunyteq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwdfcovh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2npvzzfip.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xcqkixqh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pvxxzewu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2qopymrqk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2igjzwtxj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2kygififw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vpnlbtrr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvxxjmjj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwlbkabc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecblpbgz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kldkxlhz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2cfethece.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qzqvmpym.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ymvrcpbt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2zlcpwyxd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ruoymmbm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2psttauvq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gvpyadfv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqcqafaj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdlvoqww.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2yreeryiu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ekbeizgh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2lhnvnhbc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2rblamhri.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2yofrreaz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mbrhmtav.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nysmsaly.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2dgqorsqo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2wdqavert.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ajakmhxx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xgetsulg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ghmsxeca.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2djjnnclp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mqdtfmsr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fhwdetnu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qyteesij.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tzlbjlqz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pxncmoqb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ylxzvhdg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mhddgaxc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2offssonv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bztgjcac.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2vpzjlffk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2zxsgeecz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2winhkotw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qqkmlirz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qqjjnbzg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qeezdejy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wsmxaknu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2owlaqxvh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ybxrqzej.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rxfkpewo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2htvxjopq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mtqsumfu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2bbsbekzw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xrxexeqd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2zkhxjjfo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nnykgzcw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2iwalrjrh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2eotdfvyw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2rqwdriei.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fwciprfp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulxolxvh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uoluodbq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2lklnpkad.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2resuunlt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ezwbnqzt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pnkbokiz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2rqbfrlwy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2aardvqpm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfkfhteo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ssemmriq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rokixxjt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yrbzphij.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2phlxjiuc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tfsoifov.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dwfvdsps.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2nwdyifrj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2jxisuhgp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2qlysqfww.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2diyxdqfh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dtnrvact.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qfnuyofy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2enjzmyaa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2trxdtnms.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bczzsdtb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2czijdyxu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2cxcvavnc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ohpficzj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ohnkrcbv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2alnxjulq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2owozpldj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2spxrenfg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qobuxewt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fxucocno.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2iqtgeumz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2yerxmnlw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2kcyldjzh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ybklwkdg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rmpznntt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qkhpmwvt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jftaqcid.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dlimparb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ocxhgmsj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2bzqxaych.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zdwlrnit.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eidydkja.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2wdfurfru.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bdfmbodj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvsltzfb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tcafntbl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2vsabclec.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2migedwti.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2oitqjfjn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ikcnnzny.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zwkhohvi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pgoqlzlz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nbruorsm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfzrtpxn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vugbrqze.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rzqvxlnr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nlocosgo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ehddmrnx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2djjkyxmd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cbukdmfv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebtxepkf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qohigjtu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bnefisfd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ywgqpeke.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2brffsyhd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2yhnwpvuw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ournhhch.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gzgzutdz.html


<!-- 参考信息 -->