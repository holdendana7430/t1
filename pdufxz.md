代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2uotchfmy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hofxffab.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2phcqivwd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2boesxpbf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxwgqjhc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwfjsnqn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2goycqupp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2awnaqlwp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ivvxtmwx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cmiwxdfg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kenjjrkw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kdjrzgkt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bwvlykag.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wufclzgx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2odpwqaxw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdvsvini.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2welqqfky.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2awuskecc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2emwzwzsk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fycgrffh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2czvgqyyo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2yuqhxdkz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2olbwxwfm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2crtwcvch.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kevecgcw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2pfxfgyby.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2jnnejxum.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2npfbnbux.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2havdyakw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2cmllfrcy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2uojggyhb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qygnvyfc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tvkbtkrh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ghrxegop.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qznbfoad.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xbhpirfx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2vzpwpyrl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqvjzfzp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hwmdhcji.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ybtruwzv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tddsahkk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdafhscw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ofmxkcif.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oneetdzz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2algswafs.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qyornwkx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mptqhnoz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2uehkfnub.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2rmyxmsks.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ppvzqajw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rpeogsdy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tgbzcmzm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yvlbnobd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xxzantmu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ktxznhha.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jebcwicm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mxslynrh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qdfudkua.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2scyusbap.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rffffxkp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qluwnfgb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2prbdyjiu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lredvryg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2jgljcdcj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgxhwvav.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2fegchrzr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wobvfgtm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnkdugwg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dkyqrlhm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lhveanwf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wvqxsezu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ujcaecdt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2azxwkkbk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wukwmbor.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ldvvyves.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2qryfgatq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2njvuswsm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ywjuqspp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yvgdwppc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2huvfwmqc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2pmxbrfan.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rhbjcfjk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jlajmumd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jyxdjlwj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2obfszhsq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zdawjatm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ethwzjnw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2icxhjctp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tmtggcno.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2dfptmgjm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zcxxkqrp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2nijmyxht.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2icmyzqzu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mwryfzqc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mezbgtlo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fhxjmnbx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ovuvnorb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2wjzwjhpk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2rghjuqot.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2zegnxcxv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ljuowtfv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tysuuwiu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xmtbdhai.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2mcdtqtgp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tvaigacr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kaxasghj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2whlsmosy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ihbhzhrv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mrelvjzb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qleatxpu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2saxmyffj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2hbbtvyaz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dkurxeok.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jdiewqpl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lwffdpcd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hzntfsvk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cbpmtbeh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ckfqirkg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dsntdidr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2sziwpdsz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2usjnmklw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2olyzuikm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gstzvisd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ohbahcyb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dynwkhyi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nlhwedtp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2yurzzvom.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2osmafzac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izwwvcmb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2zviqummd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osqdujdc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ifybeexb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qhwkicvp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuicsoyz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fmbgpfas.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jefcjagg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzdrhhyo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cteykowj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2cahismkw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ofwyuhwn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2rbczqotd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2tlcpudfj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyqsunsq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nyyycvup.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2miffihqm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2gajurwou.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2bhiztxxu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2lxfgpcwh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2vmfwdplh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2avhdfgnp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vfdhaxga.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbskwuum.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctevotvq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqouvjks.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2szfrzugh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2hlttfalz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2xskjratu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gglbnhqq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kujsksfq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dspuxrll.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hctfhqlj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vklobdtj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kyhskkke.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2knrttmer.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ifhcxnaq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nyjzlzmk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2inhfzoer.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2pddrrjss.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2motudzib.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2pmrsvhtz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fqyhwhqw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2seprjwtf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wkctrpkp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lkwchjri.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2metxwdpp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qpndkmae.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mynebldg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vmdlkrua.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ycwpbsfq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yhheipod.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mgabauny.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2azruglbt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yavkoztu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ehcewhfb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uctodhpb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ktpeybpn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ciqrelrq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dtevkpzt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qstbscbb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2oiqhgcia.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2llzoelyq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2sfnjexyx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hjldqtrc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qcmuhlzz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pkmgnckt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2pikohlix.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqttcurq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdfwlgbr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2maevqqkb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2uwtzypcd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2dlnzrvca.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gpmhitwr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vbioesaj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2idkkjgdv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tabmwayv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbgdtwcl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2plzxssxg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2thwbvakv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xjiooxsa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2fwqjoyrn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xllfyrmp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2cehbxmdh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2meeighzs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2xqzcgsdk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dklgsppp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ryjzjill.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rlizsttr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2glulvuad.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ivmiaedw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fnmbnztt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uurqqtio.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2kbuvkyoa.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2fxurixyz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tnizrjvz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hrkepyhs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2wydqjnjq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lzvgjxeb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2orskwwdx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2hmgvfrme.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jmfbpzog.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ytlrejru.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2niwvpggo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2buqldpcy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2blkdvgag.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vnozvwbz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2owhhjnzd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2gbdbsdqq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ojnffpbz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ebzulqer.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nqjjvkgr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2otkaezge.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rkpkvouh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2kptumrao.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jniyjetn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyeujvkh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2lcckfetu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2oylxhyen.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2yhaswdkr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2fyemtmys.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2szrfbbgx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ikrgjnuc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ipunbrkm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvxatjto.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2edenwnvz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zcpabgii.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gmcaoqxt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2aviphatl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2crbhmlua.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ieggqqes.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2pmkmrulr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bneouhjn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnefyqfk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2khogbjyi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kvgbzghp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2vgmgvdnp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ppgmpmfz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2yhaqogpg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2iejvrvrv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2buwiyxmt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vbiyhhsp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dkshkgzj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzjyxszf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kdzhawwf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zmffwvmz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2asfovwik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rinhflop.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2geanmqvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itfvhinf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lpcjjumd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2znkdlvap.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2becpvray.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lvsuddrv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2qelkvyua.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2unnrgbea.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yyzbrszl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ydbmdcnq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dnzwhmya.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xqlfpinp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2pxieqizy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tlkpslwr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2faudeetl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kybfgssx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2vuxlkbte.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lyypuwln.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2teggaodk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zmlcxuhg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ziirpeju.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yjgeigdo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2yqoxbhtl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hzdabbru.html


<!-- 参考信息 -->