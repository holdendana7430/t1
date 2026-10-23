代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jcetoruf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ekzdtyak.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fpdyhnho.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xdqyxlvj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3hisumwxj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3djymwjds.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3siovtsll.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbqkptti.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3rnvviadb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzkqdkyj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3krxnkyef.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gohobumj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3wyuwwxlt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3zdrrtaou.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3xmxeihmp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ppqzhjgb.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ugbfuqqy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3efaigxcp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zjheewnd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3hczksvqr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fepowopl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhprmxun.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3cumvczvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avchpjmm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vfdgnzhx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ckchutmu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3udcgfelx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3akhrnsjz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cqedvzxa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ifztxhiy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3khikeojn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3jsmeeyjn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kbcgbmuy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ixizjeoo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3lomvdzqz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3mevvdncp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ojphrpvk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3capvgusz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kufutnmf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3nzugtgko.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3mjkutqdu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3anmsfque.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3pcqehgbp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3djfkwaqf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3apjtrpme.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hncwypyj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytxwzmti.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkedyzha.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lkeycpqo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3bpvmjmqa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yabqjfru.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3sdhyisak.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mujoloer.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrfwjhug.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lugacjkc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fdyrhcoe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3nhrnauql.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3omihfmzz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3jqbxrvku.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3zhszkzuz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kxwgibfa.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3bvyzfwge.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3rbqqayde.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jppdledz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3otvxpgnc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3bshngewh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3lmbrshsx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3zcncnacp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3epgsklcn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3jgrujopu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tjobcgmc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccbqvtzc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rngolckm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwjtgeer.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftlxvkhw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3dllfymwz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kazmltat.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufdrnxol.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zhacljrt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ovvxxyba.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3pjdhubkc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3evczkunf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3irqnlgcz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ajrnwpqh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ehbyuvyd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3sdkpvgqx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pfuttclc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mmimrbjd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3vlaeyevo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ffldhssv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lngkvgbf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eladjhao.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vcfoipod.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rrqdxwyy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zmxtkucw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3thotislw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rrdztmck.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3wktdcsdr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaihyqcq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ezzinsrh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xphstwch.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3flutuufd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kaiwrcib.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qvugepza.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ucqukzuv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yzokcdlu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3zogixvkh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3rkoleeco.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wxsvfcwv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ckrhvqfo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgxasvmp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3whhwaggp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wzblksmt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gtwftdwn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hacqwhzu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3iwujkpqg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mpwzygnc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kdakvdnl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uznritha.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fgbbbtah.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3doudlpbi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3igfpybgr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zfgnofad.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3sjtkzluz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3isnikafh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ljlhvgvi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kttuiceb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3seqaoovl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jhnsyugc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ujvjzbtw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wsaimvhc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3gdndcihr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3nypzmfqe.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3yisulxpj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ydyxqfyj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bzikmsqy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3soqnqhpm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3jreoaulf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3oxiefswq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ivxrksqt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3tsifkwmh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3futzfxdx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3opibthzx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gfjugvmq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrdmbvgk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oiqsyeub.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdecloqf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3epsuanmf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ennnyguq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ptkvyugr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3bvjipmjo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3aurrcfha.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3teidficq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3awsblywo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xbesmbot.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vcxkwikp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3knonowim.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3txmovrrh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nngikigc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gsyzcgxy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mcrqpcte.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwhaukrb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mzfvpaes.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pxeekfyf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3souzpjzr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3boimnmvt.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ancsjtaf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pnzzanrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvpsmovx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rzgvsowl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdnyqmty.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3agpzpnne.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xtmlpypi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3aioqcyri.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqgtzodj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3trsnauhe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xzhukgwa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fcnthzyj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3abvhscnf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3akxezcwz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ecqyyyru.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hicyuiph.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkgspdmu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3phrwmzcx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgsxxzyp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3hiwxbged.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3hldbdgaj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3prmemxow.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3yawuaitr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ymchpbuh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3vrpnfyud.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pfdqqmyb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ivjclxqz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3aijsuzic.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sowcnbzz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3toczytxi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3iquiceuf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ecgxpnwg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3cmqhrath.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3angxpubm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3zmjwurxg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltnvpuoj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3fmjrdudm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ooflzzpm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ppobqopw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3apjkjfbm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bhearupy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mqklktgh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ixwgxtxm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yuedfway.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lzalsyrr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wqbsiqvh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3wwlrapsz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3imnctacf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ybqosqll.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3aryvvswk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qcsfbzyz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3pnxbssrr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vymozvtx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fpyzefze.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zybggohb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nctencny.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3vbvnpxfx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3oogxatdh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zrrfazef.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3kiphcgiu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ttgjyzyg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3myzquyuw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3nkqbrukj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qoktvipe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bgvjoyvn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vzaunmnr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3pidfiojv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3zgbirtgx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3yabmkoiy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3nirglmlp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rhabmhwj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3noldmjkb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hexmhtvt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3sthritpn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3rbxxzkku.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yfwrjjxz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kytjgjqv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tqbkanwk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kiajvesr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbwmbrrt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zjlmffjv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qpjsnibm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xidzwdzq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3tkfmqehm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qbmdrjik.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dpyosnoi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eewayrlh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3rwipgupq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3cssrxmbh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jnpsbsqb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3eorllykf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vswzwlyt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yvhfxgtp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3httjrmoa.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vkrlxgko.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3kyfsbauu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3muakkebu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3uyjpzhwz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fnypgkdm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lqkkncmn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3umqlncoz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3cgezqqjv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xzpmqitv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3apmzjcmb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3xksdqsel.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ibcnhldj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zyjwipkn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jnsahncc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lmovnpdz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3lprwldde.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3murfzors.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3hgilnfgm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tgvzpupf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3elwxwfxz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mkdyerst.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qjzxwsam.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ybnzmkuw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dvcwrpvj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeluzwzd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3gugewgml.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3obwawylo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3rwfafnst.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3izwdqfho.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3gqitivun.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vtkhesri.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zcvxhkce.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3nrwewqjp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3twaszkuc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ebfzicjp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hxylfrhm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3wnyowakw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ohlgidvb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3tfivtwtb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3bhysjiyu.html


<!-- 参考信息 -->