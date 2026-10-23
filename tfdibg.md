代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3exoyttjr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dmxjmibz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hsvndeyu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3rsszpcno.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fxkstxgj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3trpwkoqc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcltaznh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tctiuhdw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lnekddgg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tznjkfma.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3acpcvfys.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xztchkiu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlzvpmjd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3lohoeqzs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zjqysjlf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyxcqqax.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ueitbysp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxofmucy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3xwvzauhf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3djwmaewz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3exqljnpk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3dzxcocpg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ubpttmyg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3fgdsyyqt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3qvfzobai.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3woatokdt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejqzxxkt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tikhjsiu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gtjvgdka.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3wmnrbapa.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykghstyv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3jefxvjia.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ggkjlhbe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jpbmbvyy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qoiulegl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3atrakuzy.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3efdlmbia.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3snqrduah.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wjrsyedd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3llcmhdsm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qmnjkutb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xhgzeoxw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iidppiga.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lxwzxtro.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vpzqbloo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnwkppgz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bhxmmnws.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3jelzwawp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3efwziukr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3fygvonko.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wrdfqhru.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yikhdxap.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3colgonww.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3utfigcki.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfvvxtzd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hldmvaxv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3guxbpvnh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpkkxwja.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3xehkpzdp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3jjlvhuas.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rxqcbgxc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3slccvfrc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nykvkjsr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hmyyoaid.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3eunykrjb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aeizhbdz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ituesmvn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3uutglnab.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3mggbdhdd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3fbgjpbgi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xbcjuyob.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jrhaiakz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fpkozsgr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3sdvdnjov.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hiyjwkio.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nsnpsmde.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3dtesxdtl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vpynmhtn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3xfjnwwfy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nfqtcrby.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mqmyxlop.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qrvuhakj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3nghixcqn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gzbtrldf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xupinbmb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3aqvfbxdk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ohkijulb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3smrcxnuq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tfrziots.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ehudwqsi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgmikpzs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsnfnpvm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vnwbcrec.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yabolbgs.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ptdmekab.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ahlsrenn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ahiienre.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3evwvahxx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zeuvgjmb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qkdunlbz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3umndmcwz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kzmbwheb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zicsttoe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3iuxlzvkf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3trvdqgde.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnwtpdav.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bmxthvuy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3urizouje.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ojxbejbw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ekzokurd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3witpwvfd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dbujrbxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxbtglyh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3kiqgfaff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrqfpzco.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3steaqrhw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3lukqlbwn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mzogfuoe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvqqkplc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bpzkqakm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqcncsnp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3dcowtnwd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hhhqingl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbwbeqmi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ybpjslzj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3pszbfiti.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrjjrcmo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ssbffoke.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahozzmxu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3cocoagjh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fobsqvev.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3fwtgzqpa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3bsrdllxx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mavfpgph.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3uprvielq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3walptfyz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3keqfuujc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjgikqzv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3txjgbftx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3aaskatbd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dvvrdyzw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xhstifky.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3qxqfrqzp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lktjgvoz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3chtvrqus.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdsgvfnm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hnblbqph.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3svzbjjhe.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3yfpoxoex.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jxrfzoya.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ixernkhp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ktbuuvoo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ceuskjpv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3gzusgeqv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3elechjho.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3idiewfye.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3euydxmjh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yzxufvmo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3npnazvnd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3muwgnwhe.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mtptykvb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3nmzylebb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vcfkyvpk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gdvbjcvw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vyghzlge.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kvpnxrvf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mnwghyma.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3umwtdddg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pknbhkhr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3tawurhwq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hfminepp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vcblgued.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zmhwbyrm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fsxsmjut.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3olabbvqp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bguuddbs.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3iyypbhje.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ppiskoph.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xrcnoaee.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3kkhkbvxy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmvjrvmp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jmzqcvix.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pfvgcrno.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3vzyurzpg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3zdrryvwu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bcspcibj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kciovglv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ptmmkvil.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhxfkulf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jnxwbzwd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3idpmogwl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fmvybkph.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rubsoklp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpuwiaej.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pwpuqlsh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uokacaka.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3winqydhj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3kronwofu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bzyyrtee.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3oyzefwrd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3wywqgosi.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mareucme.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3udlbnrwb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3lsmvhhca.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rvwpmcry.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3rpddulkc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3yjivahel.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pwgzqcvv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hdvtdjbv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3tcjbtqhx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3bfilwkoe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gfslxmgw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3klrudtng.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3assndvkj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3cfubwfat.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3icnbrzjt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mgckhcaz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ooprkvvn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yyjyldcb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ihvyimim.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3syszxyhf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3tqucutnd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3wvrfpbkh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3axzysmbs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bapdyvaq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wneebyjz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3pbtyaiou.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vtvxujee.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3coldsnxy.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3kpvjelwc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qksnnzoz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3nxabyrir.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3jyaaimvr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3gfvueuuh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cilcbeay.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vvykduox.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnegbpiy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxsxzsdk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3jsuczaod.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3aqgfusla.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3unvdiswl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3cmkbjgzx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ypsamcrl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3izvckgqb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbwefqlm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3bpnwhvub.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pomobimm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jzckhjhx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3mvubpeib.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3muqhdifi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jtlfclvv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tpvzuwfm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3cjsdmrvs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3izgigojb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gzecjpgs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzlnspbz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vojrjold.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3kscugurp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qopqpbye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrincxif.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qfebcuyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeyowhdy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wqkqbhmd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3wyhetrub.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ayhcivod.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fcvlbvoh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3fmzxjykl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3elzdrshy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3rabdjspl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vbemeciw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fbhapnhr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mnfjnonl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3cugknenz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jcentizv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qrzkdslt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pomfstrh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3frveydzo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dwxdpdyi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mjetytrs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sgaodskt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3bbgdqsqe.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wicufiso.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3sxklomry.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3vpwqprbq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oopbqwiy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fozruujd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3jndtoglu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jfsnfyme.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pikbfmfl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qlvzxwfz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lbopprxc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rfwpwuwl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3tnbcrfog.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lmmvqdsu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vdpfonfx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ofwzukrz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kkmngkfd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pwqrovhx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3azokxuna.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dnpwwrwp.html


<!-- 参考信息 -->