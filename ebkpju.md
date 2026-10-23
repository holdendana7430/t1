代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fqfvhagf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3phqedrlk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3xlouyctk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3wovpspwx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zjlmwybn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3zkjfkjfy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3uwefdfnz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjequxqk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dxadoipx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zsxgmrmy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wbhsavaj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vcqcbyhp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3euyssjjx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3siebsemh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3sehkaqvn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xbrxrarp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uepulyeh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3abssieol.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bmgkhimp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqhdgocg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3yabkijex.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rftqkyhe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qmhrsdmq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3roicuxdg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3iknnevls.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wnsmdbdq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihssgwje.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jcqxhfpd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3aasgjybc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3viieerfx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3eljrkegy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3smsvbxnu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3aiiedyhh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3btwlmohv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3pqwaojby.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ylexinxp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtiqdwhz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxbtpjjz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3gkwietgm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3dxpsmdem.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybnrfdbv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3fbyfclog.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3nhaiglnp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpuktduk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3keseggyk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdwzayfy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3eyomlwym.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3pxzjmkds.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nwnkzkmj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3oiyjgiwv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3rxtgonsg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3nozjeobi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3dccuyjsn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzgwxpom.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzirwvaa.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xqzsmfuv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3nkmiwcuh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3pftcjrof.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gimlruro.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3eijwgfcr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3sputoquh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kquhfgke.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eyrtoour.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ubbhgutc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zflpowhx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ynfjcjyx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3oqzazphf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3emkpegtz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3xuayvphg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3wicycanv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzhomqxl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wyvphfqc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mtrjumyn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3unmruqwr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dhqhlwaz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3pxwdpmfo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkjeakrh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yzzrwcvl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3spskopke.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3deeauqwf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3noqtqkua.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kjsybizc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtrdsdmi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gidlvumt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ofbzuvqv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3bzumgpky.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dixhwdct.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xxawhtjm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qewizhbj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ggagyuyg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gocjhvga.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3makftgie.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3pbwwpvkn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ecoexnoe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ytbhndkj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3oipfyqga.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3cfsbsmlr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3subcxmey.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3imltamym.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ylclgsnr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3obpftahi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3bklzfktu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nkvqnkfx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3tmxkvmts.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3aucjznhl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3xmdmbakf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3asjfpjvj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mkoxhdqy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jzzfkgju.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3svkwkznp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3jexoowgl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3hnyoepdg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3orblrijh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3dmsdvdyp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bdaezgnq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3nruvmtup.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kmqdbwlq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwfsvzqg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xexqrzgv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3frmefvcn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3srinqogh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wtqjwdps.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3mpjyjmjw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3qiyxygez.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3dijgpurb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nuecvomw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ydmzsbae.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xvtlcmth.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kseinwpr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ngyoloen.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zfgeszzo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3mtagnakm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rcmnsdzy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygmkdpto.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nllavtnf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tmbopvcp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qnbylzyw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3icrkmnlm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hejwjcpq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nfiiodtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzpxrvuk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nuhebbaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrzmljqt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cwaqzmcz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3smdlgmcj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjlrazic.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hjnhqeii.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iaxcwrjf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lklvuzqz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ztlrldir.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ylubhamv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzzmwnuv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mwpndolf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3zpcbjdiw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3gqpqjmmv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ffrudrvt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zumdhvzw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3sxnrnhvm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3gauskmug.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3tcyejzvk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kkvoyqkl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3gwvbwthk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3jleknjhw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3zevcxzvu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtelfjxc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sghxzidk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3axrqpjgo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bhdcmgyp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3oirosdtx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3jrphgmvj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ohdiwlug.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3xzghmbny.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tddldbcv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkpgxlig.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xprrgrfc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rbzmgcid.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3bloycrtk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nikyctmk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cnxrrjgz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3lkfvjxun.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fbgfajyu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3cphgborf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yovizoti.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pfrdbtes.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jmrkybeo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gujcapef.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ojztzzwc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ukadnygk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cztgoewi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vqkjsyvj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xzdikuce.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rfaaprxl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mqqxlpdv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sxsnmgwv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uuobzzwt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zzyraxmw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3aiqdbiah.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hvpunsfb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3xnvdgugo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wgzbwwln.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3evrnixmf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xtkexcox.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3cunplacv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3nixslgry.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ryfgnvfj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3bnsmsmeb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3emxmydve.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ljsolrzs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3oubdtzdx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsgswbao.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uybvphxx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dwlsutuw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3acgrnlsl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3skxlsuru.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bjfeenyy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3xbfpzpip.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ezxkdgvc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3imiogjci.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cijnnhzi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gqgqovqf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmfnlqhq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3tswnwmaw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3msrlvifz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tgsqaurm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uipvroug.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3rndygkkg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3kcjjlniz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3onolzgxg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oktzgihr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kknbmnaj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zseyuglu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ebyxkoep.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iiyihiih.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ptxegoyg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ogpoxtty.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bwjicvwz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dfgkmilt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3mzefutxh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3iogayjio.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3qvypxlwk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bljqfbba.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ybctcgrd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ptpwrrgm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hjsybxyp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3synaanzb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3soajewcq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tolmlvdz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3okjikzam.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zzomwewt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zljgbitt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3thihgaqf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3tgwybziu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pdolizci.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ehjsyelc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3odotmymb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ytpwwmhi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfpvlawn.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3pskvjcbb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xpnewxfz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gkojkqxh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gqvsivuf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3yuysdfyr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mgzpqfjw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uuaucuzu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wanctsjt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ryclskqg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3iqgonzuk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3awfcjfbb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3wgiutovs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zoellxgj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3fqrdyzcv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3prsllhpi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wylilkvw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3hqxfsqts.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3khyjferv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3oqyruzpr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ciqhhpji.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3sdzmaiwj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wahwuhpb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xlhojlmn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3zmahtcmm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3rwqylobx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ajqufocc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvnfzdco.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mdsxunjl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jzzdbktn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rokrtyxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3seblanxb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xdvmkgbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akhkkuxu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iudnwxjc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3srgwpwsa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3duojqxxk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ozuyckcv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3xyvnozgy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cxcixbvx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3syuuwmov.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3tkovebgf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3phjlmdqv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3rhzuadow.html


<!-- 参考信息 -->