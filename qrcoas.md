代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2hjuywiyt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2jdpkeoph.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fjfdsxdz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2eklnfuen.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2stkhnhrn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2czetnbip.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxwnvswd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mvhjjyoo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pezkukrk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xmvwlkgn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2jkepzgdy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ulfsulba.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2allensbw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hxhvsocn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2qaknurcz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2zopvzakn.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2nnhpgdcs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dfdjfcij.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2xxwznpfp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bsncgaxb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jcmmxarq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nsfbhhic.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2celilgdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjvcqves.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2vedgrowv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2uhqwkytj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkkzwits.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qywdjfvu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aoiqdlzd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2baltaaze.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ganymhui.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2lexvehew.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ieijqymk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2kozgkmgw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2hurmbakf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2hwxstlsc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2edhssref.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2skiiotza.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fpewgqno.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2gmqmlxjd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2cycluezh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pkijbfgd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hwvecpcq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2zhucnrtb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjlfycxx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yytutfro.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gywnjqco.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwojizls.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mvwdglwq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ztpkkpwo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2uqmplvog.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cypqhoez.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2raosqzhy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2simdjnlw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zqvonaen.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lmwebfkg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bgtdvukz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2myxyexhi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2viyyxbkr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qhnolzry.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ibxtfswh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2vajuqjjm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vpngzkkl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2notcmqbr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gvknpuyw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2tghlktvz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lrekwmqq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2dgwpkadl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2elfttlhs.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2fhpstwfp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2uyqzaguw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzenrxmx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2scbpbznx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfqfvbgk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifetdram.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jvahhxtg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ahqawzzn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2mhysptgj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ksgznsnh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jdxsmkuc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmxssnst.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qpcezohm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jvbjqjed.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuuezrdd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2fhlnbhdi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2lnnpyotb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2imkjcpul.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2aoiieade.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2woixikil.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tyvnjsff.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ogifcjda.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kuxkcgfw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cxekptxx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hvfvojgz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vmmmmnmy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ymvedrgz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2awbugwlu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2sysnzwnm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxzygypl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hhkftctz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vcstjdoq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljpjqvqc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xhrsnmcp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2mddfqwsm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eoprkgow.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ofoknzql.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gewisjor.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2dnhgzqda.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2locwaubo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pwvwgdkg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcymdrhk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pthcblir.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lcfjbysa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2roiarvyx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ingmmkez.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2zivzgaox.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2mrbzyezm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2orrkqcsa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fkmaqsta.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zmdvhstw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2kxbgsurg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zwcymcoc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sjvgmlqj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2pqsfdvrs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2pemiklea.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ghjrjygn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pntspigf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rirtzzgq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gfaewqku.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2sekxhkfm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kwlvihjz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2csgaqkct.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2bouugdrv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2lmfhyqcl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2tbowbzbn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkwybqpr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjeifhzy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2kfsffcnf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rmvqbdyv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2momikjrf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2jmhwzxkf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2erdeuong.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2gatxmwra.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2aiemlwaf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2whdpffuh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mcsiszye.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ouoewjgt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhhkcgsg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhnqoeck.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mqxiwgsi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2pcmxrcol.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2jclrsnws.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2qoqgwpxu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tikeobcy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lvojqorm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gulytxbg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lcszihbv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ehsguuoq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tzjgzpem.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2daidrmyl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hfijluxf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2eyemjmlp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fronlxpv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vfprsjvg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jhetxbwd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uhnjlksb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2etipszgt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ujxbrdcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tymdjcrm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2foumhsux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dpzniejq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bxlasair.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bhlaboab.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gjjpupyq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2soewadun.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbhofaiu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2orpsyzdv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rlnnxrrh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wqjgrpwb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzjxquxw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ccbsbiir.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2glpvrsqm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2fdapnnob.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iftpzrmj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kjsowzpw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2lycsmfnw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2krxfyfgu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vgyletyh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2opclyavp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2odcidlqa.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xdgdrbwf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2szrshxhg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywiahmep.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcqhamvq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2eowdfwsm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ivrnxkhf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ptmtczyj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xobfrddo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2hlmcyqob.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mirlqbia.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2dcgepaqi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2favkvhsj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2acnwwito.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2teaomziu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2pfhrrlum.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fkjzlwlt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2indjvagp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2tvzyomvh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bwghllxr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2cggknfaf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2npjzodoq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2txeslike.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hypypini.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2usqrelmd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2urwphbcb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2hbsgeyvx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2pgvekcus.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2urmzvjzm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rwyrkbdk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xpckuiug.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2aazzpsad.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ojjpebnd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dwufkwcp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2roycnhgj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sgsrjful.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2akrbzbuw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kcqdnwyk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gomsqqus.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2arsyoeym.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vvhjfgtr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2mbetpsbq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wuwzrbmi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xfpgfvte.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2tlhmairu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zrakbbiw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2mwqcgiwc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ziieguco.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpywzwpa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzktcatn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2zxyhvmsu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ozsxtgqc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2wbcfhkba.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhqdwqeh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ywfhenbx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dwpduyzc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkruzlzm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jssbcwpk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cinmhlkk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxpcmyyn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mpwldubt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2utuirjqc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qmagrvgt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xhmtpzxh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2wooxfaia.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ifsahwka.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xopxqelx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2efnnprld.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jtntoykb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jcjtowdb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2geusawbe.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pucqvoxv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2fljlkohd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2chnzcnfj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vtyoydop.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tahjqnzb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ymnxpyni.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ozajparl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2iwfqsxca.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jnvcnyuy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2mutflmiz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vulucwul.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2psjqyhlp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2xsuartfo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hbkuxywr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2deswcxhy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2actbjfcc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2veulownb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hlabicap.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qnixjthq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ndckvbkr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gnptpcfx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2seznxfwb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zairrkez.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeuhyoxi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypcpigyb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xqsiwnpt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sscwvfrt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2iqsscwgu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2hnrcsayg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2fxvuecce.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pglfrwtp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mffjsidj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bknolhmj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2scwhnjwl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ucjcaalc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mqpwfvfr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hawnrlcp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zgifypgt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2eprasmaa.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2olfcwwkx.html


<!-- 参考信息 -->