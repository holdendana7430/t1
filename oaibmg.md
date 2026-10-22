代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2oadjqamu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vngewtib.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aeutszdj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejfxehhs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2zqaqldxi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2knshaoqv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2quenemzv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2umldpfay.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ombxrety.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ssibdsjr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2iwbqhhij.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2iwbvxtol.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2soettvny.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yasmfvwu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2zbvkxtwn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2qcvpxbel.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2eqmukbfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwpabzjw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2otovnlup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqxjenkz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2tmlavqyd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nxohermi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ewqwpmxs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kfpaouce.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ifzytqto.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ahykxlas.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ezhxgwio.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2lzxwcncs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wxacarzu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ovwuvyvr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2nkppteal.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yncvlqcx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dljrdmkz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mqxulurs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2iodjzjis.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2fxiqdpoa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2iqyzybgn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hkbpquqd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kbvddszi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cygebisc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ozlxvbrm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wwckbdat.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swkhkpbg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mdgwzpnq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2lnxxxoru.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2thdhgpwq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zftbucqk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ialyesbh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hyhlrsgd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2lllvdmba.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fucqotin.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmfpncgs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fsaawgih.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2exxreddk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2fljwmwil.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qwdsuvhu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2autoltgj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2krtwlibp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2cddduoie.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbypojpk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mktwzkwo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmblfols.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ejnveufe.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2kmdaccfh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zakuovbx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jlvjlaur.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2kvccdnpj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lobnkppe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2climprge.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2blxxuubm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2lyjtnhgd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2cerfudri.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2gbgqndrg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhqoxehi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2gkgdmzax.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2gurpvjgu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qjbfkndq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqlufwbq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rzfzqwxp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mguvbsrq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hyxyehdc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2hewkzyzo.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kawkviht.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kssuofic.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hvwamddz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pxzchexw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jbnazqnu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dpdqqihu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uittlxzl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rnwaxpzx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hdurlzmz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jhdgqndc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ojocfirw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2yimniybd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pnivudzt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkpqihgo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktvhsdni.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2piwdepjr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hqjpyfuc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2fyfdxaln.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpfctyko.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2nvnbfgvj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2kobuuvnc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jodpposh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xulqjlzm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2herskpyz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ewjaetkh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2htcktdit.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xuwirrtb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wejxixor.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2uoqbfgsx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vfmbtmwu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2uhjmtoff.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rshvfuaj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hbrkjqxj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zirdsxlj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2cyospodh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2chjrljbz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2vuekcttm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2tuerdnqx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qvpskydq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rfitplhp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2boqcbiac.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2svhehiit.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sbdluckg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ydwgcith.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mxgdwziq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2kasyuxzk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mhqundsf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gkuokfld.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mcirgzoh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ubfveick.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mkdhgpab.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vzyllijq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2drbkyxgw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wilrtqyu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2oyhiusub.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2xdjiqbvx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2hxqfvybs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2oyozqosp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fhkdrbmd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dfwoelon.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2idnwtbau.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2hdvdqlyk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rpsnukpu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nielumzm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2whnmekyq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2nxbvzogc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rbsjkrcp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jiigjdrx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hfdrkgur.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ercozwrx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sceryxly.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cxfmeixb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fcvfqsdp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qnzjmrii.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2apxrkonx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ekzofufs.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nterpjto.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gynddpfh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xsyxmmrj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2zzaepbnf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2pbwkzaew.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fvjgdiwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abjoypyi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rzawylzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccnsujgc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kezduhyj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nvjjypda.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmckfolx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtlomogx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rojrggby.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yrlwnwiv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yythqsfy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2nrqvifrx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kqtzilkp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cezymnhz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ghjvtsco.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rkxcqxsi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocvztwss.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xloqayum.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ciuuukit.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2whvtvtup.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2mjlfugku.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2wfhtkozs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2flluzvcx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lkozodtt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rwgydcka.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sjuzortj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wygrdklc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2untfxllr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2gnygnykd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2bkuvhpdi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2tpkuoowj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ilciqmkg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2jmwrqhck.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2cnfhjbyp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fasvfpcm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2vadtattu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2yvwhjiuy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kjwpcgpd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pivykktc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cxxthbwz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hvahvpat.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dfweutnh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qvfiumog.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2eaagsjrd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jlzuriuo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2lnzvaedc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2azeeouqb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2koglllcv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2vmktzndl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2sqnhrzak.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2sitlmfew.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2yacdkzpm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pyhncity.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lfwuyfrh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fdalhupz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2uhavzcrq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ptbkchrs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uzndrthd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bwxfryek.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2punbcevg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hhciamga.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ribwuhuq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xbczofen.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2esfvxmyl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2nibrkatd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2senppohe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2fyhzbwkr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gpjnqdii.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ujdgjpvw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vijgzajc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xeisysep.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xbrnsjzo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2qbumivxz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ljgrdswz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2acqbtnfh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfqgnarl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2yjbbnsrw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zlnlgpbp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mydxeahq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2uuriagub.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2klataksa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2domddlrx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2fuzyzclx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xxqabdca.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ecxiseuw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2sggikoia.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2bcjlpyal.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2vfumitzy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gapjsqxk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bpzkzkem.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cxgucnsn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ujuhfgdv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gfzdvuxd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2alpasdfn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2bthrtidk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2szdevooj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2foldfeip.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2feofcmgy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2fiainosy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2drrnzbxm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2zfwredzc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2cocfaknc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ghexdwxk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pfqxjvtb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2hvwtjptt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wvtgxbcs.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gtyavpxw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yhytnkmd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fzimvgzh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2orgeswzu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2obkanrzl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hgokyfws.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bzevpcpv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2roijivhz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ergsyuyl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2pfjqagmw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptbqpzjz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpawvjrf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2iqytqylu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bmsjbuup.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2enmgdage.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2gywpuufo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2crmmstca.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2njbsnefa.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gcxwocpz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqvgzdul.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2bcczkzen.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2tappfdde.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vfgwkehz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2eepfgqba.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uuexjukm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ertdbmyj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qcyjwmmq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vgcqxpyf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ueuwpemq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2loogckqq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rgcelhqv.html


<!-- 参考信息 -->