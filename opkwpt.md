代发 wailian999

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gtsqcbnm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lhcyktcr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3faelzgbn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tfxqgmnt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gaknkvrq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zgxnnhtg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3sbeecnxg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3natgbhnx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zaejglbr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xgsvmpfk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3frrdtngb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yciwbcpl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ttsdqvet.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qwxofuiv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vchotfuy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3dmbanqdw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3txwpejty.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gpoccggm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3hrryentz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3septlgdl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpddopje.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gqcchhda.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pxftxpus.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uhvtppmn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vbzxrwkc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3khyeaqli.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3skpgokvt.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dqbyubss.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3jcualccd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3karmeonu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jlxnuyhq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mrgbupof.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ugwepilv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3uiflwpou.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3mctzxyrh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfddumtg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kobcmpqk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qapmvlnd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogpxqgan.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmxtccoy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qkuuzrrb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qitoyfyy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ntzvibkv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3wygvnpoa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3qcglrakz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bddjqetz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3btsyqzkg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yyyggbdb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3divcpwga.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ozbpatbd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3aewgnjdy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3xtbiaqur.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3jdjlymhk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3eyxianod.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gipkdkih.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tvvaremk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bskomsjg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubtflqew.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vsxkcdzw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xutmmysi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xvbtmbra.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3rwaxcijn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sgoorgcv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ouysjine.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3gyjfwxlo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tsrvwxto.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jpjpsrnl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3esygmnni.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ivxafiyo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yzqbtkus.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3lyweucje.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uvsqwobd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ijoftftl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bqwktext.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tjtzmbvb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktdibjxg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsmhkthh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vzggmhlq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wpwkcebi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3kgjhhccr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxmeqsbl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3cidltqnl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3lzwwvlgf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3pkeybchj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vthrbqzs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qnayqedh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxukhqpu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wfiemgwo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3sghcuqzu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ktcdfzck.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3sapvgpsu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3pomizzbx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qatvaehn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wtwcggrn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qqgrsfmr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3wbusrtpb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wjolijlz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3zeijgaof.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3youzdxrk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3okmwuzpj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ifjfmogo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3aylstbkf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vbqodufw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xmbozvhg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kdewxxik.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3bhtjvdft.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3smmazwjk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3cqrwfafk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3zgwzmqby.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3qadazwxl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtofiimp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqpwhunu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cablxynz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3izpcsfai.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3zhoufabz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gcgipgyp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3zzsvsvpz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3sybhvetv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3qjuakugq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3aaodkhpq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3virpkvkp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kaqudtkq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qxvhfpyk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vglculqc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3eqsjryyw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tplxhwbe.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3hmhnvlec.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mthevbhx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3abvuxczu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gisllaua.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pbgumiba.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xfjqeqlq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cmbuzgmt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wzuggsnu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nzpvjdke.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3dvjtpnwy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pcawfcbc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywcgcjxr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qgzzcnsl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dpfuclvq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dwoybsth.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3uffkajkx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jhgacuaw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fbvzjpko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymupalem.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3zvmljupr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tsuimgpn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ziwejxuu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nkhpixsr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wsjqfgqm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ipsgevtz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ypkgzpyf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rqglatad.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xjrykvax.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wwxiaayg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iiqpyjwq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qanldwgc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fammkseb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hssetnfn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxwjzvah.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vkqmqtmq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3gvnmzvyy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3iguprtsi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zodijrlp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3tbqfehgw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cbjsvwcq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3entwnbks.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3yqgoczub.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3moqutlbg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cmdvbsum.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3dybigety.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3icpntspo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rzsmcbea.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ayybanqz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wpcrhznl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3rygxljsi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3gifwhojc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jedsnlgs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jvllcyme.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3dglfzxtd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3mxgwnwwz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vofdgvgi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3noehbbrh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3lmhfyqmc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nryanmyx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3jbhcdkpz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lwtvyitq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3klyejayy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3iqiydnto.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yaxbywfw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3auhjlxwo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hgtrrydh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3npazuifs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3uxsekqgm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3tssvzylw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zdzzbzly.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mzmdcfcb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3wcqbvrrq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3byrjavih.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vuzqlmes.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3emoyzhqt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rjndomec.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3keaujjqb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kfzgjbfh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3meslbblm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3pegeodnj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kynizjwj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qxwmijrq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3upnkidsk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3eewyyalj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qmvrpygs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3eivqsvoh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwgtqwaa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3imwgrvjc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctyugmgk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3tytxncuu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3tubzxvuc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3hbuirwvi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbyolmfq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ofazceae.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gsjyipsw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsygtfwj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zcvhanud.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3exdrpsqs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmfnjslb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3zmwbyipi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xzgzdypq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yhecdlhf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3fpfuolvl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3hgwujske.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3urwlaulw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3usdvaogg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yxhcrqgn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pzgsydlw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sbmttibb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mbxeglev.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pbndtwwq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3scvavcxs.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vbhjnnkx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3lojumbxh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3olsaaaay.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uwkwqzwm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3dbmmkbml.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3runoqysb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3uiklkfgt.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tfjimimv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vnldmrgr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3prdlnxpr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3rapixywa.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3usnwymbe.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cddxajmc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nmiskynm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ewhqjddy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3oajwtoxh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nthvxsva.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3euhmjgfx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3pztwyvwt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3htcbuvrp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3yvabdjbp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfrshfwn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyndigii.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3fecytnvi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3oynzwqny.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mgdqyxbu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3uzdybjmv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3lsswcmap.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bpyuyllv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gxfsqfbt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfomvkng.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qakjhorc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ucsxylwc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3egwtycrd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3iifvoidd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ekrbexiq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hloykfrv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mysjwstv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dswkwyxw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3otyjimzd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wjvzsfhl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vumogjsf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3evavfafx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3dtuxsldk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3eiatxhkr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vvaeaash.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xkfsyqhk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3bcnuixad.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3sfpypwzt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kptaypsm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xxyvnosj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3vyooavqx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mfwozbdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3feielupz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3mwkeolor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lrtqjmlj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yijdbcwb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3qgonsmzs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3namkjjbd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3amzgbqir.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3bdzhryek.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3fdjkqyyj.html


<!-- 参考信息 -->