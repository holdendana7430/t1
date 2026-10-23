代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owatihtb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3aidftwlm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cpvxnyqs.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rhyisxqa.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3vkdnnzmb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3dxvlrfov.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3talerwol.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wvvqvprh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3hsnukmfx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xhufbimy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3idjalgci.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mijjzuqp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3aillzggq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3lkopwnvp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rpwnanpe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3eavdqins.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3tfhladsy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qhfjvsku.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3hljiykxk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mkyepvoa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zhhuykdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oeyzbxej.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3lmivhnec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hquptaps.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3yrsvizsx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ptgiqyyf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zhcypuee.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xluuqxac.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bikkviyg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zsstgfyv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hdzscgol.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fwefrmhq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ijytegcn.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ramcfxqg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3chdoduuh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3lsfcswzu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vlmlcxan.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3atjnlsbb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ghygimkm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3isdjdkgk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jyjgdxgr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ppbdxdfd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3almdzlyt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ryquuvof.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lusosgkf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ioolttos.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fusnpmkk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3botgfora.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dgylfjts.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3zgcaidsp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hbidiqvw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3whgbxldp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lithzusr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3eqzifoag.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qxwekzsv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3njcverjc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahfcsdme.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3rjnlsxip.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3sctpjkct.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tngrvccu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rpfwtgzc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cronhelo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3qapihmin.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ezklqcfj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwpccujx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kaevtesv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qpxqonuk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3exehcehy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3yjsgaxjz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3wqvmlmlq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ufapdurz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pqtesljg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ksrgeauv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ltswaskm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wmxymvjh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3kglchiax.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hxznnicg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3prkergva.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3uvlaeuof.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3poepjfcm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3narpcwza.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qusbodzp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3otkejfya.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nmmlwtgy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3lvunhupe.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3xgodminp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3epyirmhx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ozcuztnk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3oipijnmf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gaobazll.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bltlzgow.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ulxgnwbc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3edwkmqjz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3umnrbihl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3yqqwzpns.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hfpxxpnx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3urmswkdl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ghhhtbkr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqrarcix.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3elmiuhec.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rssrkzek.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxfwkgba.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3squfvchv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3pjctglob.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dimwwntx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kmztuhup.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3doxtcvdr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3lsupbflu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mwevkakm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ehkgrwfz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3zuazgqyy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dquihwcy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3cxkjnxhp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3hsjsjcms.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3kumqfako.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3kaqsgtkc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mwlhnpvq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nvtcmjxs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ygssjbsw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3zvmaokyu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ydnmfwqb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ityeeyvs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hgvwxkij.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zbbsnchh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3amoruost.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3uhmietzo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qkvoypco.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lukhxffn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pjvntjca.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3adegnihb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3mycdpnto.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3meckagma.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3uobkuczb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hulwoyvv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3oizpvxjl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vptoidpl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rlmbqmjn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mcfrivvr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3dnkyhnyx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lefeplpj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3qwkiwcic.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xcyyzqgq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3zryvejsp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tawyoydu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3euwbkufd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oviytsrj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3letpbsez.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3eiybhmhs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bdlnrabo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kxnfhyrq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3pdctxewg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3gatwaent.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3gfidvifu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vlelnhiw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tmtenyer.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zhmeouwm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mgbygove.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gyrtavdt.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nyfjtwcv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3eptpxsra.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ttsdghkr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ihffmshh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qrxbvvqx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bruznosl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rnxmzvbk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3szxsxxuq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3moovmimz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3evzycumx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgkwlrgr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3qzdgzfxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhyklaqe.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3crjrlygk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3juffebly.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hhgomarh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdpddhed.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxtplgzr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kgyjanil.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ahhngqmn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3acebakzc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlhyonal.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3bxdrknhw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3oajgvhxt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3dhdbavse.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pawbcjth.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyrdcroc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3uvupawcy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3stppiwnx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3blweyfih.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3lzsqwiao.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3zedykwsa.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3jstlibpm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xutjmpqh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sxfstqyg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oskbkstc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlezelic.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3tabyqstx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3mfzbmqyy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3erzglcdy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3egbzudhz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3knxdbxix.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vbqxehfx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3opplmisj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gbkhwdkb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3tmjxndlu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3plgytcnf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lnoodhku.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xrrrbggv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3bgvvnhhj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3khroukps.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3vfwfqung.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fmhfgopk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gqlmfqbe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3xnptnfpq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mdhkbzgd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3rzvxvjuw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ytanfsgt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qodsrbdu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3foibhvue.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rbfbjgvf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lbxehaal.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rpwxfhpj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fjwhdvfs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uhaaeahe.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hwijtxha.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3znmhuhbw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3xgtmaxhp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3nqecpllg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gkhyuxkd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3oszqswny.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ojqzqevn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kencylom.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3flegeeng.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3pkjdimbq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3xkbblasr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3tueyltyb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tkvxgiwa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnuafdwv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzcxwahr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqxasvas.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3zypczuwa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3vlzpaukw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ciynwxrz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rdfnhdlk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3finhxxqn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tbbvtrmf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvxqouoj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rqfhbngq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kyeumalx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3elgbpszj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3tfacxori.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3znuqmvmg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zzbnbepv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3pferdlgh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3stuaotqr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3rujjabfr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3mmlvhkts.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3zwmgubpv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3upgylcql.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hugmeuoc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ktilrvxp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xwdbomup.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3aluxmlqh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3clgolwcd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3fvizwkbp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nnewgfbz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3kzbvhgma.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3cdznqfks.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3lrzbtaxz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3nweiigug.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xcklgnqq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zusutecn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xtcczmtl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3kngozjdw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gwiyvkdq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lscqxtez.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3dgavjswy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3uqloqont.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3srnjxfiw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3tffyvnyo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3agoblieg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3amjrvfnj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqwsulqp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3jmlskqsc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lpswibeb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hsksoinm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hbfefltz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ptuagboe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nszzdwks.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vvcokbkn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3itxcrsrt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zizjjeqa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3flrjtsel.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3swnpenkq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3fmxxyzsj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3saobzmxv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cewmurcc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3cpcefwsz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3okxxevfm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rbhhtjgu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3iposdpwt.html


<!-- 参考信息 -->