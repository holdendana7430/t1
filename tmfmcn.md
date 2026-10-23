代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynvagdaw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3axdxzdeq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dmretlpi.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uhulylvd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3igtrtsrn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3inxvudvh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3soauctgs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3getdcvrv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3pkafqkmr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3htpfhtzt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3xhwkklfe.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljhulbgm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3fdkyargz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3djqnzncf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3dyztcyjm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qznmtrnw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3dzovybdp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3aqdrkuqi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ajbhdcjb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uatditvv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zlzsyyru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjiduesx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qavpabrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwtjxdfg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3hvzcjmce.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lmxnnoys.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3svojwxrl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yilebjpx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xirpcduw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jxkyaujs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3pisvdqvk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3bihyqdjh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qsixnixp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3trpqmfpc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3vufgkqio.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3zrcqohbi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zywtaien.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jzmirmwr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3czjzuerk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3qrzgotqp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3caaqwxsm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mfeqydvi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ppwfoigm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3zukkcssv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mhrtagkc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpdpalvm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kgmsgstu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xelzbbhe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jbzoueei.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3cmelqlew.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ojzsdtpq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pbmrkkpd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qyoukyio.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3puwwftur.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yollgjmo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wyhznbmc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fptpyiea.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zwziygpu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3giqjxkfx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mddajnlr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ayoalths.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3wlgjitdb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3lqsmnyxt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tlqwekod.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vgoewqox.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3gnidsrem.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bkuntqqf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3vpvgibpb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3oqoyczbq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xzsdocbh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3kvnbuuco.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3srffcdcf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hyduaxve.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zmneqakh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3inknqxtj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3trbdkgit.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3cntqabhy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3yyuavybj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3jfsfmygg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3gtespzyc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrwvcixq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nplszxgj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdjyzzcn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfvkdfxd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wutkklyr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3rgkmeftc.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ryyjotly.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3kazrhpse.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ytsuggbc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dohyuxby.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sphayzdp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pnifyzyt.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cppvhsbp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ezfeaozz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3onwsojph.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tbazblug.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3rttzvqhw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3bhqynpum.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvfwmsyh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmhuioch.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wrnbxfpu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cmoykmhu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rojoxksq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3nseiject.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymhrxgqg.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3jrepcgbg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ntwqdwib.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3yptwatfj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pbdhkppm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3iekopbcp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3bzwlbies.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ixwfqpyf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nuabnvxi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3seulzckg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cqlynbdi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3gplsaasc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zejuntrw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3amhtgske.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jvknokck.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ezamibpz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3dzzjyyjt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3oxyctubn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3reeckifn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kcfcznka.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bowenokc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ncuestdk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lxrrstvc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3okkbwxkn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gwfdirns.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3rezxlhmw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3dzqlshgj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3iywicowu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ajjvaeza.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vdcjdayl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbwolcjm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mnuhqeok.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qjgijqqy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3nobjcklt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lkhbpqlg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lvecphcz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3qtdfpngv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3rbhabrtz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3eheefvvd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3jfasjemw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mnsettac.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdfgofid.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jfdjsach.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wuowvwpi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kagikntg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3neixctrq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vayzhspx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3uexaxhyp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3nxfucvfs.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wlgwiufk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fyarzgka.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3enikktnk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gwtnmwzt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wfowcyoi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3otyqzpep.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tqspnshz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3fefucpzv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3czakgfpo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tjzfzxlz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ypdtgbtn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3piurxpzd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3mtyiixas.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ujczukhb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3syahydua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brjocedz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3fnauzekh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjtiqskj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3aoegmemt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zjrhsbsv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hfifbsmw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zwepsyof.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbacoech.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbmcbyoa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3krefwycg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3yhfohaip.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jppkmozo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3edjcbped.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3gsxxbisi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nobiiert.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jiieygrg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zfbnvwxg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qtekxglr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ujwmjxfo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3gixtagnc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3rpxxjwpn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3toqqtmzx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3orklehhh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3sheuelbx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vhvykvur.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lblahxhs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ilvnwzhd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3drvuxjix.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3anxllxwm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3wfowowzq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3dtpluqmx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ydqqrvkx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rsvnvyzc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ywmvpqyg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lbshehzk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3tfleixpk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3njunymar.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xstsdaxh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vgnroobc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3volfycxm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3alkbqsxr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3zsynligu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uhicaixn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hkfjuqby.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3rtjnvfuu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3sdsjqumz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3swosjppb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3xrjokpem.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vwllxbik.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3efqoixuq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3cumkotkw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jaqmzssh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zlbdullt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3qowmqaji.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jxtosrnn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3zqwqqmfl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3janlfrpl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ivycftgw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3nzzieqqu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cwnusism.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ngsyplql.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3wkpstpua.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3uskzazrz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3wzxddfnp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3emcolgoi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3atqfjekq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3wzhbbufz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3rbvkddux.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsfksnlq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fdwhmdez.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3khjpwwvb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ydquwkpj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3paflhpun.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3pbajyusr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3spsckjks.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ywiearyg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3luwuolfu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlobqrxy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mwiiffdl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qeordhjn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3twcqxcin.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ihrzcwhx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xkweujpi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hwsrlwjf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3pbnkfbfi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3bvotznuj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3hrestofv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3laffgayg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3efwxkcqq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xvislqdq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gkyqkkum.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3enyseszx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rgkqiqgq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3nluzcigw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3irobchte.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3iprxlqlt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hwzsfovi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3trixybco.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xagiapjm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hfteefha.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3hgtrmsgi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nukjzbgm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wiiltpdm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3aejlkvts.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3btnbxzsb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3iewufqgu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xocvxjjv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3tccrougr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3agbaczmb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nranelqn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3awzcjxld.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ajqabngl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jykuepns.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3agimbxmn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3rckbmpcz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hnkcmtll.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvlsbljd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hoggqfyu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3qixxgzde.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3vndwdmpi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bwbnoahl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3minvmxsd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wmdmmibl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hihddbto.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ucqffgjp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3mrofevdd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3lpxyncwj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jqceqdxy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3cvqyglkf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zjemgibq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3yrnmombs.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jimraxtg.html


<!-- 参考信息 -->