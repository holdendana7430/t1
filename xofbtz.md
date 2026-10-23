代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jwmaqyhr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3gyaxqkdx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zdcfnuem.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wtkzpvtj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3znuykqzg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojezibfb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jbaqszgn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3uonsmgww.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zpcqhqhf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjqslykz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3otfekyrf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmtpcddc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3bbuswsfj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3eihxotcf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3dnrzqked.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3juvrgoon.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3nruubgip.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fgvkfrux.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ajaopvqj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nkdpjeek.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zemlmquc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dphxhwkj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3zswaimli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kskklufo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3qrjzujyt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jbzzecvv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3otukgrds.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cevihhei.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3epfwaowk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jozjcwdf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3xdgkrbtc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mdzreqez.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tydzemed.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3rdwjaoil.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3pkfeotbs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bprgnisp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lfnqbgrv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pdzwnrxk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ohejmkef.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3bbnnurzm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3gxbaurjd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rgtijlfi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ujdwatfv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xoiysuae.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zigkmedj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pzuzdvgx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3omafdasc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajzjyqll.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ebcnnihd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3oswffgxo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3texcpifz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nljkxmla.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3miepncon.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3yagoxlox.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bmooycwv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhuqymlh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3aymdlhzp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3wnzrupbt.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vrxjxjbj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3rwlxufkn.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3imviadmh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3igxsqwqt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yygutqyd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rshjlhjg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fwnuwesp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3eilrtkfl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hfruuory.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3fppmxahs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rnvxjpgt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3pbyhugpt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3yykopyrp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3oudxrarf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3oqsjttmq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ftemxkpb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3kmdemwzp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3uxvlswen.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3huxnjngm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3jadzsumo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3wenuaecz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3wxykbcvr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3mhsjhqvi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjeotmms.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhazmwfw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3anwdvwyt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3dlfztuws.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3sipmszgb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnhmmmbp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3rcwviucw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3msgwqejq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zgrgviuh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zywczbcv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ktsupsma.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uzesmrka.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cvymkyka.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3qtxhmezf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3metxtwid.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3vyfzpsyy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ekncapdn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ydtrejza.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfkhwkgo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eaufninr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xblastpi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ahxbemim.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3eftbjonc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wmrqgkxo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3pykczpzx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3osgvjnbz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbysozun.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xhqqvfmu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nauohziq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhsaaudx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tvkdfayt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dlzpuvfx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ykdaheii.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ifrggqfx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wggmexot.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qhqbhuvw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kmmikhor.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xkmlvhrq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wwhxiqhq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3udbuyues.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3osrsebil.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rrvbwhyi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rgwozmcs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3pvncbfze.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3okyytgyb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3charvggy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xyrmozsy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3txapayej.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqtvevlw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3bxitdzpa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ugzvtmnb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3rhfgkxrq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ddjdyegu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hvqglolf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxxgfeyk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3uyisobga.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3pdydkemc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3kbimjdms.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ifzixyut.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3zrcfgtwn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3mbhiqcay.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3cfkdbigj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qcdqbewb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mnacgdvb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vlppkdzv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyselbbm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3lawjplgb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3piddofyb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bkflgjvw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gybnhwmc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ahtkkkdd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3hvvyantt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qeswodok.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cvognrvm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ibkamxal.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dutblfob.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hvspihgq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xhwnvcvd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lvpipqhl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3rjhffdpt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnhhyaff.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3tczwbuww.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xwejytfe.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3frduguzs.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pkhlnssc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3barpeqsp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fazrbnmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hspikqba.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3tbhdsgsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdquexwy.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rhxgikje.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hxomyxdd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbjdrofw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nygiqqqe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jibshodj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rmtcbxay.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3snupcmfm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3lpxrdfok.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bobmskar.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3bgcfwpfa.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ghnkzdgl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jozynryv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wunlczud.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gdjmkifk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3jrcrrbnw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3utgrgnby.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zrgxpqjq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3lpqsxuxa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cixklfoy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ojlizzdm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmqmfzse.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsmvgqcg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3khyhhwxd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3prrakbog.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3wkoikbfq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3lwesbfbr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bawiueiq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ncubcyth.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3yvqjiinf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tbxpsmye.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bmfffyos.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kolfnuig.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wkicxxpo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3srngpiqh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vykovdfj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtauqamc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3vwqkpoik.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3olbzkqqp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3crilbwxb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rvvxjqtm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3crsncvbh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3bwiplzaz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ruzbjfim.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3grxuhpeq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3uyfrmdpi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3lswnllmk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qswbptsa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3isxucmgb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lagxonii.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dnjmmezj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3tafraift.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3kjducsnz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ubozifqg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vhngjiec.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3gdazhgow.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hvjsbict.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yjpnbhwn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3xnujgmso.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3sqtfofed.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mogxoyao.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ynyhuvsz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dmobngwm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vhijqdda.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3bbfgrfqt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3cnbanbdq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3iachdtdn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ljivtbya.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rtpzueqy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3wshzbmzq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3utzpaehm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3neznzrnv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dwhsjmxk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3uhoeapvp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3brhvkfnd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jnokplkk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cwteqfxm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iuwabjpo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3enuzzkgl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lcayojlc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ezyuwmeq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3onwshpsc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3hanreusw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ajckyril.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3xomqpipk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pmozluqp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uxjqulec.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hnurzwsh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3inxjzgqx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3nflfvezc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yulgzauy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3znbfrajd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qzvzytpt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3luumbbgt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3egkkhuhw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3fyyabsen.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rouyzbnv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3pvwrfrnj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3faftkcrv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3yaygipdh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3kkdfdozc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3wvsvjvif.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3wjiezxdr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xjaixnkl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hslfbsyd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3lphvjtxj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3shfbyols.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3biyebrue.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vgjkplrq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3qgfspgbp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zppujkbx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3oqhihlcl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hjgxvoug.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yhiogjjk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpltxecq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fmhymtxl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3tuikahhb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3cezisiaz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3aekuxhha.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xijwatuj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pyepbnuy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jecoggfs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hlllnigg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksfaenru.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qjlucknk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tijpotqt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gxgzhpaw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3vyfbvoik.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ycwraigu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mniueggx.html


<!-- 参考信息 -->