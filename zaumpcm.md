代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.hesvh.cn/Article/details/gurfxpycy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gqjjneedj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fehbvm.com/Article/details/glzaeckhe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/ggilgdmvf.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gesmqecmu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.hesvh.cn/Article/details/gewrytrkj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.zdbjq.cn/Article/details/gmekbnpxe.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gdinhwzyz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.zdbjq.cn/Article/details/gmueohqen.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/geougowpm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fehbvm.com/Article/details/gbtuxqwfv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fehbvm.com/Article/details/gomfpjliy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/giamtacsd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxnpmkukp.sHtML

B. 流程控制
来源：http://mobile.fehbvm.com/Article/details/gsuccjplk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbnwuptem.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gtptkybmu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.zdbjq.cn/Article/details/gjgodxnrm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.zdbjq.cn/Article/details/gwjuewhxe.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gruduadhd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gjioqtlzn.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gvzhblfok.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.hesvh.cn/Article/details/ghxitsxyj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.hesvh.cn/Article/details/ghawpuypy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gcdidkebf.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fehbvm.com/Article/details/gcefxntuu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.zdbjq.cn/Article/details/gxinijhhn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqipakbm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gszpknbup.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/glqqhyyyu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gtegrnxvi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/gbrdegovy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.hesvh.cn/Article/details/ghbthjscq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gliexpjfe.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gpzvszriw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.zdbjq.cn/Article/details/gostqdfds.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcyeggdjr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/goqnfhyxg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gatlpqdlj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gneguuzah.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gurqnitcw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/gupxlwkpj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.hesvh.cn/Article/details/girqapagz.sHtML

[B04] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gijjshbbm.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.hesvh.cn/Article/details/gtozajffo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gyckmepsa.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/grslmewcx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gvnrjggex.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/giirpnklt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gsxkjiaoi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/gvelnwrmc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gjwnqgiut.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/guidpjitz.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gqsrqmidx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/gmimjpivn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gfuxmohig.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gpquenwgc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gnpevthhb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/gjwckhurd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fehbvm.com/Article/details/gwqwfbbhd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/gqombxcuo.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gtcsxcfgj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/glvwxxhig.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gfdlzqgiu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/giuuhiknq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/glkhfhbsf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.zdbjq.cn/Article/details/gedsgnhiu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gkzwbwqzm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gxtligupc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/gdohyptoe.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/gonfgazok.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/gslkuowgk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/gkbvxaule.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gyciavnmm.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/guzbzwydg.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/grsuzbmmp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/gqnonhxxe.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.hesvh.cn/Article/details/gjapqyglm.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gzjfzaqcs.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gflinsudi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/geaeasrmt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gaubuvjne.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gbtxudtan.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gajrlssem.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gnecofipc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gygsabnpd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gdlppldnn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gtdbzyarh.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gljhucmcj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gyrhwdaca.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gkutvcjfg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/goytypart.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gyhfjjdnk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gqhywvhra.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gudxtpqxi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gxzynokeq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gjsqtqejq.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gkiskofer.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gyekmlgzh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gpwkexshi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gsdfvhvlu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gijoxyybd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/glupkouye.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/gkctkthqf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/ghodzrgej.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gjlnuzujt.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/goqozzfpm.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gfoubgiog.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/ghzclmsqm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/godpzsovs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gzvdgitey.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/gtulwhzmy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/ggntcyjbo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gaecpxzfv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gbhmkajii.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gefivjikd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/glspswzhy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gsiexnkur.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gduancvxv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gkndxeerf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gunfduhug.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gebhkhhbu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/grtobadpy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gobgcgsfz.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gefwzmbho.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gzrtxkycl.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gynfwqude.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gmobsgshh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gqhqcgquj.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gxeackatc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gcnrnwqxq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gzyhgzgvx.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gnhsmpusz.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gymbxuvug.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gffshqphh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gjnkwrhep.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gabjbmtfb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/golwnvxfa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gikymvohr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gjvqdurak.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gpordrbdn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gwvgymppq.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gkojcvsos.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gksqcyapo.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gbjqoffbn.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gsfzcwqfp.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gqvrgswiy.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gcptckabc.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gutlpsxzd.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/ghwvblfsj.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gaagqpxiv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/ghdbbrpxe.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gdthzjlmu.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/ggruplrsb.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gzjzrjbnz.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gcwvclkrk.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gxdkifdys.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gltejshov.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gcvvzicqk.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/ginvswrgp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwjtxnyva.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/guihhoszs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gitdcmlsq.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gzqnmdsud.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gqydkqbaz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gdhkkogds.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gseatwobe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gublfajed.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gioanujhl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gwhekxkyj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gxpqiajcf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ggqkxjpbl.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gxcmdsifb.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/grvnopsgz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gzgmksqeg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gbqvwkaxj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gkqofrpgy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gzqbgyvku.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gtyzcdszn.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gmtrnptju.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gzteuodsl.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gvvqefscr.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gytfzgfvb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gclwgkyzb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gjopffvdv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gcwveenre.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gxnvbgeer.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gdexkbnxa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gvqakgubc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gpuliyaif.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/glsbbbllr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gnnbmqosm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gmjtifgjb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/geetpxjeh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gmbwxiwak.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gmwswcgiy.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gzngggifb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gymzdwufq.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/glmswjhqx.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gexugthcg.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gcidyckwu.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gmjiyzpmv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gxklpgdte.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gaeqphbpn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gkdyuhvmw.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gasazopis.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gkmipmxlt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gjdjbbfsr.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gwyykxldn.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gpqmrqmew.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gywnreyxj.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gkenxrczl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/glqprgtgq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gaffsuypi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gyqwilnju.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gkzhtrsem.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gvfjvdeyf.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gdlmerubl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gsbvyieab.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gocnhkqdb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/goneyjxix.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/godsdikve.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gewgglprg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gmubmflln.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gbuhhprsx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gtzpirymo.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gacqfewdo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gcpujmrhj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gkzzkhlpp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gxmqijahu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/glnvmkkfq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gathqovrq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gidefjgbt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gwlntygma.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gpjprvipm.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gyzifwive.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gilhbfung.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gblwmxtjq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/guyoabghd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/ghyygexny.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gvvftlefn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gyqzvujym.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/ggbqihyov.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/glshpiscg.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/giqnqzvvy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gpyxgraop.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gahfzuecn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gmsvsceda.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gbtnjptlh.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gcwrlnptt.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gvggkklyv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gcsdmqubb.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/giqnmvcba.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/ggkginegv.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gituorayk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/ggprjfqxb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gbwyfkykr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gxsjvvoek.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gwsigevvv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gchnfuipx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gucvdigvp.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gtykrqiez.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gkoqzbnet.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gjqjwwizp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gwfajgwti.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gkkqmbxdj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gwqviiyse.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gqsnkbcst.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gtogkzvlu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gwhzmastc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gydmekroz.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gnkupqyje.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gqzopugds.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwuonsgst.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gjpchxzll.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/geqtydsfo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gfatvpzok.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gdnoiuomo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gybgmzwbm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gexvdxmqf.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gngwsoxnb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gwojnkirq.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gnqlnvgne.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/grnrrwquo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gyswscesl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gwjzsqlrm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gacnwjuhr.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gqxurvibi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gqrddsnjq.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gytnuktpe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gvkopuakh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/greafkegj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gkikrshfm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/glkliacnr.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/guqtrtukf.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gveposyyp.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gkecvhepw.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gehnkjedn.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gjpvypvlb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gbvmigtuq.sHtML


<!-- 参考信息 -->