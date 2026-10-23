代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mpudwkhj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3azmykbxc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3fltxhhll.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3pdbaxudl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qmrrvtgk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3fmwxythe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ywauvgqv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3tvzztgig.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3biutivoi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3iyvhctcy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3mzpsxvij.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tuuxngua.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jwnxowew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvduauzo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qqawgufj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtrypcau.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3uekzypnc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3kiweegip.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3modkrhof.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yrnaidda.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bvlrrzov.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gdxuixsk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3pgbtsmfr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3oxwleaxr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xhiigfbh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3xmookbhw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3pjufytlr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yazjbspk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fdpsxixc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lrtdoind.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3spiwtntn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3gcxtxlfg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xmugmqmb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xvobgbwy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3fqxmpixu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xgaeipcx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dazuvqdq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyrqvkzg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rmwdbtxq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzozzfgb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wxqrbumv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3gehtbqkn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bmkpnzxv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jcnicmmv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3sxoljger.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3izoaolae.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vfesdqii.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rchurtxj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zfuiasxu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3psuhajhi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3dngpfvnt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlxkohhs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lbhgxzml.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3gucvzoow.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3khekcujm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kofogtzm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kasrnjwu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uznytkpq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rzssugwj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3hesiowae.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3hggzekwu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3pxdznuqb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3pnowxrcz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jqkbdhrh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tipepzqn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktphskvo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcsxnagr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gaxnucsx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nzqnyjue.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hgvbvbwy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nddoewtz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3cxthnoap.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3kwmksmsn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeeaiwqt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3enzloorw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bnlnnoya.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ipnyhaii.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hchuwghy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dfkzwwvf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3hezcwblh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3clroubrx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ewsdbiwb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pjaxwvix.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xxrupmlg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ocfsfjqx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kmfiklgp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3bkcguhgu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fjedfwos.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3nwvgvufx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xglcvqet.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3slxfmbzk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqhvhvpi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjepoohn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3puzrpxhk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rgdtjwiy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3idioszma.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xzpsjbfu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3weskfivd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3mpjzldan.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3llmivymx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nmmwftxn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jljuuwib.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbdgzfsx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ktheitlt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3upbbqylb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3reispjao.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3xrdastxz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fwukqgew.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ecygnoac.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3udmhmvxt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ezxmgyrv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3jxqeyzel.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ynzmnlpl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jlnxsuum.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sjrgaifo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ftgphudi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nzbltqat.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dqgfcqcq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uwrrkhky.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vtdskyjj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3synhxgtm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3unbteace.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3cpfzfcvw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ahdhofvj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ezebbden.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3pktenvlb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3pwxefsda.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrodfkng.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dybaysxq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3shewizle.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3jnvkfpoo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3skeznuka.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3aonjgkgc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ztanxijq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ujzdxram.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3roslejxl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lbqyidis.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qezhhanx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tvkjfftl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3zvowrnfq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qoqdzyva.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3daurvoqw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3svwvdbrl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zlwflkvn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3occudcvu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3apnzbxpl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lwqrhjuw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cliahxsr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3intlacck.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3luppvqex.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hmuqcgts.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qxfhnkcl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wywysrgr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryjrqvek.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gzjphgxt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zoezjuux.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vkjjuccl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cvcarcxx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3pqslhbmt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hrtjhudu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyqgbgjl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3svpehnro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilcmhkvh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3crrevzat.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3uqyedcxk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qotpevch.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbsxaidu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xdhjlqht.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbbsjafo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3djfxizjv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3aqthzuje.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bqjnhnxw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3qzvicgvn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3suynqedr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hstyzjkh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlqgumaw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3atbzoedl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3cgpmadsw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fulwupvg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3wjifivph.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rszmtksh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3bsrcwfyd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ugyolimf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qarnmhme.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqijptht.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqxvjnio.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3kmrxomlt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3yppfjfur.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xllyqjfe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3pbynndjy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3iitqtiiu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qswvoscv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xcwfxwqe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3buqnqnmq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vgssuxzx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lrjiupgj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fbopwzbb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rwdgheby.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zrvrbpyh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mpnuqvqf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nolofjxw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ihhjkbfe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rcjcnimt.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ecudjgqo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3whjeaswb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wzmyxdym.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gcwddtje.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3kvmckkqo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3rlzxvcsq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3oudrzteg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zbdugesw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uobjucby.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3whzsfnvt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hilmbpkv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3dxtfzght.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gvpaxdzy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rcarurzm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ajiegpxk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3zrxfnyus.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zcsyxdft.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3awhgevae.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3llucytqj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3nioafzbp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3qdqdhvjn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3bhxvsshh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3crwxyovb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3imaasurh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ainqnybm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gbmvdmfx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3roifdcva.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hcwlmjme.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3mupghotu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rgfkblgq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3hkxjeprf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbizndot.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mjltxcjo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hckpzgvz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnymkzwu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3khslmjxd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ymvddlju.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpjcwwcc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ukkqclfk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tonakfax.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3exfgtnui.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lyfhgitt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3zewsbawh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3uwnpyqqo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3zphwvbgt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3wedmticu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3evhhyxmz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xuwsyysh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3virribup.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mabvlpjx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ltfuqvok.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3jywftlgv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3obxiozvl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ofhtzljo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jomfbwbz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3cdbuqrwb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ccfzrivv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3nyermtep.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qhmpynfw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3cceazayl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wrjreoch.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zaxcnwuw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xhdsmfpg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3msipfbnh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ggdeilef.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3pqqafnhq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3goakcnyd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3svfoifqw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3dgzyrvhn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zsvganje.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqmqpsqq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bhcvwttw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3stupijrx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjzjxemy.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bebywjpg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3sawqmhnn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3zvaizzlu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3exgsrxmz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xjquwcca.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3imoueuhy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tigqefkz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jrosvqsz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3dnzcnnvs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3tcaeheal.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zrvhdojg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3evtayqor.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3msrakpqj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3huamkstq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3cthqcgoe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gncwzfvr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3iwivzoqn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jawvyfxr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cvkzyfgv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3oeytfrlq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3esxlltld.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3whlqmmcf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bfchbgjt.html


<!-- 参考信息 -->