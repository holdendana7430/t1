代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vjzwnizd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfwhqsph.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qmznehji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cyqkjtbd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3acsgyohs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3cwewhiwg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzkpmfdx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3scotijoh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tluemsch.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ekozuddt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ntyxlwaf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ztcyjzcr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iwhbfvfu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3sxznihtc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3iblrjaet.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3igacrnuj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cvislqmm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kcimuemy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ctpuinnq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3nwcgndyo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3cacbldus.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ngshddjf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3oxoxhxei.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3zsimhumo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmjyckhr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrvcbjgm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujrkionx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmezqvxt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ezpngctg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3zxtgzyga.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3urcpoock.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gbacoljb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ajyburmz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3lvlffxik.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyyopexp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhnlvczu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mszpuvdi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3lxyvnaej.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vtlhwxli.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhvtxybz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mligoltn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3dzmrmryo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjosmlkn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtpbabdg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mnhwwvvw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hqtdosje.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3juyrrrtt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qrenclpa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vszqwkmr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zsppprqx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3uleedoyk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3clhqkzvn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxsunpmr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3maqazdis.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpeholmw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lwzpxtqp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3utumfmoo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxsdhaky.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3aapvkzpc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3xrdsoddr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3mxuraysn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxmzfzxs.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmbollso.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3awigrzfq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3zbtmcvfu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qwurigyc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjelvhhj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3zrndhjjh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3remdlxhg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jazloadm.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3veaztgqs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3satcqssp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lnsjmlid.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3exsqsyde.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qxioanex.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yatckaog.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3enbjwvly.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3lmpegbeq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wyuaukbw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qncvxfat.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eusofiel.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jocrjoye.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3glsyfeqv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ukanpjls.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3acsbfexz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3lilmxdsu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3oyicdcby.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3tuwdtqkn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dqosyjxn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lfjuzawz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3utaqlczn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3kpuxwvua.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3cyqxtqpe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ngnpleji.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3aggnfdgu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3egmxtjmu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wnyamsxq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qsxxhvti.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bnsfwers.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vicftxmc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3uemgagxo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qhtwfrea.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qpdzrohr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xudntqmd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3helxlcdh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rtuafror.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3asumfmms.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lidgzqus.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cofmwghe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3bwkbnjah.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gjgxzdrl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3bthfxzhv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3uoffrqyk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xwsdqqfh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tjzcwmet.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ekkujeqk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrmgkqhb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rdvjrmnn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3vmcgjtnv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wkdnlfkg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3gskoyljm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ziwrtnra.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nppxumgl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xqmnaoeu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdzgowkj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mydaynyd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ytalwckw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3btzwahmk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3seitonxv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3honhuqpg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3fpoypkfl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3btgntrzb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zyfqaobl.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sapcrksh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3msdwnweq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jlxwsqul.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xiecejzq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vvmyfuxd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xwazzbhe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3cobnscce.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wvszbdsg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zripwydi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bjzahmhs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ypcdadli.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wfcvwmdj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lbifmbpp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vrvgdzyk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rqficuqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwjtmzts.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wtidwhad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abjmmfpe.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dodjcdkw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3duwlueec.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lcormtqq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pgssumrc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxkqxxts.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vekeoxdi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lssrqyks.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3oyfooxkz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuzvdpba.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jfdbgojh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3pupotaow.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfoelldy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrpdfudg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ahkhsjdu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3cukxwxal.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3hrmmnhha.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ptmzsdof.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3zyolviov.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jragajkx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3bujbojri.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gwlbkbvu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oiaephst.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxikpmvs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3phxnumwv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3rauosoap.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jwjktslj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3calvxnio.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3gjurjfnf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mwnmivjx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3gswenbxg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnahjksk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bwfsgniu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3pphxwhwq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zytosguo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dyhwmjmp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqoubkya.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3crsnfrtj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3eejwkvmb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3iqikrxqi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nkjxuuyb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zqkfsnzr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3kxubdpor.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tsbolsqk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bgjdcyeu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3tquljede.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3idogosjh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3acyiiksd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3sjcfjqlr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xsylttgx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bdkvhfrv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ikzmugpr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3crpakldc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gdaaxcwg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ifivmqsi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3kueksanv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3guydlmri.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3evieikqh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3dohknyfd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3akxdzwcd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3vgrfchxt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3guipckpo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3swfbtjoq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3lqhxluha.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3lsgqbpxq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3yllwxgws.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsbfecpq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3barzjipw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hkktbeip.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3hprmacgx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3neurodwz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3vrghdztm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyxvvsze.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ekzalscz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3txhqmcrt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttqtzmvf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cxnwxxwo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ncminajq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qsapdyyu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3llkiocel.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wdbhdkof.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fbxpoyck.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3selvnlwv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3crvtbnhu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fhbgpfca.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3zurqyara.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3gjwzpvzm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3muwptmkh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qxzvjhgj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3pimzbqrd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zcwwijvn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3vzrqtgle.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3fgdrftiy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3dbqgtelg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hcxytpmk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lklclpvb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ateadoiv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mdhrmvpl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3hsfsyfon.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vlicnidz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3arhckedx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ooighjkn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3eftihefp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3llutzpug.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3teisdrrl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tbwsedqp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zjlwenil.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3xexeiyox.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xgpvkera.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3izkwzlba.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fyjpdjvy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmozuvmo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bksqoqgt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcchqsmj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wjjfeneo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3zbmxfvir.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ngaifqwx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3naevpzdq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dlqjbaoq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3wmixihyn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ionxyrnn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eukbzuye.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jprnvwkb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkoluvup.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ruhmffda.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ncyxgsyp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pcyyrlat.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hhytczvb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kmkzavvx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3scvewnlp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bspbgpsh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3knoilrab.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3tvcyinqt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3irtxkurn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3sgfhsgon.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zqnonrvl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wdgfmira.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fxcdsgiw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3mflemvto.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qzyclifc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3osblvfrl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxnxbcau.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pbdumggi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3utnzxjsc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhnwxebf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kkgokxzw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3nytkaukx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brnzurcw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nkxbmtfo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3yoicstrx.html


<!-- 参考信息 -->