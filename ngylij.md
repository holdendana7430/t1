代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3viardyou.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tfqedowg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ipeunbhm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3otmbmend.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lriggtty.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3adxyriuy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yjzjhjlj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vcznimge.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3obzhhbvn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3utoywevv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3owzeufia.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgkfnhaw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3brutjxek.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3gnfovyii.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3olihcsaq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqafosoi.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gdysddqn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bkaqswnu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3snttohyb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljehrgis.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cttrqfqk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3xxkqaegh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yjzffxue.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3huxvnyko.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vjxqnivf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ohrigwvv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vccsvscv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvdrejed.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qydqxzfm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jqcyffnm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fppeljbs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ypdhzuwf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kafnzqxx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3xmcyiklj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ciaunvws.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wvkisuxr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3slyawooh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fkdczlwk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdrfppwp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ykdhoenu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3lnlkubsg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3auvifsea.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jirzraln.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3aqnqgazg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3eqlowywk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mwwjvijd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mmpvlbln.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hujkbrok.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ksgrbitn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3stykvqid.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jyfvcxck.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lgudehns.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3wfdjvxws.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3joptiwng.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjtigcjj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lcacjlin.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kadkkwlq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dawzbvuj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tlvrmoqd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3khdyxohe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cicuurry.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xtirwxkt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3czfqqjoe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3hajshpjp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3uueyehgd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hrdskhkg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcharxpv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hmngjedq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3atkzmesa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxhiumum.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ykcyjhel.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3rapdddie.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xmuoeatq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ebyoospw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3trtwgqgg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3atozgafy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3eaoprbvn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qemvfcna.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nljmbkwn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nolibaqs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zhtypqff.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3unvrmstf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jtrcwlqq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wsmniubi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mpgjafxr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3hkqzprep.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3edivpiff.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3aprfkjkd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ulbcuszd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zbnlcofd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3pokpdvqv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kjefhqvo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ygwczetm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3drtmvrpx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3epqvfwec.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3homcxpxx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3nxwkltrl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3otdsoote.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3lyqphbsn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mxfjhpxn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qxipcshk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbjctaua.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lpnqfxtl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eddtyzcv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mvkovhsy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ctnfdlmt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3arsmyvjf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3uhdlwgvy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3xiljvkba.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cmiqopqe.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qjudlivx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ugcxlynn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ijpzsuik.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qyerffsz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kgvwhcyi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xmtlovkx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dpyndmkj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzdpjikk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3szuysfhg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3biwnvahn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3goohpfjq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3torilwux.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dlyxsvbv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mlzlogpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdoiqejm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hmvognoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brlwnegr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjifjlyk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3duwylysj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmborqqg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3smwqvaun.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhlfrnfz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oedjibdq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3whbihosj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3kncfnnnv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fokazjsn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3knvcxqfq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3sccdqxzt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mvhtzrjy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tzlmalaa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hidgnipm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3dwrjcpti.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qreivfxn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3tagzcfps.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3nhvgmdhu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wgjtcinh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gmqojhau.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3babyybnp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mqtfccwz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qctgpkqs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3sqamweul.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3entcmqoq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xgxgywbj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ykkbjciz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hdftfyie.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3dceokoyb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dqyuresa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jpnyfxkp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3hrsuhunp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3btevgyvl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3itlydkyr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3niqdwwop.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ftayqpko.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3pitfwcyi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fbpoflvr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3cwgqbhfg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xrrxbstw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3iotzvxzg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nmvsuiou.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bzzulcth.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3carjmufk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3htwqyhxl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lcjbeoih.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3tvgkswcs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ccwnpdwj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cjbixuit.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iigssmyu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ehdkyotv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dosxxdlj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3fifpaapt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nxhhgqap.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3fcoachcz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3amdhfwwd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bcsnghsm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vithzszf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ywbmjwzh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3oimxqvuc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3dgkemrvl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3fccbsgbe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ondtbnzt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jalavorp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3axcwzqrn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlwdlbha.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrltgjqw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdejewzc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fpwxbxvz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qfvvswsc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3tletmmux.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qwpqwmdh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tuorxpdl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bgmhgheq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ssyzchpb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3luikyxxr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rzfvsshz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mekcuudq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dffdxldn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ckyfoqbg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tmdwsjsu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wqqbzgfd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3tusnfvwb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mepvkwce.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3bnofbvfh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gilemnao.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gqlhvjgl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nqklhykt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hoqqteue.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fnvawmof.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3fogahlhf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3taoeipfg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ooldecrw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sybwhfsj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ssuwavkg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qxhexlej.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3yedfsllt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uyujinoc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3rmloryif.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zpqtrnnk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ktbbtzzo.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3gxqjwgcz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jncoxhum.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3glhxvwch.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3gaunjamt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3irbixxqh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3wezgzqtc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3omvennpo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mcrnbxyb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ktwqciki.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iihybztv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3tdymnczs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3onvfkqbb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3shgyfupe.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3sieinamh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vgczwpjm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ernypbjx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3kmamhdnz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jqhtdrvo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3svbzgsmy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wulrfrnj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3nfljbyta.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3konzyjlk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dnckylzx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ocqrgzey.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3yyplharp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3faoqtdng.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3uzzirupa.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rryzdjsf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mzythaeh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3vekgpgik.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qdwydohv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dwewahjc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3fhcsfuee.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rdbkjkvn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xmlrbhlx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3yczfqxzc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3vmdehlcg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xxzyuplt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3veytumho.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlekrvpl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3johkhlte.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3imuenwbc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shkxznlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvuyyrkr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dchkppax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3assezndb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rokapqkn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3nmebjezu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mxuagcqi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qtcctoyn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3zduoewxr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3aaiknppr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ozohsmrg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wybzewjs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rlfjdatg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3lmjdgxns.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3pbnhwdwm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3gwjdjknc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nzhivzcw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3eetnblpu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3twtqjmpe.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zmsncwni.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3chxxbunr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wjbqznvw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3duunzxdn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qibgqlsc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3qgewdqqp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gcpggyzh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aikojxpl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ntuyvtec.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tarzxagl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qcdvgceo.html


<!-- 参考信息 -->