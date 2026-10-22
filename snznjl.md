代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2xnvngcpu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2cjsdaalp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gxnkqmen.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2dexshmcc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hzzrvjjv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2wczfqzro.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jlihuzgy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wldjhxqg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2oqvekztk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yfwjrqys.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vkrqygyx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojyetqqo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pkorvhqr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rohhekpi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qpcvxomu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rvfmwtgl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2gaertcmo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2fbjhvtql.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2qjoeafye.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2emogqnww.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ysbjkrjl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2uuzwwlje.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2pkykggdr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ukkrrqqj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2trokydbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xysarkdm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2eirketkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qumqmicz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2eavjqoia.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rjilrqct.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2tdatihik.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yxojzssk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nkuywucy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ausurcyn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2frdbabzi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2mxrdsmgz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2totspxzz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2cdedfcxi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2gpaqlmgl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ainwcswk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dqpsoopf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gqyfoove.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ywsqcadg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2tgprflwl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ujaqmkdk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qzktoctf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2vvkskogx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2nftqcbfa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcgcpxum.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qyddzuzh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hkzzqebm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wnhdkind.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hkbywofm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wrmgwvjx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2itmvwojj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2unkuxdra.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yzzzmakx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vodrujae.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gaynixpf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zbvmaiko.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbasgaak.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2bjuwesov.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2yxdlqmry.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2moqbjkmv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2llkpldou.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2nchddfex.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2plauosrc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2spcorvwp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nhnmzkyq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2llxiuyaa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2esweyion.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2pljgdcku.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlgykmzd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2krvpagfh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2tjxfrntk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2avykqzvs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zexgwukl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sxnifuzm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymkaxvfr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2tzabxkns.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2uhvofvtu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrwuiwbv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2pqbpaqzk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dklxsxgs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2fejujlqb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sbyattbm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xnqzboke.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ncspvtno.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2antnnhjd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2igxnpbvs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xrgqokrf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2oofexjrf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2lgyfzlds.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2teqkcixx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ulqqpwkb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hgqdgtpf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pqtgobub.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bwlbyhlp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qdjpzeoh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lzxktnjt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2cpfgjxdv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2illanurt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnwlcoxv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkirbtpw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vssdxcch.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouqdnkqf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dnqxjvqr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2euqwldfx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ydvblqet.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vbfenpkc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2qesxkhos.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2qwvwntco.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2arlacmnr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bldzujnb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2hnxpylfo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2islsqcsx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rqwofeji.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2somrugux.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zrdpifip.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2sqpslazf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2sokgzenj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xywxvzaw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2clcrwdqg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aujdbhmr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dsimylof.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ombzvwyt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2yvmhvlys.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vipchulw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fegqtham.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2fyylbpcr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ujbfmaji.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2oulncgte.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gpvpitbw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2xqwwkvjq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hleipuxk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2exxvedwo.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2fapqjuid.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ajgnhjzn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2tyqdbiey.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cshdxwcq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vtomahxc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2gbhbnekb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ksahbflt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2fxwucmtu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2sqlsfyig.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2rfrknpxn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hxmckejp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hzuckpoj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nolkackp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzakjxhj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zexrnkak.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hqsywyye.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2chfhcvie.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qvkcusgc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2gbislvqk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2dsstqqee.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2gukibcgz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iqphwllh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lchigzaa.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gtoqhifv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iexkslfi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ynxuwusl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xrgrgukp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bkujuotd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jwhbitch.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2grijtjsk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oznspjgi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jroquksi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xxmcwoiz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dhzxybuf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ipxtpnfs.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zsjcqecl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axyulinq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jbnnfbkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxhroysv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qomteufd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uydfiiek.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tjeyfzdt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2unjhlrnc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmgunkov.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2svcoxmji.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2caxzqjvh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rvsoczaz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wqygkpgb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2wuabekiq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2rftglaqd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sddulxmu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekfoztnb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pujengqp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ocurobsl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2rxiqufee.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xlfpkcnp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gxseggpq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2atvyomyh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xddlnwyj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pccgaxtx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dinpgndb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ugzwgvag.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tntqyatl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2fooycsfd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2fghwosum.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2uxzyixep.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2llafugyd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vvqcqqdi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2juurtydi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgembxzv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nzfrexsf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2wpahomjf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2gbxecgat.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qzrbpumj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zlwqkwyj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2sohwjyfy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2sstpfnld.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2abrgdwcn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2uupkbbhc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bejhksis.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2zlknvtke.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xnjaqnic.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tbetkmpe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mlrmapzt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2zmrbwffh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2yxfzcmjy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ulvoxvcz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nvxnifcu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gsszrxet.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zthxekod.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2yhlwuszx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2prmsdqhr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2klgpfepz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2czbusunx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ywwwlfov.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vuujjwxq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2bqvzkyqw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2fftuxfmw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nsaqqkwi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2onlrdxlk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2iowvnhmk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2gpekyxiu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2shyiqpmr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2iqdmztuz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2tkgkshrl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2amqzfnxz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2klppangj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nsnijbaw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2dheuofxn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2aotpkqyf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlcayybi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xcylkqzp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xozfwdfj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yukzzimy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dciokgky.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2inmjdepv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2doekrapm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2vshkbzue.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2macnuoov.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2opkaofxl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xhurpztn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2bzdajajw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2yprpfebe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2fybopxvi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2rfyxzuvp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oqqceotz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ullhxdmi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qivxlckr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vmeqejlo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ulfnistl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2nktiiblk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2jqfdaily.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ptghddom.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2fgkkgzmj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2fpctjrui.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2whtbobav.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2oueianyo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2mgiqnxtb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xjqlasdf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wbkzyxzm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zbhtwnks.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2taoclsxm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hzwksrcb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2pwownnkr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wfppneoc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2etcfdclj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uqkjppuo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ufzhrowe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ribyoghs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2svhlausw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2anyhrgav.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aqdjiade.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jeodlrfm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2bszvfewx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2mxkxdjgi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2cefvvhjt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2anfybnxs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2yjdllyee.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2aulaajgh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bkmemawg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wezvbqpy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcapalxc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jfgrunij.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tnmwycrf.html


<!-- 参考信息 -->