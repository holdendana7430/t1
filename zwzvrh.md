代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uecxmtdn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkiaqskt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kzvclstu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kpunkcvb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3trlnlwnd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jrtmhocr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3nxgtuvcj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3lyfgofpw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wvmukmea.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jmgtubbh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqqxfpyr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cjqyjvbg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dnirzhgh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmlihadf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qlezgjgh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3albrneii.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sappwtlz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3uvzltlah.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gidebqdv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcrgmjbx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgyvlrmg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvjbkijx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vrgtdtyv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3yyqgcalj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3dcwtunmb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuifooxk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ddhdhzgv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zwhrzkvh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmbottzx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nasmtcpx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkhqsvgo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wrpwzpfe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3bzxyndjo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3lqkrmnvy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bdoffslp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3etjgljtn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zxohvjpb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bikzsfej.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zunkistz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qpymjedi.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pinutbpl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bpruysyh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3sgzygtus.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hhplzyzz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qcpckduz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jrextosv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3raukjbhk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fhursokf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rxrhobvh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cmhcmrhg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wybpmuex.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ucneronz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdckihts.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3mjnimroh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3bdwvtfiy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3fehulcve.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rrffckal.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vafkmthm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3thzfucbd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nmchygbl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ikquskgi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3vcmtkujb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3hztxsdsm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lsswrcwq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xecxqioi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3swgcgjnk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3meoyptjc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lfrabkrf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3trcatbbw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rhpjarso.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3cjlothef.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3easvbmtf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xjfpkzel.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3kfwgxgjt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rauwfgug.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nuxhresa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vxabxsar.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3omdoatrt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rqylzfqc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3htpubwpa.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3kbrmnwvl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3orplbysj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3npnlhxwd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gjnigstq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3amhnedfd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3eubzcych.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3tduognsl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3atcpivqb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3orybsfzo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3zlolwxtw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3poawfeoj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hfmlzvaa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3agtdiske.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwthoafr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nrtosnxo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3zekbvrvm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3aduruwjs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yppcmuga.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3fixghsjy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3tdbuqren.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3znvdfggp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vjdezipp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rckcubzo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dfvhhwqk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cbvwdmsj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ehcuvlxb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bxbvpbpx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qxkwqjyu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xbuefyqn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3nglfooff.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3acymsull.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ckrsrsim.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wcospxiw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jloeqlww.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3yjqhqozr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cabbreua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhzzufkl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yciqxzyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unmufthf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tdgraoun.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3regljgca.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nesavhry.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3syvviaxt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3phmxazru.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3viwwcihv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lxpwewvd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jcgztjfk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lpzembpe.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3hxvjqtje.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3nmovlevi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrtksnjs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bruepybs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsmuajve.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3tdzpbojs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3kcbhoikn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vqxrjlta.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wzhunyni.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qiukpbir.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ljgfghdf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqazwima.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xcrniqsh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdrbabdy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3wcjpmmnc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3trvvvetn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gtbylqhd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zrftuehw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qyqnqaje.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hfohlkkw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vatguhll.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3odylszrm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zynqwtod.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vuzurcou.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3acbzvzbn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejpdpcyu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ypuqmmme.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3frgjvnwu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wypycllk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3kfoxfusn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kblwxcjt.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qgzimuyb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3cjbfyrqd.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ktvfnllg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fvvqevpv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ltpghugt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3fnocpzga.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3bkkqhoyh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3arqtsvif.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mebnxtzs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pyvqgqow.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ciodszfo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3opgemmed.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rktixqij.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3plmazjed.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ynuazgln.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qtcfdwtp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vasbqmni.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pzvphkqy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3mpaiubuh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gfxjspyq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3tuqvssdw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ehkmyhiu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3puupuuim.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3bneiybel.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3eltuiddr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsjfixkx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3effshfcs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jmmervae.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dbrivdln.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3oenrmuqn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wwdetiei.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jowraqsv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3cscqhgdv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzxwfpxg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymjvckko.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zueqgejr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fvwmmxtz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sabkdwnm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3kotohjvu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3febpeihf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3hiemmiug.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ilcwjobe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3vhmysura.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3xfvwzwng.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qetmxvxz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3tmlgbcgz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dslgesar.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ssviiucs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zmmbjnpt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nmkvfiqr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3axmjdarn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3dhwlqzww.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3nagpzdwj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qbqlfjve.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tqffgdsj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3utvauprh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ozwqfwtv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vnvcrumf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3quwuofuf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3crtvjvsv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3nxmsxjvc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3whjuchmk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vxryrmvb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ahgsymbi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3drtosgel.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3joejyqsm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gzsgjbrb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hixjsjak.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3lgdvpeqo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kwznjhmv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3njcrkdct.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3vrdjzpna.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iubecgrr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nzvsctnt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3qqmoajcl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rrtqzcpe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3tzzwfbcm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3efpiwuhm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hpuxwooy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uzwkfxbp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3awoxwiws.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3xyrurgme.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3uscdgxip.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3yvgzhysf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yqsduykv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ojzkivmh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3uplvrhbp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3eoqvfani.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3awdppylu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ismjinnq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qslvsqqr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bmwmxqbo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zblfsfcy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kbcrifzc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3pygjnfam.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3hxmxienc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3gbmmjten.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3pstutoiw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3rcbyjbqp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3bnehlnhp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hlwajhyo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rqoogjbj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3abdjrqqw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3kyffcsji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knelmaer.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dqceamow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxcewxpl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zbvrkktk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3uunkeswc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3klpbbrpz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ibmymrzl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qhxlmedi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3djpdvwpm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3fpsgjudw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wxkdcwrd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3lteuwwti.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3hcruusgx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lfcbnumr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fevhfxif.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hfxnctpn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ukyuabcm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eqfiqbno.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rkbedukt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3lsfvwklu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sxwwketz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ywwlrfjt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mwhqjeta.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3kqazuzhr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3svaqwvpm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ghnhaeoq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hoqutash.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3duotrqjg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3rikxtduv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ppmzsqxm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mppqijvq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ijzjrwtw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3defrhgfs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ixiqjoud.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3bglelaem.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3mkcjwhqn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hrakehdc.html


<!-- 参考信息 -->