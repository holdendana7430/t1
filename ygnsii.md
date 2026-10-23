代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vcbluwth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljjpxryb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3euvaihve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qigtynfa.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vnqlfnic.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3pkdgsmhn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3lxeqjcwg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jzuemays.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jwtjhfqm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eiavoqhv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3kyhmafwl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3movqfzkh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ocksvrhk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3kdjwcuuv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ylbsaepg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjskubgh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3juogrrue.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vaxkmekk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kdlvnwrt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ypxhyreh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xzqvnpee.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fsbwnvag.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3pxuqstko.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3qfczaflo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vcnudniv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wktfwrbd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3phqytdko.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxitajpc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hwalnkcz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3skgjtwqy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3neenlwpx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3phztbasy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3gavuzyyx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkeugscs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbxwhdva.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wnkojbky.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ftndnusc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3xcxcbhpb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3pvudmsbq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqajdkzl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iihxuyfs.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3lckgaviw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3yngytxgz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oarnoosj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tszgseoq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3asrdwnic.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3mnpetpnv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3kdbjcipi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rnsgxouo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3yjfnwikd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3btatiohs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jftbobba.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqolycov.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfynvkwo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3otwpmucz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zuoleggs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3kvenuhou.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bckfaabn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nzckkoez.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cghvlcsl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3snyfeopx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vhbntmof.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbhuzpss.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbumyfao.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3vpyezlka.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wsqksgjv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3glkuwxwo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mxbhyegp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ygpvlyhp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lfxlkelp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ftiozyly.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xfvrnspc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yrqvngiq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dswnclpo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3yczllhjc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sjuqrufx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3atmnklcs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3nkuceqsp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tryhznjv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnzbwbwy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsfgazid.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cirrqqkl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kngizbok.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zrxxxcee.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqgysvjl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ncqvnqpz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3udekukcv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ntnvuqyr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tckrwhcv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ttbkmpxo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bngtrxyr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xskyhpwk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3xmcoptwe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3aslzetes.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3osuscwcd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3kisugufi.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3srfynayk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3veykhgrf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mjxcxbye.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3qxxaeiev.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3hcwowush.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tbhmqygu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ebwxhuev.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wuagtefc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ywfvwqer.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3dbenhfye.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lsyayxdc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fkbnnikh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vhgpicqq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ztcovgte.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jblrcycu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bcdmgljf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ukuvamzf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3htltnrdq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3pwswdvsi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xsvhwkji.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ursvfwax.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ubtktklx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3tdoffhna.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jmbqdvbm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3lfaqtnah.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3goxkrrja.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gzrnewcf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ldgqzbob.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cifoicgv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ymomyfxo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nhcrpggf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3uzxulfec.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3habkgpyw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oemingfy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3iamfupxh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3lmwfdexb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3cnyjxksx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xyvbofiu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gegagaiq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yylshxgm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ngxqqsce.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ljbanxsx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ixjfnlvh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3piuvozug.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3tvaalhbu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhszmcek.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vystoklv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fhwcgvhl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iiwmipsp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3herwsvxh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3brbmwmqv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bgrqmpmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csddhjim.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3uxpfhkry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yegisqul.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tuqocqeq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vnldueuv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3chcrinrq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aatjnmjr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wagbueht.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xwwcjdcl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ovlbpemj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3mburcyqu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmbivsua.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tglvgzpj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3irwayngh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjytyxxb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxsqjlah.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3olypvrxy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3vmkbuydx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3idrgbqiz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kyjlrhih.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3posxpllc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ujshfovh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ujonbnxh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzjhgwwi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3aomjdbwu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lpvhhkeo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3typkrfgh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3krzebrwo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bwrhoocu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3hkokfslv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hvajntjj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3aifntnhk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3prtnddhg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmkmjwwo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3amicpiic.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hfnluybj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ajlacull.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rciptwad.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fkmwrxtr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3cmlmaeiv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3isbltywz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3jtbzqyvw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jxloadgf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mytjkkpo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zzeaumzd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jpflavdq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3uabystvf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3uwlumdbh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3klupmxhk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3npizmlcm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3toliimke.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mxnyyhch.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cfvrvagc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mnsdzscu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qgzbgqzo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3erkjcepm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jturlgts.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3zoryjbnr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3kwcucowk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mhrnedxz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3grglxywz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bizcbmig.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3iheauico.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kvbniror.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3vkvfgheh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wewloerj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gjospvls.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3styewlej.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxqmzdae.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yinsruak.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vilzaxhb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3pyaygxmq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3khfjexge.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3csrdxsgj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bacgutsz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3hofenuzl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rgbjxnai.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uiesfhit.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gpilwsnv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3oncvpxom.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zozsfbaz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3mnbxhwmy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3iqeflaix.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3gwnojixa.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ityrxtkv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3cspedbeq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nvqhtlbn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ywwgxzjw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3nmyucome.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3otsxmfhb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rkaoubwd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3xijohdoe.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iimvdqmc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3wyhkxhxv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3rqnbowpk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gypinoxj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rilgjkaz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3pjuneutu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3okiywzzb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hffugbig.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3thusjhhf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3phtwffig.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3nrdybmxz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3qogtpjul.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3vtaicpei.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xnredxlw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3iqwxpqft.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3mjncfjjx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3arwivxfh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3uwgbwutf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kutqrmtq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rdepfeoy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fsuztpdm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqdrkdnn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3bewtazci.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bypuurya.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmqltspv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3simepjwm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qwxetvox.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3mncoxtqq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zyiuarxr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zchbbjli.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eoypbjyg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3llfqrest.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oawmzxsg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lcdyiwhs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3snrphvyy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ntwipwuz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3umrumydn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gadugmci.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ixkdufko.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rsuacwdn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ucbfcvpi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3hfxttvpv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zhtjisau.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3snetkxks.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hsaxqjct.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3yybqlslg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fgojvrgw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zvjozgzz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hqkdzetf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3covokiux.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bunnfoph.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmbcgrrm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gbgfrtqj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3pdfmwloa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqpuwxma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykjrjsch.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3kfcziubz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuwcajns.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xpsbcted.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pxzwaaxq.html


<!-- 参考信息 -->