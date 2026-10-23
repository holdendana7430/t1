代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3exveeerw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqqsqnjc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3gonhvkrh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vqsyepms.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3kwpifeag.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xczjhdbw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3yldlsghc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ihbyushk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3rizpiznx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qlwoxrtq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3vqoxjrno.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3lluyrsgx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ssoriqqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbagongt.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3nswqdtom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvaoycwr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3irgunhqr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3tjaoujay.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ochasmam.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ssbfpvnu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bltrkveb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ofepsugo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3lelhnvqs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3qccufssm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xpdrjini.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3yulepmdn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3llpoxdmx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xilgltib.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xdgyzohv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tmojqrqz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ibzgqrzu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3rfgwknog.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3kbzrfdjk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dvytxnhg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3heqefjkc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3xzfjqgds.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxblwccd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3luqpjqyj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uooyudks.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qsgvrhsu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tdyztmnk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3cbghkbfg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3unwktlkv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xwiypqrz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lqnodced.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3bcizlkxx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3amuvmsvr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lzfulnxy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3msaabczs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dlpqtmwo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3psbddtdg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3cppovnbx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vloskkcm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jrdjcqvp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3mhvqialy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kgorgzyz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vurfhfua.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogjecuin.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3safqajdm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ofwjvkag.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxcweblf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bdpoetuw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qaormyfg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3elsqypwe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mttqgtqg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jvecbcmy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysutwokm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3pvxdsxlf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3sdfetasb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpydiqia.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3agvwlnmn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3jcafkzhp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjxvvipv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qauqriqf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rbngjovm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ziukcweg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jgsrnuwg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3aakfncuy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjiosvaw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3uaqecxmm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3uufpmbmi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bqzptzjk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ndlotcgo.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3edzdpsvm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hwcodfjr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kjssnkpz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3bombqblh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3owvafgjl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3kcswadbv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3tmqnfeez.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkjrrjld.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ldjkesma.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppjxrrae.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jyrsrknd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fxhwcyyq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3kxfewfki.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3crvtsqmc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3jyukyhrf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3rytxrymx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvcdeuhx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ukvmryca.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pzydgxss.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wywlwuek.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3dcbbvgrr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cotkfxwr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxzxqgdy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3igicdiof.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3rrghwplj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ldfniqqu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3plobydty.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dyrspxar.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wnyagrwz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3eefbgand.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pqmmopmv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nbfdkflm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3yxhardpw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3msjbxkan.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hxubgqjp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hmsdftyp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fjfjupuu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bngmlzsf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qmvdyvir.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xggwhgqi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3kbcdwmoo.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xwsgpyek.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3sbzfbfga.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3dzfwzndq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sxhridfa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cpcmhqgm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mhxtjbit.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ylhburqp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3bkyfpesn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gqklobii.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vczxahdx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3abinygwk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ixotpuji.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3butusaeg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urjsckkz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lrpsxxic.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3umgpowoe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ptgibdnx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xauzqgwf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3umilwvei.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3hufwdqhf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ncprnwcm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ntharlbl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3drwabbpd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gxpgpgxp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yiejhyjr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xrfqzkcx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3itelkuve.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nybhbhex.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ejyilxpu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3grzdntdo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vgyadzxj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3thmrqqga.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tyllgroq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bhaibgsk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3qbdrttst.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3segmxauc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcjvwqaf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3pedgsmaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3piqwnihy.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fgzudjei.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ebkonqlk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnixpadv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlsnxbum.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdzdpcjr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ygonmsxu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xncgihxm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wvedhhgj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbdxyyuy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sehscpky.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qoensupl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3niahlyqc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yauxxyvl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlgvvhdq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zyptbgoj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ybghxbpc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3qzychcbe.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3pdserwdl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3dipthzpp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3scwzvjbq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qqlwxehf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yoqxcsui.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqxqlpfj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vjxsjyqi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gsgewrwq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3nwpxeots.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3fahcrnpn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3uwhwjfpg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3iqiptaej.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xxxewjet.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3whoithkm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3dvxzuuqu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mvkffzop.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fxllrvag.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3koqshmyl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bcbiqypo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3nvhuqcbd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dcrmxetr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3tfwnvlyt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hpyyfcqt.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dpgqimro.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3kwsplpmi.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mkvjwxda.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3aqnbfvhk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3gipsgbfb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fxfrwpbd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3kjssqcbi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3edsytokt.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jcsipdhk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wfljwknh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ujnopxwx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ghkfnxny.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wmmzrbnw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yqeittto.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3qlbfgddm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3bxeiooul.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3arnmtgic.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ixgxbqff.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3dwclwsuk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3yrwgczgs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3uiznstum.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3bvolyusx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wngujyfc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3osmzvkns.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3yffmbzkv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtygzjwl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3stzisjlo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcqdaohc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3buxozbzx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3faepsxoy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xitmryhd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3foohclds.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3byjxsxuz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gygzldgj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwhbelgi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ctyinvvf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jwcbcvzm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ooureyzm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3qwnjloch.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bighpdpv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yyvybfjn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3mwxunobx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3plkgvjlw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3hnsywxdu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rjqxiipn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ptghsukc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kgaqplns.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lhkmyyki.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mjweocpx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3usvvamxm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3wjobcqpe.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3mnnsslvn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3sznpohhq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lrnchvex.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3edydeikb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3pbxmdmot.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3juweuabc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ioumsvnu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3yjsgypos.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3choqdyof.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dvnrrani.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3tjmweesf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cjkpxwxj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xforurcd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fkxhooyc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pwbmdgnu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3eubgtzfk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3nvccvref.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3axovdeiy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kyfmvzbj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kwflwuus.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3jjrdmlsm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sslfbpah.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fevaares.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3syewmata.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3joyofncf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ixhfwsti.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3usujuzou.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dfeolwqf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3chadkerp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bbggjygl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvevmprz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3fefrqcxp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3okhecnoq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gysxphgd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3podshdbw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3htumnvin.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wamnhlyk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3fbtxczrn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dvinncoq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3vpehjleh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3anlsielf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lwfrvlyr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3udrxigan.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3uwqhjxwv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3bohigstb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3eysugphu.html


<!-- 参考信息 -->