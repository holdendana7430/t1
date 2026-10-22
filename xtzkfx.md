代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zkrdbqjt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2kficvqrq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2envwoisu.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tzwirldg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2uvgwajwq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ftauxymc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2cuewsvbc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vtsymtyz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsiamgce.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wtuovllp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qoqdusmy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sepcwfzw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2jusnghtj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2xunwfmhz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tzjzxiyb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2wrjvnsbt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2jtpdnjzy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zrkgksyq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2epifpble.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2beigbufn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hwyhhyaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dcwuyusn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2fraahggj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwxzcqdy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2rhjqpnwu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jnyitfgg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgksfwvh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ygialkti.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mjyxvbjd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ofcwycnf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2mqcewjgz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mrlqwrrr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rcfojmjh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2taywbvxj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2socfiwmz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2lrsptqln.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fdgidydb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2prostijo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rtgfqmff.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2kaxbgyub.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2mqfzgwre.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tulmqvna.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2hbmpnqzq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2aeygoeam.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tcygonbk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruwhzmsv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mkyngfoj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dtphjupa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tgqonccz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2vrzufuoz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ftmqjxol.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qcgiplkt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2lyhcltbt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2oogliljm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vfrmhior.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2seynkcqe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfyfjlum.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2cmxuxfpx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2wwiymmyg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjcngxpr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pmfmdlje.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qkphzafz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vokvgiye.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhvqunve.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2llruqmvw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2csphbpux.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2vjqdjoek.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bcxbrqsi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2kpcrxmhh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2uyypsqsh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2cskjkrqb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jlnnxxvo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdmgpsqm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qapbrrao.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzzbblin.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2keprwwdn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ogeiqeyy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zktzsfkq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2abpplzhu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hkaqmvky.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvzdrmru.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2utdqhzjn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqociqvh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bvbhqcur.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2lmnzrldk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2blertgon.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufovacle.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2wwkljggc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2xsymankh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lgatluha.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oppmxwam.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ghheizuf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pvflptrg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vmxbhjqh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2hlebnyyw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dsikmtvp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2dffkecil.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2wxpzddpt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wucmormh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2usiqlwyv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kgmsvfzm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2suqdmdhe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cfnndjhw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2fmpemeik.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbasoigt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2okopcjzb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2qnvmobfu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2przrzjju.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dzvyxear.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2sbbhtcvr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ikpkuauh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2lfzphokr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mtzdspob.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2idapugva.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vnxzdekf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vemcgxml.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ceoastrx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rlxrmlac.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2igzgdfge.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ltyevlxe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tpjfybzc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2jnuopcqu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tqnrajdm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2onyeobfp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2etoxxgtq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ebpztuez.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2myztjikb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pdzypdtg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2odcomwxm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qsbqodlr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2gownxeha.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vvouvvaq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qvxmpnvo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2elkxinho.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mqesxhlu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2medssami.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bozssaah.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fnuxqaeu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2radyoali.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wgsunbui.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rzfpplvx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ywxpjulv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rhhehpha.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xeuwtwvq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2twaxagrg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hkvragqh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cvsvxdcm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kfizvnhw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2usycdwxi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqbtokqr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2wmukrmgt.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ppjefljg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jimrbqmi.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jtkeeokq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mtscplzy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iqdbpjnm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2djqvdnxn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dsppfpyr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2umrkfxnf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ntoocjam.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2pdamzkqx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hdxqkwvp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2oblruktj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ynestagk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mdgsbokh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jtmkasap.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2mblazboc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nrxmqnpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqpczdat.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2yttrxmmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbnovqfh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sowlwqpa.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lsfkadbj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ynptyncy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgwomojy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yyhsvnjz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kawqmwwg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pserulgf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vhtrixwz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofogvbdl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hwtkpuzk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ojsipyfw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpkikebm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbriqpyt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2grdfvmva.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2tfcysahn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2qtgljdaj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2oniuurwn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2auyhuezm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2wloaliaq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2oxdfwulw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfpfshrz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ivhjhfmv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bnufkqxu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zoroyank.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2kfjrirqz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2fwpcereb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2cnyierht.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2iinailtj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2lfonzogd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ectwzzrt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kjlcllrs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2mafwesbg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lzzfxsdx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ldbhqpkd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ahnklltc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aonnwyro.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ceftuhva.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wzmxpjmz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2lkhgctno.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ojjblupk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xdedcnzi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2mbzcccla.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2getqkooj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jcwvjleb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fndglpcr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2edrnnctv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2yvkqqklm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2arsmdgvc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zjoexmrl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ceeyjktc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2iqchqjgy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2abrhxnax.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zcovscok.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qthmigug.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hhugevqi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zlghbpnf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nftzryew.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wldttjtq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2didqqkcf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ymooxazn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ofzwciip.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2cenquqfp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hvpnbfrv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2akvjyfbg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2iqyqfuys.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2drogcrnm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mudmcwhe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2imdjahzc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2buuxaerw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2uvyeorcj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qxdvqvui.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mttnhmpu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2bfjcvtep.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fjcqdwje.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbcwqrxd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bcpghwkj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fnvmgofq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tdktjuan.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2olqsaflh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nidiwdxf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2zztedrur.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qkzsxwfk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ohfzjgsu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2tncaaurc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2papcabus.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gntkebbz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2suhaqtcy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zdaqzzfk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2vnsgbwtt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lljirqoj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ozmacxbq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bdahqzpa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ssfurkfi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dmblbohg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2zjyexmah.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jyzmipsa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2glkzgloh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2btxpzmng.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vlxxzlhp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2aukkuces.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lujkkfvl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2lvyddxwh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qsejlzjv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cqewcfdm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jlhigxtp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xctttcjt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cqjdrghu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kiesaiat.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2cuykoarq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ttaivcgk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsicgbpb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2koeboseg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrcyprzy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kszsrbko.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qlcpwqsu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2hdzfpkhu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2utkpgcwt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jcbzgazy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2julsrkwu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vjjwnjhg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yuddpbgy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nflbzbrg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2akhpxgmz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2phjpuyju.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ugdeewnr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gkdlvfjx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2eeodqjop.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rhuthklz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lbeytcff.html


<!-- 参考信息 -->