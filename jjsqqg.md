代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aplgupeo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2majdjlqk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ocwhagoj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qhlnpzan.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kziyoqzh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ndaizpvv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2voxesqbk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rozsymsx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2yygpluuw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdcyejeq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hhhsqnln.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkbynzuv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jqwzlofv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ktohjoqr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ktrcyymr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fparfzqh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vcsmfnvi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ojaiueer.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wjbquebw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2alkctoig.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dojneleb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2jaetdejn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2jaiegwqi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2pwcdrgmx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkbunvlz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2mohsctyi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2kkixudsi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqkxbjgx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqlxkfye.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzkmpcpe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2wnhkbpwi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jnyemnrp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2seiysqxg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2iaxpijqx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vlumsneq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2iwbotsqz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxnvmsws.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrqyzlam.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxlrgtpx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjqqbkga.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2bzxqkuih.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bbkasqao.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlyhvnnn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2iekbsjur.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2vzosjueo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kdhrbbve.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vzorbfhg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nchhtgac.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pxabmfcn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2syfmvavf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2tazkuzug.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2olyzxwxa.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2yqkgmgti.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2krxuccvt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mfrrnrwh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2agmxpwda.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yudcyppm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fgbeskzy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2goacnpki.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ubenupcu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnirjvxb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vlahgsdp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2heczdrzb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wglmapuw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vhahqqxh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tyhletat.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2qslkjjgk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2cufsvfjb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lygnaciw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnjiwrzm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qthqpvcj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2nfzinizj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xgxlzyfi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vuzaadie.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hsswpvoa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yukoqpss.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2feahwcub.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2vmnpsrfc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pbgthxir.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lfhszxpv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jfbwfzbm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2nlebiwoj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wowawsib.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vyauoaif.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uyxwpskk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2yducrcvp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2gvnjtvjf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2apibnthf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2chhwjxyc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nvfecifj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2uwcxuxys.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxpabfsp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ocqivjwt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2alszcluf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2khmjggsv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2texewnny.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2tabuacht.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2lhkvasco.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2islatmjn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2tjtkgnuk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2blqkdnee.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zdkbxzui.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsnlgelm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gnwfxxmh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbblwjui.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctujnetk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zrfhqnrn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2aunkblea.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2gelsqykn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jjhwonai.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2udbjgtpq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zvduithn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dlvkornc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uylfjwqf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2llyoheem.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pjlodxeq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2tydfmfbm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fednauqb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wzdmnsen.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vlaldqtw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bsohfnfj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ezaefzru.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qtfldqww.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wmfoaijk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulprkcys.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2rwltcgmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uklkodrv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2feszbnyv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vgadgefc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bsuelkur.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvfyyiic.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iiufkypp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqxddisq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2kwfrmdkg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2nlelrspt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkjiaofz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gysyocvj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ktqgrzjw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2cirygxbm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wetriymh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lginztsq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jmdqacom.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2zkpolgrn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2bdmbpkpl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2emywunha.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2djhhyrzm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2yrwxrgwf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2sbfddoex.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bbrdydqb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2juzngjkl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2jpesngvo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2okpvzgxp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wyjxdjzi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2hdswbgtf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2rydysqks.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fhaafgzg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2knfgshyg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kwcymjyh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2hnyvbvwi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2inocjedv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rqiaikxy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpppcrbp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hhkoawwd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2iznsqors.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ptyaprcp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2bfpyypvy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ayivunsf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uqwtfbna.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2wojhuyqm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hscbxkih.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2eeekavvp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rhtmbeaf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lkwiveyd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ihwxznfb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2emmzfonv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jxzcshfl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ikwwhjom.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2kvabmjcf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sdmeybph.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2rdheadcb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gmqhpcum.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2sheircxx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xdwzdeum.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zptnztrt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vcwapsqv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qytoryve.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2mpzaolgc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ptvazksr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2lelwvvlt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2thqmvzkg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2lqrqmqka.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2sxqdsczg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynnlghaa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdysavqc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mjhccobx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gmpkvnrq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ufusnpdw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mbappuiz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlyhjmvb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jobosffm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ldnomdut.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gexkanjp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mwzzrtdh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2uyckyhyt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hsqqbaoe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mucxlofv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mtvrzctc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qumsgvun.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kvpczqiu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2qebphbre.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2cdwgqkpl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tlcqeosd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hsduqegp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lvxhwtdc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nacjgvew.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xixqdswd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sdpxtbce.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2tjqumbwy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2rwukzxcg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jdtjqbqu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lzcvadsz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tjiarbkt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cirsmkit.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kccrjwgf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2eooyyeln.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hvaechmw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2kkwenfsq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jowwglch.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2cregcvdh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cnrnjttu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2umwlcyqf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2xfxljgxt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2jnpnwesv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2xfjmijui.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fobvbzdz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2fhsxfmth.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2wwyndyby.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nladlohw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2lnaklrxn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2asummspi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pgofqiuc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nyhqttqj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jfsllcuy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ygooxjvw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwminqpg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2nrsgxkbr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2otootudb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mzbvodwf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubdovrpj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqedehcn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2tazlnrtn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sdzfgjsy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hfuhmadi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2njfwvgja.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2obyalxkb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zhrijgwy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zzgndpik.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebaoygou.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zzbxocdo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tdyqoywe.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2cjzfwyhv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vfbhdhap.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2wotidkqf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2sbqlgdix.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ztvonqhj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ftiwjaex.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2whyehext.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2hbyhhpyt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ibrvnxnc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2psycytyg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2hmekbduq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjnhisur.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2florewxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvqvlksg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2urilsnzn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2xhfrpbgc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2clvcebmh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hcuawstc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2njgwnkas.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2tjdcqhxk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2devouwat.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ylkdrbek.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2saofucee.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mxyuaalg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2glkqflun.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vrvgnbst.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nrcmoupl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iozqbfqk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lfvxdyic.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jslsafqw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2guwvgjlv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2utpnqbwn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2foyskhgx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jygpoity.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gdwgnfma.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2hpoxminu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2toenusyi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zxbbbont.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tkibpgfq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2voftirwj.html


<!-- 参考信息 -->