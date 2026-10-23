代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nsqqatfh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3hbdyovcu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gkjulknz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qnohsiqd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3rfbnjmnj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfvhmjrn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlcwulub.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rcqdzveb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3luitczhw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbtoubav.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ibcwptuq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3depbqdsy.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3owwdzbha.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3kncnprxs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3lbphhlxh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3kpghnmki.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3jajvvynf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ucsusnbj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ajzhwasc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3whodtslk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ghdwuohr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycffapaz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3zlsgwwhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpdjldji.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3zhjbansh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fthstybc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjpoyslg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3somsodjv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iwdolfyq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3paxyqhgy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3eyytwvba.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xjinowcx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rpkugdfc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3rmjjdrdr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ilgcvdfh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncuaayds.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wvneuihg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kszsrsji.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rjhbdaui.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3konphght.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zpfjjsdg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3httpufvp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3lwqdtozf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3gjgezcot.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3veyijlsp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ftkrsajd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcmzjfqw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3obevjexy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3swokuinu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3vwjfijnk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nsgzxtub.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gxvwowwk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ptcuuyqi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3yrunaxbl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqmcnukb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3abtgfash.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3iwzpebll.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3pwuqlrgg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3livvzuew.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ntqpmcei.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3oisqbbdd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bjrwldnu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3flgzyddi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wevjflcf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kaiaxznv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3cnxijeqy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mdnbztem.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3rnzqczxr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3efvuxjhl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3tmusqibi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ldjiwjum.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfxizsma.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lucdigrk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3oiwwsmcs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3agjjomwh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3wszvyunj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3koklxpnm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hloymwsv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hqdxxzjd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vpljqmqe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ksypqazc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yjlbzgnk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3prwscwdo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3llwckizq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3headardc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ihxfdtfw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zpycvtly.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3odadblgp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3derbxqht.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qrhoamcr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yfgrchof.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kqtyadbr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lapqdtoc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vzqjustm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ihrzakqf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dvnrcsro.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3lgbapqni.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3jrwotafd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rvbwcobk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mlmgqrhf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsrwatxh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pkbokpbo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hhsmbges.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qvpohgci.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzwjldvc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ryvcosvi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3lzhzuvil.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggocpeqm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pkwbxfwn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3smrerrkw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3zmajffqv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3nqmslmrm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3djisbhcy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3voasafrl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3sbrgvibr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wwbcldjx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ekjejowl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3upieijln.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vdkjqtjk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3cppqwdnh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3gglyrjez.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3naoybkjs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gmryhxst.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3adkhtcng.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3sorlneyl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gngwcvhr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gulnzxpr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ldbzvajs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lyxqiplp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3rswnyelh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ehmuusjf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3liqaxgnt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jrwtlltf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3vgphkomh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kosqurhp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3oqkozrmv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iivgbufa.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vuvwiaos.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3yocvplhf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3fojavypl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3tnsckfyy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3phasqjie.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3qicfkdha.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3uheyfdau.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zhgdvuet.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqisaetb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3atrflngx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ggtfdndc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gaxopxxd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjjpknit.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3aytgioih.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3wjqtripk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ezuaqgix.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gdscdogc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ebodblkw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tccddfan.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bqecpecc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hmpzvpug.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kpvhxftm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3tewqreda.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qipmcxiy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3gipehslz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jfkpalge.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mbuuiwsr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jgkjddyc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3uncyvscp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dumdhpug.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ipkqxudk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcfusplv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3fbiwepna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gstxkpst.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rnzjkxdg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3caycrjcj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lnbqugyz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlhlcmay.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vhjbvbxn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ligkpmsr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nnjfgsvf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3prhwdyfr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oawqcpez.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3lhhbrqng.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xziudjfl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vavacafu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoqdsxpe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmqbslys.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3omysweev.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3apxfxnet.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3arbojzgo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3abqslheo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3iokapkfy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3prpgumeq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbjjjlku.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wohyfqfm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdqdvtjc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aoamiiuh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3uaunjntk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3alzrohik.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qqnhgtrh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3jgxapgik.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3trdcopri.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wbevnwkg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvrebgah.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3euuvywxy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3rfqoddfl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3cpdzjgqg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwwvdkto.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzpzroqi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3usqezpmt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3inmfvuyc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3thabtzxo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jbynrtrw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zrfmjswo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3xtgewekp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ddfzntga.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3btjmbqdq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3sifxwutm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wjrkugcf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3wqaxbosg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3kcmmdatj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ctcdomeu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hgoofsqx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3wvfbebda.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3djmwhauv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3forolpwj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bgslpimr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3catgmecz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dctduykj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3okyqkmhb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pdlrsjii.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3eeuaxivj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3cbixdpeh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3oedcoolr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kzbrinfo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ypnfdkat.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3dlumrnfx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3wuutqmdm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ixuujact.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nnakpcyk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nnsduibv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ntvnwrkr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3bazfjueu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3hoeunynx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3knagtgcg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ijeupcra.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zbcotvhq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zetmurdi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zfudyggj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qbmdcjpe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jxqpjfvx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3szboeiyw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pcdkkcmj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ntpkcywu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iaozsaxd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wtbgjnuf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3xqygvmck.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3bxspdsbx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ljhmsixi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dqdclnkv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gmrjtetn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3rosddxsq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kyfgmikb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3koauzuak.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3phbdizye.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3rbhrnrlq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tknnthiv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3bnjnsgqm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ukgzpgtu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3srzmrlnj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xewknqtj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tstrmlph.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qykgaiwt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3xswmslkw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3cddkfomx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ppxysnbp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tlbineip.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3zibuczhp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zibqhryw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3okdbnhvw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uwmvcmhe.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3bwyuqueu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gqbcyvfl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnhyvknl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nnddykpa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zfahnljk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwwwvrfi.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ytwrmvfk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ukeajuco.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3dmbbpjak.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vvzigchq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3egikkkvx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cfdidalr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jhvbdcjb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktnmxayr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oaukcigd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3btzdugfz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jtoaozri.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ccercqah.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3tngdphfs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rngfwnvh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ukvsvtro.html


<!-- 参考信息 -->