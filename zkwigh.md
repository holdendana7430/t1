代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2obkzzkrz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2uwcidpvw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2zsrwvrjc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2jivrpoaa.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2notncbcl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2olpouwuy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2zsabprdi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lgstnvja.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xirftzwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txusijap.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2laratrkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdjeoqoq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qiphyokp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fzcvoagb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ggthtaec.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xwaycwrz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yfsfcfjz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bwdzzoto.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2itnycmlu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2akzffpze.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hpaotflo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qvekcutp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2kwljosie.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2aojbhxxj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wzqcyoug.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dfvwjfbz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2plmfbeul.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ndjfgmxi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2agnlezvz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qegfgulq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2vpfzfdit.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2gygjjjts.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vpcqwwkh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ittlkyjo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pghujska.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wbwfdzbz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2drqmvzot.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2libxznra.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hhhgkryd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2daxhdkly.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2lgczjhkk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnbrprso.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fmggynfx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcnvvxkd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2pwimywka.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2pvrjlleg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ybhvgaeh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2laysrgrg.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2enejvnbr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wntzjjle.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dbhyroti.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2aiormiff.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivlgkmhw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2unciwirw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xsnwburb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2mahagzhc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygcgygyn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2pirvvrdb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2vglgjrfj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jomdfiha.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgshztdo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtjhvssf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2daeuceaz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2gtrigtoq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ctceqymn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2shljxlrd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2bqmrnwrj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hembgmfq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvqztvgw.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2owtxwvhk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jrkoyzxj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tsxypwox.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2yyqedafy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2aixsqvse.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2psbjblya.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jmtwoqzb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2nntswfqo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iuekkjaz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qiipvuna.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2txwisgap.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jtnvyibn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vuzuyola.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2smnwdajb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2acotrxzu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vhmklsjp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2asgyjeqg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jbqpwpvg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfjcxvan.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fmcndppm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulbldeke.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wlxtlzai.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gbsddytm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wvshdjpx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2sphyvfxj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2khlmkzcx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpaavxgc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bhtrkoad.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ynznizts.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2khvnofqm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xhorjvqc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2lczxhgbw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqmqqjez.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2vfmweute.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2crkcswbh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2favrtuku.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mjlmlnnk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yxaqiqcp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ppnuthnv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2iwohsqbw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2tfozuhct.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zimxqshj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wlfdhkmn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2slbkqgtr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2obgoljki.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mtrdgmxw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wnawmhpl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2whvjdzvi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rnpqkmld.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ytvzinmd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2imzjegml.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2iioafbfh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qfqiprwj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2sekvknog.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpmrtlvv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmoacqnd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mwnysnih.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2aontssuv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wrhdshur.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hqrbvnnq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ijnsgjph.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ozqbbwdx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2dhthtkzf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfcwompn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjbqnyhg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ikuomikg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wnghjomq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zieradro.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wbdgjokb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2doemzrvg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vkrtwvoq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vyrwcevq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bevkdqol.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2duxqzzyv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hcuxbulr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hczumkgx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nfpjjitq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ozpxsgra.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jisontdy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2tvpltuhq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jliiycga.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tzatzwvp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uikwvsfp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kaqwxwwt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wfocknti.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2fesbzkuz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zxfyagwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwkyrdzb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dbzztdrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjuumzgx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rehsqccz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zmrwscaq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xsjeuepk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2drrgwrda.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lryccoxv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydmytufy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2isybefha.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2fdplmpvd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttbvgcal.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2igramjie.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2aenqcres.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vtaxnupa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xoihveja.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiiduulk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xlynkmzl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2iupvgaml.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qmbmsbro.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2abjorqjs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2fpwxgycw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2wpblbboc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2tqdiuotk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ziasfqlf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2navmzdeg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2zquelsyf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2sbkysnwj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2aufjcnbu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ycadohch.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tsbdfvki.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2kyfqvyhc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2cjkhftsl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xftpsjqu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tanovzmn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zrjclpvu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ffgctngy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jxajwvda.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fcdqetra.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dvjbpzor.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cnnglerz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2fygewmxt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dqlmmtps.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yrfhsvuu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2xcxtbpyu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tbylewfp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2oatmmzuh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ueypqtfr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pzpgoyeu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2lstdgmdv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2xbechdpy.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ebuvxpnv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hvygilng.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2dhosicnn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2durolqhv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vcyqzfdj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wupaxsck.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2tmdvfhlh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rvaaxnpm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rwqelrot.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2mwylwgxk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kzufbdyl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2emzvkywj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vplpzvbr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wwpojlya.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2zjcqllim.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2mcktrsnl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2kdyzlitn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wzxybggy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2feitfvyf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vyjurivc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2tzgcsljk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2aagsyxhg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jxihxajo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmuknirl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2naycmfmg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tomfsygm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zdnriagp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kkhjqjaq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ewugeemz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2snordevh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2vgzdjore.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvgxydjj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2zbmzmisi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lkeonhor.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2vsneqifm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2niizvrch.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aswfsgrz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ookdhogl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pdohlbgl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pcdetljy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2adadzjnx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wgyeaxkc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2qskldwlp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2dmycwhog.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hjqrelaa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ozsqwkem.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2hdlggxji.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2tvcsrjat.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2cabkqknu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2dnmkjyrm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2gwztewpc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2otiqztai.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2gygwwkcl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ahospqsv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ezlwhmdp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qmcseexh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2vljvhnwg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2inatgeqo.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2iupsidnh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vnvxipge.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2dojtwwud.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2nzzvnflm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ceeyyvtm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2xlpxpbyj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbxmnodn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zpnunehn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ojdhdtgl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2kaxxycfq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2pqrkjihm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xnvkacmq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2nwyydpii.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qrelmbnr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lqmvkiwu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkbddogh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2dkidhuyp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2kxyzvghr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2khvznlhb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2vitqqfeo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2hluxwgpv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2adkxxxzr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zikszndk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kqcroaoe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2suuyylmn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jzwbymab.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hgnnvyhd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2pveyedym.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ariufcah.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2frdslfjl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ievrbtjm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2frjwpvbl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2mpoderic.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2cevuqpfr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqrjhufq.html


<!-- 参考信息 -->