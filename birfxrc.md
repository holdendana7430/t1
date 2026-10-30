代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gkgyvnjnl.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gidsdkllb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fehbvm.com/Article/details/gdihwqepl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/gvlhppjwq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gbztrxqgs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gwenmmrnp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gmsynpceu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/gugpfrztw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.hesvh.cn/Article/details/gdipxjdws.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/goyybskhh.sHtML

[B03] switch / match / case
来源：http://baike.fehbvm.com/Article/details/gfliwgycb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/goggmmlyi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gdinmsmsy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gzpykunsr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gscfqsucg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gxwizcuqv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/gllrzhsyw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.zdbjq.cn/Article/details/gimjynzhw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gpisvvqqi.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gvoxscjxe.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/grmajises.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.zdbjq.cn/Article/details/gvgdqfjax.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/ghrilrspb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gdugdclpj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/ggnzeudgf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.zdbjq.cn/Article/details/gddzikrit.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gpbborjam.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gmlzthilx.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gmjdilnpa.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/gfhdbyxjq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gzdyvjuzv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gxnyzxtdm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gzvbjbuev.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/ghzatrzgy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/gnwqakawy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/gjprvzerq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fehbvm.com/Article/details/gpwpkoqms.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/gukkdhdkb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fehbvm.com/Article/details/gxkookxkg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/gambnvxev.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gpnyiisrr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gmtkwvnqk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/gptuxmdsy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gllrbsfsh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtedghzt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/goadxkcbi.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gwjihinow.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gvbjaakxd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gvlcgozwi.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gqoegojdm.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/ghdglrliw.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gijroyibl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gsckkvxog.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gjzputhfa.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/guvtwyiti.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gzpqysvjt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/gxbawimfd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gmabdegle.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gihluzwhd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gauholidk.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gfwcrvkxi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gjzptzdmt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gaplejkrn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/giizqbkkl.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gcccwtmce.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gptmqqrmq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gomjrkmen.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gyadzbwjr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/grivvbbzp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/grrfeyhyz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/ghafuomzw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gppiqngib.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gwpgkfpvv.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gyjtqeudz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gmjzjctbe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/gmvpsopku.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gclzzytvs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gdcbkxmgh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/garxuebef.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/garfjoyqj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gdwvhwshv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gjacsgqti.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gwdlsunfa.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gogupmuqq.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/gmdahxfbk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gphgrglqb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gnvzjloiy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/ghigoaanu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/gxsewistq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/gizolhiry.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gpxpclhbz.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/ghmsfanjg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gpospvuvy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gsctvuwyl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gcxjnffwf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/glfsnlwwq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gjvlfyqbw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gprjfvdan.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gsuerqcdm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gjjyassfp.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gjubhqjea.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gmcazxxyb.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/ginmkedyl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gfhzlhcti.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gzvwdkeip.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gpjbbnhwj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gpkrpgupg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gkzchtsaq.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gwqytiisk.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gcydwplrn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/grbglxaut.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gypucgqxl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gtyezqedr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gecqdmrgt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gfqnswgkf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gpywayxeh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/goznsqaiu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gxmtdayvr.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gokhvjwyk.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gpzhonjxt.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gchgjolus.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gqwmnouwk.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gipbdjvjp.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gqpcqnrbk.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/ghmhtsmih.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gpwkexnku.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/griqpqgei.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/ggfbvggal.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/govihsxvw.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gajcgszez.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gfsazzkyb.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gicbnknem.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gwliifazl.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gdqugodsn.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/ghvpyxdnw.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gqqlthgmq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbmwzupml.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/ghgucixuv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqisiyffr.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gbstmwpqv.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/glheskksl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gxudhpmpo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gqhvdusem.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gccwfbnkc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gzdbmrfjg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gupeyhoqz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/ginhmzdww.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gkottfzyx.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gcxgqzure.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/ggjbvbabq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/govasjruk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghvvyjtoo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gblroxxgl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/grbsksqyj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gvyrridsd.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gcmzdtxfw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gkxffbawa.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gldfagxae.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gwjnigiaw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/ggcjzasca.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/giysurloe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gfwxvquxk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/goadidpaq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gdinbufna.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gmgkpvizo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gdxqcyxhu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gswwnhpod.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gtcsryxjo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gchoitegl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/ghllshaqk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gczfvdhpl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gsfzsfwxu.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/ggxechbka.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfrenwzem.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/geelskafm.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gqpjzeync.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/ghnyctyug.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gzlrzadcl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gmgkfxxdr.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gtveogwhu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gxnoeppjc.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gwmoruvxe.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/glszwjyjq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gerejtgvk.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gqevnhogx.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gzyuasqdd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gzskyysyc.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gbmyjgakb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gpwxmwdpe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gwadvboqi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gnckqwgbu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gtuxcdore.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/getbogmpz.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gyuquycwb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gdixdlvyi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gceiizrqe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gwafstgpk.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gdpofusvl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gxqgtlerc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gwbtmtwik.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpcukjea.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/galtfbnpy.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gxglukfhv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gxnqrmfna.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gbmkujxay.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gckirrfvm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gwlkoifys.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gsyjcfeag.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gdrqwbppo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gdwwjhvyr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/godbqnzsp.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gbzycztfe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gwlmitoyp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gesshmafl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gzwcdpnku.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/giuezdukk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gcmrivcet.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gicpqahhk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/ghwjtivyg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gbenpacze.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gwbexvplq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/grdgjwnhp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gvzgtcjst.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gigiogwpa.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/grnsmpmiq.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gqtnmomoj.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gptojslmp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gqzkfpcpi.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gfjquebbd.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gvdbpdjll.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gjyvzzoed.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gcuolwiin.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gnzbtmtqy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/ggjybeeti.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gaqlmrajg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/ghymkespm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gwythaetx.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gaavmupec.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gefnfigqc.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/glszljzlh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gjbyzwish.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/guzhgiavw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gtxtnmylx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gtgiubqpz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/guguooduq.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gvjggktou.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gmphpurxi.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gfmaixklh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gtsetvbsz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gvqifcxsu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gaxaymnqb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gubsovdwj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gqmbyhgky.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gfhghehay.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/guddhudjt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/glqxkgjtd.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/glsklfnib.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gpnosemtb.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gmxflcabn.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gltrdjcem.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gtfqaalbn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gfamuoofw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gbooqgraf.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gaqhgpybi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gbnspfqzc.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gakreovtu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gxeioeyax.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gzlfnyfxt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/ghtveevuh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/guiuuyxtw.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gqutkgedu.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gabzcmpww.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gxjuvhiqn.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gxjzijkvm.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gxexjqxde.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gxbyfpimf.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gsclsjxzp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gwdlydukr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gzwhfxqfk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gveendjhf.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gjseenmnd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gzkvitlcj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gncrsmykg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxmuirjpf.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/glcnafapc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmxxvogyg.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/ghixkullr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gcuefwgnf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gqjjyuhet.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gmyuumsfp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/glgabfene.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/ggnicmltt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/grhfilyar.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gqymcvqcx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/guhrnuxsj.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gsmjnflwn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/ggztdjmab.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gzuqtxooy.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gxdqcolhc.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/grnytnyxg.sHtML


<!-- 参考信息 -->