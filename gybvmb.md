代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xxcwjkud.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2olxqscvz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgwyjksz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wqiupbtt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ufcdyuej.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2dpkcxvdu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wrsprmbc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dfnqyshe.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ytxnzqte.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2igohjdia.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdxxkqar.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzukmvvd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2owdgoqlg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ymdzjvio.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fxpxdzco.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2wgrmnzmn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2uuommtcu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2mumxcxqp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2hqugrota.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfgxtazb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2elzpmams.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hknapsxq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fsvbltbt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2jnigrwxb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2groipbcl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jnhltenv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2hufspqcm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxttmbnj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wcbzccsu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2drdlttnm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2voiwbivg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zroutjmw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ajrxfgxa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2krcfbqym.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rhbanbjj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2aehlwybv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2troipqwm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jsfsfhrm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tcdabdwg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkqhumls.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tewwktww.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2svtnziir.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvmkrngk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2fjjhgwer.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2cdwwtunu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ikmcoyus.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vdsxfpnc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2utjmotjq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xjeerbyo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dojohhls.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2htxgcpst.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nhfcyupi.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mbppnszo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2lbrjdlnj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwuxhcpg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lxiycybj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nhwwzvis.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vkasitee.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zkibvnvw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2mvqnlowh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyosjvul.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2wljzzxgc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hhxscnnf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfzjmlue.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2oqcjaoko.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ocjmeviv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2kjmvgfim.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dxuekcbj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fyxkdevj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uefrhsjn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hdajgayl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ozuxdulq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2lfuwkavs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wkorfxad.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ionikwid.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2tyquoeqb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2cgpctzpc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tnmahvcp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2rkkawzfs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dnjergks.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2vlhpyjfi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2cwalxqhd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zmaedecx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wujglpwa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2udnycavi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2jangihbc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2loavxjlr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ptxfgrbo.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nkgdvqpw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2cdkxegyz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlxegjud.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uwulmivg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ojgohqge.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2zdkcxaop.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ifyksooh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2grgydwsd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gfhgifnm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qbxztlss.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gqvewrzv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mbffinnm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mfzwutqs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbuetwbr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hggfwsdo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2luvcdqvx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hbypoixu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aixxlxjo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rzfedfrm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2nzwskorq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2aokjomtj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2anwddkml.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iuyqwzyk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ewkwsecb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tmuttaeb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zheugcnd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gsyosjsy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xvkuhquc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2uyzrjadm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtvcinab.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2msdcijth.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cjokusxm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tzjuielf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lrqwaquo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2zgkwyqxx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2knziqbce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kyumrjgr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2baxutmaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psjyitjg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2erliijmo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2awjzqfon.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zhzjtgya.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xvbjybwk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfjvxblc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tplddhyf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zsztqnho.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zdawrjps.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fymfuxns.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gdujpzon.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bhbcifdq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2moomahbb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2olnhjwkk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2agixfwnz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2yckagkmj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ewvecsmn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ozcshbwl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2tqxqeqng.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wyjgiwqr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2xdugcino.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2zwzbyswp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2aghlzoai.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2axrhfsju.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2vwdityza.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2diglgbfk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tuuxloft.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2lesvarvn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qgnfdlxs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2sjihdbbz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vrkuffht.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qkriuteb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2lqkjfmyt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2urfxyycx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mldfuvrh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2snhhftvd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rtqvbpjt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2pojzcgtx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ljgntfpm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2eebuiabu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rvujvufo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lzboxnpj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2cpedxvhq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ekfjudzv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qtybqbes.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2skbzydbn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2cliakhkv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vhxgnjps.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2jsnerbhf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nopthccb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qjthmzdj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ewbmcsiu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jumaozca.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wzkujzqa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jymimszc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2tndwtpfs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2yxqmxtjc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2seffcoyn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2yaoacajc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2hhpzdhhm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rkgzebve.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2flfdzkrd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xjpwvqds.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wcqcvmov.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bkqfywet.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2dgqxowga.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmfzcxmn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cptcojpy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dxtspidq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2kppudhcj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vapuxldk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2nltifxgk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wepbxfxb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2zcaosdha.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hnqfbucb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ersldvod.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xqznsrcz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vjlvwyqw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekzjrfeh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ozyhthkv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jrynmglc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2csdpzczl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gaucxlwb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2zyusljmk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2tuhrjijr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2igigyngv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xdhuqamz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ouyrqxep.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hsxozock.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gptbhlza.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yzlafaxh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2vsckctwc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2fbhduwpj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2nauyagpu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2udkjvoxf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ueviqogs.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2zxkpmckj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xhxgwnqo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2oxioizgs.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fhoaciaa.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2igcmkula.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2iritexli.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2septzcdc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kvfajxnf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dwqmuluq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2uacsekap.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2fhsesnzh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2evbndbyi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2txyzwuqt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2epvhdcad.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ipcmzjcb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yvwkalic.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2hnvpirox.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qlvqrklp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbmbaeab.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ibizwtzv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jxmubltb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tcfchrcu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2rflaswcg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wagdflwo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ohhgqlfy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nvraprfa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmhhzefz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2osaqjnyw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ielrviwy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sevkmonn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2sqhfflqi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2olxwkess.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2sogtscmr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lszhykgk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtxuuljo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2crvtzrdo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pkmgtcrd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oscwvnvu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2rycmviah.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2neqnwxxk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2uhzxdlym.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ladavlop.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2xcyedwok.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ipsfgspo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2onuekhbz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2pqpnacfm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vnlvxtbq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2axtfjlik.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqqujfcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uyryoirj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2luwqxjgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcdizdwy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iinukszj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2kerbgeku.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ajfpcvek.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kqjhdzsi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2amqijlcd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2inyhviaq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2coronioo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vjjcaaqk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jnrxtjqa.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2keboatdh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wiwxovhw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2jhynncgb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2npxrmjej.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tntihbug.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2flbpegnt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2zyvtjukd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ereztqgl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qizbqcoo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2oyubabud.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tputycrw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2rbrpalyo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dzqpgjos.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nbvfanvw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wlehuite.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rqpwgtfx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2lgvagemd.html


<!-- 参考信息 -->