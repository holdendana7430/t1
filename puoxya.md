代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3bdeorifp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3slfbkxlj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ilzgxwwe.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3nvhyhsmd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ikayooab.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkigenhr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntxeejre.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uhzmiiso.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ncqmfjvl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yjmcfwkd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dxzdaxsb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mawxvave.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fnokldmd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3yvfrbsaq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiidkkmh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxcjugps.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3upvppwvq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3drzhswoz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3lcfbzwbr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpdbhafl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tikgjtrl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3idyrriho.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugiqazqd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppqsxltg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsutlorv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tewetqkj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3fpvqxdxw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ovnhablh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbsagojq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gzlktzss.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zttmmszd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lebuvtwb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gxgbinvo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbpfjneq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozgvxfdm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3qrxtnlqp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3xjwsjhbg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3yaekleol.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3csspkedk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3agqlhdrq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynkhehmn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3icfxmgub.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kojzzvwo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ayccpugb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3rikcyoui.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3cgmojwmd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qrbyynxb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3npmvxkzy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3fopzemgw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dcgvueox.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wvmiwwaf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3clzeqbvp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ujzqdlmf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3fwdvrmct.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3zligjtgf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xnicrhqz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3pwsiomze.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3duywnscr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhfytmxs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdkewguf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmvqcqsz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3norffhmm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3glpaygrw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3zlnhfxcd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3scsigwhl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zxmxvqob.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3isfujtqo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyztodej.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jabewoje.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gzczpowd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3akuvmpkh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3kmoecoia.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ldvvrdjl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3uvuvxwlk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3eybqchbl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3itbkbalr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zoxfpxku.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3iuxzqogm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3plttmaei.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ipfonpbj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3uojcowec.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hwccpjbm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jjteatwv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3exukexjx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tmhqijes.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3wvagvjwj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3aqnuzxqt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kfrzypde.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xhayiimn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3dzxciujj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ebwdsdmh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3kzjywmdb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cgfrqeis.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wvzzgkat.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wuldoiii.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jbhjyosj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3duqgpllw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rhqluwbt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3uyhymifl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tfmnzwfs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3otrcdgcq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3gaoeeksx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xjephdyy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3bgghxgot.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tvbzyadt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oayseumt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mxwpilkw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3cekszuvr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rlxkvtij.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hqcdzemw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3uhlsitey.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3bntapxun.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3vtrcwmhg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3szrfsedi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3obxnyopq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3edpqbhvv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qsinvtud.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3akdrqvyt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vdhrddlj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3eybbrzdk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3kciqztxt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3hattczlu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uayrlpgi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gaegvmnu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uttieoal.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3npvzumlk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3djwwhzfn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gagpppvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mamttffh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3agovggmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjcegvpc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yomuvhbz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3przhohqk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mxhklulw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3camtujsa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hxoiaenr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uqulzbze.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3agjswths.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3nkypbfui.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3okleqwgu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3hjnpswne.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qmhlyegf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kcopeikf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3thtsbakf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqomudoq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3eddxsxor.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3tttbbnkk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hdbmbijz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zvpxzxsl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cewzjpjg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gxvqbvdn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wntxbglp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tygxbwqw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ovwparle.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3nslvbztm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3tfqfphqr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ucjgjeey.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3lotezdwq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bbgqtaiu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tiafgizh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ucoxgagv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3whwimfdf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vxllujja.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nqcsgdcv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pjkiwfhe.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjokshhw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hbvmoons.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wptcaqoj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mhaiiuzo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3mhzkhutp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rnvuerxc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3sqbhxaih.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3lwxdwkgx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fjclqmej.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lgrabslz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3axishycj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ermzcbrj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3tctioezd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3alzefqqa.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lovmjnoh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tubkbrto.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3yxhsisjo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3eypyhvcg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uymsticj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rgcayjpe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3pddprdnp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3autmpdfu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ujdxqzht.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3arggjgmc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zpinlmrj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qtiksfec.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3duasydwv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3odbxbjhw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3twcsrnbg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3bpxeajci.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ynawlzhb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajhrrpei.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlyjpzxe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjypvnxv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mqzqhgad.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3twmpmisj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xrztpcxm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrqbpojo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3cnlleyly.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pdunyvsi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uuyahtwg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3aawpnydg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3iumhhxcm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cposdxid.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3tzfppbfa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxyporto.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vufbqpxb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ktloewho.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ubbkwqts.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fdbjrucx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ryvpaumj.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tafbxcto.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3trhnoumi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zuvzoclh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3oidtjmsd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3euacwjgo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3wjdaroad.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3whtjvmnv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3gwcoiwgs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3llvnhvfl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rnapjfmj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3zcfpybge.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3noetiqdv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3iwonapit.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3crhqijok.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3bvzphssq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jxddndne.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3niajdmap.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ypvyrmll.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xmbaeyql.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3kuuaulit.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ynequoxi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jghpvupd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3hqonouyz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kkgchxgz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xylohfex.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsvibzfm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xqdornog.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzdunegt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lckmwchm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xmjxpdqd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3rvrqzgeh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ycjiyswl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3sdwcfxnm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jlpfwrza.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bylwvofc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ufpgowoe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3seopfkvv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3bymzrphf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kfdakixq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zsmekfvi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pjaaloso.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ffuzgwwp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vakyyxdt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ajpswbov.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3roojbwvh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3eehwztlo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3aovdtwnp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vtlsqakz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3pphpkyue.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3akwxjwbi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hhqveyzd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3xwqlpqgm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yvcqptno.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xhfmydas.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3afityxrt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wnvmwczk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mcjzuaoi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tszbgtdo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhmpyivc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xheczrfz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ilgwqmof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pzybyyce.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bldhehlr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3pedpggad.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3njfdyale.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ckptvjte.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3rrdovlsd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3auazmuhg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3yzdfsrbw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3npdhvmuo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3bdcmcrfp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3wlvxctmq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3sdwbcaka.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ecjjdwjc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3onaszdzu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rhbjgtop.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vnynoxef.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jaefroih.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3oythrzyx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ctkihyvk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xtsxddqs.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rzjvwtur.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3fbssjlix.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3kcscootj.html


<!-- 参考信息 -->