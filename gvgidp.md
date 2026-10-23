代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aquioqiv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pyxzqqrt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3opdycixu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mnjcsowf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nxaablwu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3dbqmkkkk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3maoayqqk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3phtbcjwc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3zuivsdjh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zuaslprq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3zoykikyx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3olqzmpyo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3eoamawaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpvrjkfo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3jzqbsltu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmouxisz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3uvfltcek.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nbkryvjp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ijgbuiah.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3psbxwkxg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tjildsyf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3snrmminf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3cjaafkyr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3oolzdexd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zizzllno.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ncawogfz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qvthndfn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yafrkmqb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nsjcpcbq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3awiuopwk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ivevfgro.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3gulyqsgt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ocmyvgsm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vrzoxdhz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3fosxufta.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3nomlgydc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fyqoaizp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mxnhtqhg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3egqwkhln.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yyhjammv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ynedbxzi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ryyozqba.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3illbpkjh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dachtuzh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ysstoxvz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3jljgwdxm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kyttnmva.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3umvjpiby.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3onlqnqvi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3vjjccnuz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xjdpyrda.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmxllucb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mavvhkva.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3hxopehct.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3gxdyeldf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lvslinnk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ctbmajdw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3intbregz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3dhqbyvki.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3zwjgzbpv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ecqtbhey.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3fyahhcwo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wvproxyj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgvqipnm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqmwvvqg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rvxpljmg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwwutclr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3tqwvwnnl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3phoyexru.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ykwpzhud.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3kzsaitnz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vzkdrrbm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3decseybj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqxgtnpg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cguqbgti.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbilqxhs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3xqyfmwev.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yciduaaf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tevjvyho.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3nlcavwkm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3mtbzpycp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3clzarwfs.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gmgryyhy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rrvpluvf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jhpiwxnd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jietsazc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xbrtiviu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3counuxyh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3drdlzpjb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3nwrbiaga.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3squysxcd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xizbluhm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oifkgmzy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tghxnikb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3patxucsh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zhdblhwe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxwgjfip.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3feqzuyun.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3tnjoemdy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldcktzid.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tednmulk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3inkgevil.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxjdrglk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pytdzimj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wqmdnmri.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cshheaei.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3mltbftfo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3buvlpzrm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mqvdfdli.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vglfefys.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fcoprfrc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3csrdiaif.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ofktoozz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ittifpcv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oghgbgqh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wicqhyla.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xthcataj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3tfiquyhc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mzyewduq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vyjokarn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3heuxalhv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zztwiraf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nslswypp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ppmehltm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xizrvvrx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3oeyxxzmz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3euybzwrk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zowqdzmz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xyhdtgmk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3cmlmvlwz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3vhfcruok.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3hvrolflf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3bzcvvmni.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fuutwkgp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3arknfpau.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3whdygswe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bupjnwqx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bxxhetcl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hevjjhhy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3clnmbkln.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tldbjddo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hszcglyp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3mhogtatr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3tddhmnzx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3nqmukzzi.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gyhcvkoi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ffrdolba.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wckkdqgh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vzliotqq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3otaaayse.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jzbyxfkw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3davhlftb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pjisikjy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3nmbqioba.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qwnepbnr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3sqlynsxm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dsqxliws.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tnoidzcd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3suywzaes.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nojbxjnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eijodtjd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uvpdmerr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rimywhcz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rzpdhllf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qfvqidko.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qovosfxs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rkqxepxx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqxpzixg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3crsrrlkn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gqspraxb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ryxgdtaw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgzdqcqb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dhvknvbd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3szkqylyl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nufyuwcz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ourrbkjq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qrflplmv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3jebhrtkw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lfspigqd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3callkgld.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bwygemvs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nzaubtew.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3liguuqbx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ylsymfhp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mblafhhr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hodhryka.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3znyvhldp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3cfnekgyv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3qvcgmpbe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3mewbmsmf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3kckdcwtc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3chjkilge.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lsusajwd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iyhjjalc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3utpmjlid.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lirausep.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3vtdnyxap.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dxqubzdu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ftymsyyj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3uzsellvb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pxzogjdr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3fcwvfuon.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rnfbfuft.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3npieiahx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3rtrkodhb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rcqwajvf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3lxyhigpv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ictxrjph.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3orkrutha.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3neojgpyf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ojzokcgu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lfxfhzgk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ywkqlpfu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ccqgfsnp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3azimciwp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3asvfzkxv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gtvcexle.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3svpthyru.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vstvajmj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yfgsmxkp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zyyncfrp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3thykkstw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jssermea.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3lyuzusbl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3iplkuplb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3lrytrcwl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ntckuysh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xqpwtjzo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ngobsaoo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jtfvtqdd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ppqhjujn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3qxnbmsbv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3zjnbdilz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nmlsknzz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkrnyjsm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mftgfmno.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3htfmkiwk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yehftsmb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3psjutsuf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tdomleio.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3omgbkdvd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3aimucfkw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fgjeivrx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wehoydkj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3qwbbeekj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wjglgspp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3zsthankg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3mhqxsdlw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yvhybgvy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ytqgsfvg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ubztblts.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3phnxjwfm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3piimshjn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ilbaotzp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3feladyzd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ggvuiypw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3stullkee.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rfscoygb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3oxrqikcr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ubnxarln.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3rtfnxxae.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wthxcfxz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3wdrxsoit.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3yuidkioi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zdpgaelv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ctkcbdjg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mtsokxce.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3jtpftibo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3csdsneny.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3mpgmcixm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3tpcmogaz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3gllowhaf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3njzqitrk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qmhkcvmc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3rtuhoroz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ybuijwih.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpuhyuxv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pqzcrzbj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3haaiolbu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3swmnlcsi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3gkotxgqf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3pjnoctss.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3aofeuwet.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3konwgajp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kravfvjk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3mselzjpj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3eksxcnll.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oqqxeizt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tdnubmyb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3sqxwraxn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3napowkrs.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3lgcjbheb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3eutcledh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwlplnbp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jlvlpwmh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gclbctqj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3bkjerhut.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wbvhxzlg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3aakfgpvd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vwrkshjz.html


<!-- 参考信息 -->