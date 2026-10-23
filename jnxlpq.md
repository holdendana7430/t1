代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cnxiowxp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3eqfobjfe.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3sxgqbnqx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvgjwvmq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mapyugak.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sffxzwho.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mgnzwhjg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3oncxvstn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ngwccfbg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aznwjbbz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3fcvcijrb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3yjdkfkek.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhwiktqm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxhmesvf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tmouhktr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmwtujgu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3frwagmus.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yfluftnf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3afzdgydk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mqfknsyp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ojvkkdvx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqhbiicj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3roejhjnb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qsvwiwzd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vyarrlxw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nfvbidme.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3pczxvyqg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wuyzhnlf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mpjvlmqf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qsrfpakx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjccvndo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhwgswfh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyfobolm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwjzjpkn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rferqidn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mtumsotg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwayvcwu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3nsdxadyq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jqcpmcvp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpokgvdh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rclhqfjj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3smcjjxqt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3etlardaa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3joyykuaz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3lhqapwok.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mzcqjotw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3qpifbbfo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3xdmgenfq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3dypaguxh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nshbwdhf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hwnyejta.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ejrqmikj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ccgpeisb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kuwsmjos.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdruvjch.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3txpwfufa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3njqudmju.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zsyerisq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kaansivd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ijnpqaur.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pefjhyzp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rztyfklw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3zstdqxeo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dueamsjq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qmtftvom.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3wlicarlj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhutanpp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3znieqqze.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjgwgjgm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouklfyey.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ambgbjxz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3facyzsmm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3liulfkfv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3qzlnrfxl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3kgzzqguo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3prwpawex.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wncfnvwj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rxrgxubd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqnafrjt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3kelbbjsq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3iakzpjdv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xijbwnxb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pkbnosjx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3tixpsuln.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ymoxtklb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rozyscxu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3afcnkfie.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ujqulwzd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3udthkdba.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3eebclcvk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zexeopaq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yjxtdogx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3gmxyodwm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3zfwgkfow.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kbmhbmmu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xdliptrd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3btzebsza.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3eqqbybms.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3agnjfinw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3fdnqyfvy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3aixrfafr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3imtyupyf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tbqlbmxw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkvrdmkp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3byxxzbos.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3kwwonxol.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3amnhwxzq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3uguubwqp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jbkyckun.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jksuyfga.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3rtspuucl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3egugfyok.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxfwyti.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gywhrnzy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxkuvxpb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3shxklnmg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3asugqhkq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3etintdgc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vyklfhcf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3vlnsfiif.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3tmlkvvoh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pksiilow.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gzatxunn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lpatuyyh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3otqlihhj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mndlneir.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ndelvkzb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3nvckpgcc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3iudzycju.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3cvbecjeo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iusrcxpz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nyqyqtoq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ditqjtud.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3frlomsds.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3muofiovh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fpirmrur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwoznxsk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vcowettl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gfcqzylf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ugldqxil.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3qfyokjcd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsaolkjh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvdfvjfi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtrpkbto.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3suqmtzbi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fyvqymkd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3wuzhzqsn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfjlfdwd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sqbjakjn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3vslqjaxw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xutkkcrq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyyelmai.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ozhpmrhv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ryykxzxn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tcveywat.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mqxxkloe.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3tzhmhcwz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3kevgamps.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3tbtstvtd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3lcfrwimt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3aedocfsd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3luibhqux.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3cdkkjmaz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3liisiwia.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3tovkclrs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3znuhcsev.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3cplhckuf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ozmlhvdg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3zkixibdk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxcotfqz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wdaiaqjn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3eoayatrw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3gsnxqgkj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nusdygfn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bsmrawpn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kvlubdxo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gmwygqon.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ptoajpok.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dhwmkncn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xendtatv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ymbierur.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qbyytjvl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3vjqgpuww.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3jfflptam.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uwnntdvb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ecsvqucz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3lntujcix.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qcakwdea.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rdapanyl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3smauemis.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vetpikqb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xzkfrhbg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pqvazgag.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vvvanczt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3norodpfm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jxnypbtf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3duufrijn.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3auyxqmxs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3seaoyjkg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3qqmdffzd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3goxjrwmr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3gnlnojni.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ugrhygoz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ylcwejtn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgovghdf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3trwgflts.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cojdluux.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vuvtqspt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3flyrditq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3zdshwqta.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ozraasll.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3xpaxyfie.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bblhxlui.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldcairzv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fqerrkkz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bmympivn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bzupmnox.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3tejhwbed.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ixwkhyng.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3sruxorfg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zjjnjspy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3exgcnyhp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3symwmqyy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tuobhfhi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3kwvwguiu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ymhbalev.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ayvxvagc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3dmaluovg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3auhgmpwb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dnvprygw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3drfzlpks.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ljmazkeo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tzbxymwb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3heangthk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3feasfban.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3acgqlkht.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3yxkwkfmp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mcuetkxz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qnrhofsh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3gtrcfbke.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vsvzoryf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nnoblgat.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cfoavgsh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3kpwdcomm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hwrckxsa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gtuhpfee.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtepurhv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3dxzexewh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hfhfrnnd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hvkgkmnf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hdrbemas.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghbvbdft.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fgxaljdk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3mgmeqdgw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3cgzxvfjz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xjbcpljp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nrfogczq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kfwldkag.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xcyxacyy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3aamwayib.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qhcttyzf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3smqaogri.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vgwrzzku.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3txfkdcxx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3jkwfkzsc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3teuvheww.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3eblrhndg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yafkpxlp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mtxvckkn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnwhrwjy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tzpdmvyi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dbanmhgq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3robwzmpx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3knlsagxr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dttjatkr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3kcpyrkgb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hzhskloz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nkreuzzn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wsamysth.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3zsvvtchm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3hpriduda.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3wfrehvvc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3bmbfbwde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itdihoqn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3odadrzih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwbcuxfc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wqjiaaak.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3twiedigh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ptyabbhc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kzhdvkym.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dclsltgt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3umxvltxo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3enwpbity.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3vpplvimu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3fvzuksro.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hvjizuyt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3nkyoaevc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gilghnzr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vqshamer.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mdluqzci.html


<!-- 参考信息 -->