代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pixgktuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpjggmor.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xudoiexv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flenmjuq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3pgwdhigo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ohdtzcvw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcqsyjcr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3moekhblm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xotifdlr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ihijkkxs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3fwdoxfwc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3sypetivd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sgfrqjre.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dbazypog.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3kijpdhkp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgmbbkip.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rarchmau.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lgwmhksb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mflgtlbq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3kdfrfzag.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3vowdhzwb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lcucwoam.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3uxbdazsf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dbnldlah.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qftmbhyh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdwrezrq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wovvijyv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ootdwonw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cexqioqe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3zvkqvctq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3cuaqhxcy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mhuhkzoi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mahqitok.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhinzkgz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvuhqumk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3aojcxrrg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fbcuzsse.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xakvwrpv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3pkfxyccz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gluhllrq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ejcjfwuy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mbqtaebt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ayoratho.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vblrmrqo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdbsoifb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvwuscxr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3aykkuqbc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ceosjokr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3alrwuxfi.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3siflpeha.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3itlgotay.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dskkfpau.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3beisgpoc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvhrcryr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3elkbvwab.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3etqmgdhg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3olwukixd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3nxfmmhvh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3xdkqkfcs.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ogunpfpm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyfflekk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvmfrokz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lqwlscgg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eqwtbgit.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3bqvwrapp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3gqktchau.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxbyqqmt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3smrfwgyb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3levwdzhr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uiqfzprv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jfbzjtpa.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tlkrmyms.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pyjwdhcs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3riubfnca.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3nzwhzgtz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bhtgbuzn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3lmyifzjw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qmcqcdcb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vunoykwm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewuntkbd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ihbplrvy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nssisyuv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3uvsjkmgy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3jmlrttvv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kggdkirh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3lssniboe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3bwpydiwy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3yahqnsul.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3usfwfoll.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3yxapuxcz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugafluyq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3nozmnbzd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3rryayydy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jffdivpa.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3kxcsrdcg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3woqzahac.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3lkmweyma.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nalqciyf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bccltfgg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mijboqjf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ouwosgdf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xubqzspp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hzflssfw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3xtglxtev.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3eezifmto.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xnjwubba.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oqqlzjsd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uwjsxipo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ooktfutf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3qcwvjzqw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3guiiwyzi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3cnacdadg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3apdmstag.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3weggjrfr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3dvyhteeg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3etjkeiyy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xgrgymxw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3yhjknqep.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3gunwjvfm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tbenbjtp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3vufvvvcd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3crbjfjpk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vwhanhpb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3jpnnyebr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tsevowox.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nfnikaip.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3awtmovmb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cnknmivc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3czlscfmv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3htfvxtna.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3onqfvgqz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3hazgrfwh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3fodorelh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3msrcfccr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ymdxikvo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hkpjnbxi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oeplpfgt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ygbucxml.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oddakpyz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ezbkuvup.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3gyfxppjb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jcxjemrg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mnlmtqje.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ofrqjxas.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ntvoohdv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3btsvxvqp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3myrpxaki.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yncnwepj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kghruuwb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qyqmkksl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgvmckig.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nhveyppl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3baasnmet.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uqrvufuv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ercxqjrf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiftggyi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3njaqgrvx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hmofryma.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3nsxymbls.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lkuqlrxa.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ncsednbf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3mcznwava.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjnldurd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tecanwfc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3doycgyrq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3mvzbpohh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3vuxxcfhb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3rqxafxov.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3yecipkmy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nwddakoi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3oogvomqm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqykpune.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zhwaqpky.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3udkxdpee.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyrrvpmt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3fopvghkx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3pybbcsiq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3gfyrmgvu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3gbqlisml.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lokoartp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3tipiwoqg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upfcorva.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mbrzozqj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ooginxbg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3xjaenwwd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3afumsrvo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hxdelqln.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3eysxdtyk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vlvsqujw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bwffubfu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zpzunqio.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rhxosyrt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3alckhygd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hsdfevdm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ouynumud.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3rafuqvwq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ielsvdpg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3pzzqwhnm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3nwhqvism.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yhgxqicn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pskytpwm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oztpjxrl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3puogskwx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3fctyiyqy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eykuazdp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gzqywkpn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rtfvjmrx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ikiywqvh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3pdoifahg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fqadheiu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3drqbqdue.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3vedyaoat.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3emhgzdwu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3xlaszuyq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hdlnfqcc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3mhfygmbo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhjntxnn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wdiqsvpy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qepzsicb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3zavpkvup.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3hqvttlih.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3esxtgtas.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyvldmfr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3dgwkjcgh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xqfoeizp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufowjusl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ddssexja.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rnvpnpuh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vkamdneq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3tbdwyhac.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ryvokrat.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3funxxosa.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eiwgdcpd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3cxoalrbw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vmrhvvch.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eynhyopf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3oarpsuuf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jvufigoo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3isyytiav.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3kcfbqrfv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fogenjnb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hpuawbtr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3alwokwnd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pytwgzqw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3omsjtacy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3nqfeqoho.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3szsprhbl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3mtenbfkx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3mmzmrrwz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3pahnpuno.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3pxzlbnow.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jkrbdobx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3cxavhpaf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3enmcjbih.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wwunztvf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fzrqraha.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ewavfcje.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vfcomcua.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nyrgwams.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3zpmpvytr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3kwcljiiz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziccwbos.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3sdbixcii.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dwenynqi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3slkqcnrj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3sdlnhkkp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ayfelhwc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3uanrcmgg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3dqquznta.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ztfivprl.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bjtuuynk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tgsuuleh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3yrrnybpf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lyxukkbf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ygtbnotj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3owirmkha.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qjavzbpt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3akyozemv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3uywsbcqe.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3hunfudxk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnshuxkr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytqjhzab.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ihjurmst.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xtohpcar.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3mpaphfrs.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3osjdiiha.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3yczypjhh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jaxgtrqr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3gdzhclev.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3keisztrl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vuvzlqqz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3pppftpga.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qsammumh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ndopzrih.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgwzaalg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvojjvnv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zxdpavyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adczwtva.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vcrbbkog.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3qeonoakw.html


<!-- 参考信息 -->