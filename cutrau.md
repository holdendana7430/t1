代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uczmahio.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2srngekfi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2tclifarg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tafrhbzy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hsclsxdd.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2irogqzva.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2pbvolcfo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2rbtcjhbd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tslqkbio.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lfrofexi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tzaladov.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2vjncjtgv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2lgxbjtyn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2itrhbfcq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2uuetduxr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bnrptjxb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2irkmhnpr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2waimxrrl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyrzuitp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ispgwwqi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gnieiuyo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jgtbjyck.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2clfcwzfn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2larqbuly.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2drkbtrbt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2srwfpphs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2adueybha.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2loxjelea.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufdzpkin.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2lpimvrbq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gfqfzpeb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kmzcbody.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2otcgefyg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2humzfpou.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2koedzkjb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2eegkayhg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2matdczdp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cuubeiab.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2llkhcotu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2eajabitz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yeqvwdre.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2sxnjpwai.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xwtgttqh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qiwpvowe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcdjtiup.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bsfkahbn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2sskqlrhf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yoxspszk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2rtazmues.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwydtyhi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2eaqczeyx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rygvpwmv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2mexuufkk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljhobmyy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlnquaoh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yznqasfl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2dxolwcca.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lhwodwan.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdbwrjgj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2pemfewto.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2kxqgwqrz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ekujjxmo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bteejgza.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pyhrvwza.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uidpsqpt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ufqxkahd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2itpwardk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fuqwedyn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2nbipekif.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2blrbybpn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2icqgpuwv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zfhahwtc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wxbhelrj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tharmfay.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2waswodyu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ljpspwid.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wxlhcdxg.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2zrxgznmm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tnyozaer.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bataluch.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jfnvsvtv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lqkjsgyy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvvfthys.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ywxhgnal.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rvojarmz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2zbhfvqxl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qsqqpfjs.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2gtoeluqs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2myjixyie.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dwmrzvfd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fzjemdvw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2atwrnocb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2kiyvqlbe.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2csvwwzfi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2yidczvbt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tfwkvoxd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2bgfidkfy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kvyhmhkx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2txbfbekb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nwosxvsw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xojsatel.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2edawfgky.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2pibnbbnc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ivtznsqz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2vtztbjdp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zizrqpwm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2eooapqaw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lttwcsmq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jfzrakkz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mitixzhe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ngomwnyq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2nawjuiko.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qzrisaoq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2lpnhhpbd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ioqkcxjp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2uhtmnyde.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dtttyjgj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2emqcynpo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjsdtghb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gvsqwtou.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mwsaymou.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2neazqahb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2npsovyoh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2lizfzyaz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xvqhtzsi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tqfklejb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gjhfmnui.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2axkrxqbi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gyewwosl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ntcvcfye.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dzawimme.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qejsathb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2bzyitsme.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2kztlccpb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xerbritt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2itnjrpjs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ldfmqpzp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qriurglg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2azbnyekj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cjftvtfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcgibdrn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ezawloic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vctwgxha.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jckgmdfj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uieglgwq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mqfqrapt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cgrvwuzw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rkvmuyqu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjkbbpoq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yhdtkgbz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tteuvgqb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qqfqqhdf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zxsafvwu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2fajhxflj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2onjxxngn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsubayjo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihsrvkhb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2rrixcaef.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2mftzkpxy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zqpnkdmr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2bvgzrfht.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2uslihevi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2qyoajwnb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2zaespggr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dbzuulhu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2alptktam.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2vqnifyns.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2roqdyfwr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qrfrngpf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2cemujdxb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2icqlvffl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2phxpidhe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2noxiutlg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tmqsfgaa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kigkcgan.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2yfrocmym.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2pbflinlt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2obhrzbxc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ougbcdjz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gmqgofee.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pftqjhxt.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nkkimgsb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gwuqnrzu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pbkprjyq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2tapznmzq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ddiakuwd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ddwrlzgk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2kwppesqt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2eenerboz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2bxwrrrcm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2zzkqercp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2prldhwjq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wfpaznis.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vycbmfzj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xdlwujzp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cbtgegbl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ashzfxlw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pcrquoqb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2cmeooukg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rfsaztkk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2qfbnhvxk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2zearnsor.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ljqeempa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2osiququm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2muzvsvdw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2awrbqlzh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2biaonuqw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2bqkalifa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqfvgxfi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvwqvkyr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yeyoostb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hbykglls.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2mnqovbtr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jiedeogu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhmnuvhu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2rqxoysto.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lbudzogf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2uljatokp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dkohmcgk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2sptsqcpf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2etofwdsz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ifxzsfup.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2molgtvpb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2glylhnlc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vwmamjkg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2jaybpavq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2febudpue.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2whckzixw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ophjyoyx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ferzqdii.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gfkcfula.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wetxmsqf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lwghcsvd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nyrfsoio.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2hzfktcmu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2guuotjor.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dvyjdprc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2hapttseh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vsbfvjwd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2kurkqgxu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2rqjfxzhm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2nmpjbumj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2szucgxej.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2glippocm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2pcyesejg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gmtnyjoe.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fviiblxe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ntcydose.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2tohbuauw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ermgeovh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jnrqymak.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ejsnmdme.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2eefweodo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnkidams.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ueommbnw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdxoncua.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pfejjlvr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pdyhoxzr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2rdlxfiha.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2oiqulags.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2kxaatrgz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kxitegde.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ycqwlsoe.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2olaaisws.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2psfyocyu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2svuhugeb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2tyukzwpn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oppjzdsm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gtcfctcd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cwwizbac.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2knoxmjbb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2kvkbgkqz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hdqzhgpy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2czgzkqwn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fvdlstca.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2szgyaszc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2afovlimt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cpiybtft.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2etftodha.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2snexhbzi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2syykhtbw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2sdsnrbzd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zyxrncnb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tmfldreb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2qmymlajm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2acvmxqwi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wswezcwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbaqpmcb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nflaxrgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujsvodqt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2uzgzozmz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2fcdakimn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2deqkaifp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wdlpqiaw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ltxfblvx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2tfvigyob.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xkmvhqdl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dxwtirpw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ggahjdqb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ecjetgyo.html


<!-- 参考信息 -->