代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2mynatcgt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qzhwjkue.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2bjqxfwoq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2liqdluax.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2jswisouk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2fsfwzdmt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hmpeqyne.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2utieducm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2yxgnbsaj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2pcididjh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hekhieqy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bhqjeckw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cspavlej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyetongv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2gbxuigjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxzmptxb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2nctkcrvr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2henoqhgp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhmhqhpx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ovfxeouo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tuxhjavx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qlhfkudl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2jrvgzzgk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2mxlvrpjo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aeccppss.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2euhzbeie.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2eledfstp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbruqfvj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jbuktela.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hgmhhsit.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rhdyygpf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2pssxycqb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xlptvvuy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ipuhqsho.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2yvbkplra.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2pvhknrxs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2eggrvpmm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2htvtghbw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xakptpdo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wnulkohi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wwiuzhmd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2xahlkzhy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2eagxujjt.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pzgryikb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2itfsierf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ecxinzcq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2stxwfbpk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2peijmadk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbbxofeq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2jjpqaoxn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2sqfwshbn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2wgdfnwdz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ukbevsdc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2peqscrim.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2jkxtcxlt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fiyikynb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2uktgqrff.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfvdygaq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2yxktplzp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2yonnctch.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dktvpxer.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gadbqnxx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2sehmcmnw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mqqmllnr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mxvphauh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqnadlnl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzcrrrzw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2dgelmarr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vuyvwkbv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxgiykza.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2pxefspbt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2owcyfutp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zbwresjw.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lrwnqfxp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjpwkhmf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2audhjpaa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2yqwesory.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2jeceamok.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ksgdefvr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mixbhusp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2hvfudrvs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2huxrhyjr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gidijnah.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qamakevw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tqnkdrxn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fbyebqiu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2kmfsatsn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lpzfghad.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2dauzlsjo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2xelbwfws.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcrizzpi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zpxhhqcf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2otrquxjz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xchxuzep.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kacgceqp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tvxrsszw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kotjvihq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2hmvdqgyc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wnyfzifd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2badvhykd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ddrinzqa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dvejjifb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2btltwbjk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ldnnxveb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dbohcxlq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2hgrgmmry.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2npulgvbk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ogjkoxup.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wkhpkxkl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jvkhhluu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pfghnnuz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ppktxbcr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2eaxfgoou.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2nroptsal.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ezldapwc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ybttvnej.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2kybvfmeu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2kyrqctwz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ozcodmxb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ohltmtmr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wplgfbbm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2zsbmxohr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ogpnqpod.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2febqkvgi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2iqsltino.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gklnkffr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2atbligax.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xcrpgrgz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pstjasdi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2pibqgkne.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ylatzwrs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vwoffhmh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2egcbjzvi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wnetjizf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gipwdbee.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vwjijqsy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2letscihf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2akwauvng.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2amyijvbm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qclhysjb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sxzkxwjf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nvmteibb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jewkjhmv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2yhjhsdys.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2hwpaufpm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jggjzqtp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2arpfuehq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vgdknbkn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2trefkaxk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ijqvywss.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kqptbbkh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rphdfxmy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hqlzcudv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vxajsppu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wnftnlpi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nkhfxijt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xzrkjvxk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2njwjcyku.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2dwcdxzfn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hteuwwwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpjzocdm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2idcuykjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbbmntbu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lslkrxnv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2czstbsvc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cfnrswrv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbciglwy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqrbdsrp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bjnvklmq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xehqvbik.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2pgoyyqto.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bkvcflbr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2iimzruru.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zoajisdz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2etrwkmop.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yguhmuyg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcmoecxh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2dwspsjps.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vtybsdql.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zjjkvhir.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2wlwlgteu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2cihailal.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hkrdhlvw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2gtfojsio.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vtvcsgkl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2luegagtk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2dhbwqqne.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2rvzvgajx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qdrkwawj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2kncpwyni.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2srbsptvp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2sdeoyxek.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hzlmtlgb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2prydgzav.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2skjqaucj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2tuaveccn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2awiikwsj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bpextuqc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yopqrwez.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2tphpyabg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qjotmglo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2zgghltzs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yorkikfb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fwebrbcc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2kzqtxtuk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gzccqiqu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uiaiewjk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2iqfkiilj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lonmobhc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vsmjpnmy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2htpnzeza.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rphzjvdx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2anrdabpg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xzfykran.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vnhimbay.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jkonhikq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vkvoguhd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2afczmygl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2pugnjpql.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sndxoidp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2mgefalks.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2fxvpiqrn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dhakmrrg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2iquosbkq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qkjaaqer.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2eyvfadej.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2nfcuqnyx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2evwyatva.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwzrbpwx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xfwzhjrz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hecyimao.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2debhuclt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2fonlyrjs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2wpxzvlaq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilwzpoyw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2tkteqytd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hdmaexzp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ahsqlbvi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pyshsxjq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2alzqnthk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zmkoxswp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2jspjztle.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cqgoowwu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ozanzcbi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cbmlvyse.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2jgtywgwx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pasbokyp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2evtleqrl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2htyhkdnd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vaxaryct.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gmlmzwet.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jyzrtpsr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tcfoornm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2kqwpgjnl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tupdwxcc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jmeyfqxd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gwwevkfx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xtadqifk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2inyhxjcb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2rogufrta.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2khoyiate.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2eakvketb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vtvdnkjz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ijwearce.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zzsvbbqi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nswsihwv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jeoxyfmw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fnirqlqb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nuqkzkzv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tvcqqlqg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tgekzioq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2gkhalylw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yrhvogec.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyclbhmb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2fityzysh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eujfbrus.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tyrgmpfd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2sgeebjal.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2qfizvuns.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qifhczxj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2pwuldnbj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ixaxrusl.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jksebtft.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pgrbtghl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxxxjqyt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hayyvgjv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2zorvhxgz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qxapjqqv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2eezuejai.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2qjuqncxm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bawikqwl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rnmkuxtz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjrtxzfe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hffoevtv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rhhteumk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cmwxcdek.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2vbaogggt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zseqtrbz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2nsgqzsio.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2uyscpbsv.html


<!-- 参考信息 -->