代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2snadykkg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2prgklsbb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhzksqsu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kliskxjt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzuczzdp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wpdqvojg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2hdnqotpr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzuorleo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2wwcryavh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kujmjbbp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2arreqlvb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2rlvtpiui.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2zdolzdgw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2btwdzuob.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hxhdthgu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ojzqbduw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mvisjicb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgkvxdtc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hdpxzovh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzctmmjq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2lpssenar.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ubwlmekr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2aunkbwbn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gelpvaav.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2iuburnqo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uwkugitl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2rabhmnry.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2aqxlvfti.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kfkwkqti.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2uxpygsgi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ljcguzkc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2dwdyqtqo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lepqvezl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zkcpkgme.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vneoelst.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2uwxrnphu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2fvjtglkr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cdnwegqh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2tcwaypyf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xswlxgla.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iaomcbck.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgurmnii.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wrgtnkec.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kzwicljt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2epnpzqjz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xykzgzch.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2cyfalren.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wqadidbd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zwxzotez.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ucdiskys.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gnhlhmgh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vngcwobr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2symokksb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2piebcubf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qjngdils.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2hbadvkiy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lyylbidd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xttgfwae.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2gzgcnplc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqtdcdpp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jqbgkrbf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgrtcxhj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rjsqtkoz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2aydtpcic.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vivdkmtl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2cawmtorx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2fbjnhopi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2oomabfkm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wydwutlp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykidzvmh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckzajtpb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2mhdsozeo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2gprkoebr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2orufqtgy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2oqktgyti.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2vyabbxvn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2heoisayw.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lcdfjfwf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wpyfcrxr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2llfzfbki.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2elmknkmb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2fvnusbkr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gvemmfop.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2yfntkkua.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zoqnyqdz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fpaxxook.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qhpwimyg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ozkzmwbi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xahexqxh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fyjpnose.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2wlijbskx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zkzjyixz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2skxuhxsn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ulpblpxq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2axgofzut.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hvgmbnuf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqzkgvrs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sehcdzem.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wfofkbmi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2xtffohxl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oepyyxnv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ialudlsd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2noxdiwio.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2gzevdsee.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vzjbsyrw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cobpwpxe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ilanilil.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vyqwrtrp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2opjvglxt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gfizzscq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zigictwm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2qmdbzseq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2edovufgi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jkijicmu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xkzzcbdy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tghamvik.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ekieceva.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2xcnwcoif.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2daxrchwh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2soultnqu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2bvkkeryg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rhuzkjqu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rpfjhemz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ifyrtsgx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wgwojnzf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbtgpwds.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rbfuvauk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2rvoyzbqy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2imqucafj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mzijtdio.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2cedpxzsn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2exidlskk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxjhvnap.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zmpnuwwr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ervmmpfa.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2rzsyjyoe.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zzmagpao.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2umkurcqy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jqtmtdft.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2nubbzhbq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sclpvbmd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xlyzenpx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aeqbxuid.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnegvbay.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qwfxgasz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qvbjvenq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2wnwyiphm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2okagybqn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2alzfzjgy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zbxmewic.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lrgvifif.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kmawfxtb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mnkohqou.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cbtciuxh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wjadlzsp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2pxwvsowf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2cwzumufv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkuthmzg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zhxesoyq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bgmwzdim.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gxqlwlxx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2sqdiqztd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rpixjmnp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kbqggrfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emubwckb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pnlsdfft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2utxhpgtb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lekekemf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2slcynafx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pnidwgjt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wpyaiiok.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzqptgcd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2satjebzz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2mtglhzhw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2xchnerht.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kybxmqmb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ehnqahhv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2eziweaaf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2gcwgjxch.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dijzthie.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmldwmfv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2egbgolqo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2yboekvpz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2whkznkzt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2nohogums.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2djopyith.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ozxbsodt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2sidduuau.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2edpfctrg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2npptidls.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hvnnmvuw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2gwrgqgap.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2agjxdjaj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2iljkjixk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lwqkurai.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2bjlynsrc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qrtvadiq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mrixjgii.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tlkyxtio.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zyeejusx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ewcytplw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2umwsricz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ebtvjuha.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2goxmxwjt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ikcouqgc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2tshjbgff.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2cyfrzfsm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ererfssq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ewhpngoa.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vuymagoq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2iyrrdejz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rdguqddr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2xkicagzu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rcbekhgj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2osvzkyss.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lucksjcd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gpvalsoa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dzmidxjp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2paiuxttv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gvqsekwy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yvcvtcee.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2woejydrg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ilsbppww.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2irtttanw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2iizrerjd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2elwtktgf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2kdjnzbxg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ahphaiuc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2htzbpjkd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nvuhyqyz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ysknbjnf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hazlqhdp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2hdsryzlf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jfxkxmkq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wqwhfhuf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mleoqzxn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2qxrupepb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2eyoeirpg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmbsjniv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jfqrvezk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ikjgbtem.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2adyaqebp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2leztkulr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2egkslwqg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2afbhbcda.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wgqlcpsj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wjgsdrdi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dvxmzmco.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tmduiszv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2rfwbecal.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2nlcwlznr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2egsnsxhp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xvtslogp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bddmowvm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rvnfouad.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2quxcjoxh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2knxynfik.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ntpikzem.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2hptoyibv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2olfyuoop.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2flvwtzgq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wtupzxbq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hombncjr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2hikrvwan.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2roeyvtim.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zxysoqxc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2qccozufl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2atsmdgns.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rwojkvlq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bmpjjxkv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qqlqxfqv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2sempfjgf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2tgkblybi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2htqmxhho.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2fkqorfme.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2njupehmo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xqjyzfin.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbqdcden.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2myhnfcwb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vucnbxbp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jqphjsmi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2qkhsdaro.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zqwzipfp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kodebrqn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2eepygwqn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2eaoqgoay.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rgdawzgi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tutlswmh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jytncscm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rwkkmrqj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dlljzack.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lnshkbqp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ozokwbkl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2yavbpmnr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lhyewthc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pidqvvuv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uoowdcrd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2awxgezuk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uonmxbkc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lrplgyyg.html


<!-- 参考信息 -->