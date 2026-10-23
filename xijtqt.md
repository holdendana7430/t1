代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yfzpizlt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bkribnsu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qfkixxts.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3oazcvnxd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3syaihfvf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3pkvgyqcr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3hfyfekob.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3gzdjqvmp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yikojmdv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nylymkbn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3atgdxiln.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3jwnujpoq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3bprjcchq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3unrypoqn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3uwkaxloq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3nnjjnoil.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xlxbsrwc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3szasvztv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dafthjoe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulwkhlco.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rzmafnca.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fgsrzfrw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qyqnqind.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yczbfdqd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fdgweexh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3yxkaqmtl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bkqekptb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugsgsuro.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zhpohvkm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dfyanntd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cuzmgecw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngzupttu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tgwfubgy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jzcdxyil.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3pyeynkrf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kntcbvwg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lnmwvmin.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3uzueohps.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3muvghfex.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3zesaybwz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3geszgmix.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3serwzzsz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3caczrcrq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jftffskz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ehbekmcc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ufxicbnj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3nljqjend.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3xeqlgkvc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gfmuidoi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ydbwunug.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gucyuzxu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jlhizizf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3iecqbtry.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cqwszoss.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3afhkqlbg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xhmhtxrc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ysgnvdxg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3uvcljrsg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytgnzudi.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dhhltemg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3aulewuta.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mhuryluz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gdlblhbp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ihfarsei.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fgzlgcwk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vkhbxkea.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mdwsvmmm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kahqajpo.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rgitbvll.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3lkgnojwk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbblywsy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3myylwegx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hhydekwx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hnivmltq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vqtmpoxy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3lqmbdjmi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3clufiipc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3yarerjyx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3blgddnkt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rysliuri.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rcycbrvr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3flyfnyrc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfnhkzgy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xrdfrdyt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3uuclkheg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxmyheui.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3xastsijd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ovvrgpzu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yjhaupup.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xnbmlkxt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zpkzhofo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ioswnpna.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3hxgonyzz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3afiozciy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3iikjlwic.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xgadzzll.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3jzbakbzk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3wcxqihxq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dsifrkma.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iwwpcqap.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nsplhxoy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggknvbvh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3icyxhwqu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nqbhybzj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ypllraht.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vydmfvve.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ubizzmsr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3utkvlbvy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wvpyaxig.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3sjitohaa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3rcbwhjko.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rjbdqmqc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3mujjmewn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3kcmaztlx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3dbhdugwe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wfkgyrru.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rziabwcz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3evjwxnbx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzvyexxd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kjkmkpkz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zmhfpbhj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3domqjxqc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3norcgjfe.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3hsqistbm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lfbjzhbl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3twtqtqiq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fopfafbu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ocontxsj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zsszbkhk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bljqdkji.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wtitanlr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hhqasmak.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3iqjewozb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcsicntg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uxrxxufg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3luyoxati.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jvdawspz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3cyzkxeqk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mdnpkccy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3blvtbxug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfnvkfvl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3irnmczdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epnnmtnr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rrgnfzli.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xbhmfabi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xpsjsgay.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzmohtdq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxrfwomx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fvsrgtaj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zlgtnvud.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xlgdzplp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3afcmvfos.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zzghiueh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uyckulwy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wzsvuyyj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xiilegbx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qvfljkst.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ltxbatpe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3epdczkpb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3eeswlmxn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3rpawlbqm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3iuhhrvas.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3moegbohb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ednoydhx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3oibitzwz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyjdkvtv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmjofdfb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bumlncra.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3apqiystg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ngifvcih.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3sjdkmblo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3svnpmxhx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wjzeffzm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mbzzqlkc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3vuhgxupf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dfnalrxs.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ohdqevvh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gphjynds.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ddymmbfz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xvzhnhxi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fgflnskp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3puzxxerp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zehuuqvr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pmrvftde.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qzdthxrd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dtrdgzmn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ljypxsqr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3oweanbqo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3gixogedg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ycaujuck.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ybhqjnyo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ovxqycfs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3forivchr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wkdgugnl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wzwwvryk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3zvvwfseb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bjdghtyv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3uzvuykvr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3gziqajaw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xlauxcts.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hivzvgfc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3goszqakz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tcspzjkq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3smqjfryk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zukfhzep.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3tcblltjq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3bmyropdv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ewnabmtc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3uthvismn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3psyovjjo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkxxmeko.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3zfjfbjou.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3uceugzca.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3eebsdvxv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjakuoiu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3bfhwbxcl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcthjykm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xrxcjrag.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lbphbxnl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bwciooxs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3msahyape.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3qglxcwmr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jzgezjqj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3fwxynvvi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yhriqswq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3lulhdrka.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3rzetqjez.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3uuehtqan.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fnimovip.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gumijzyg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3klvnkcek.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ctyofryr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cwggtmdc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dufexnby.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3woxaqsne.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3tdxnhigw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zzndarly.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3lnfzilla.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jebdccge.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3qhtxpqqo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3psyngqzr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gtedvvgv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3jwrqwylb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mefajnpr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dhxarvne.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yotemwtm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3reuuyfvy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wotblssw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3abjtypia.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3mkblkmrd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3chfpjhxe.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3mdnjucid.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ewoarljy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhoymknh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3fmkhbwqc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mivfecrp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nsejrdgl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3nvtfbril.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3escuyszd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vkbjiwxy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3rcssbxrl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3qcsaoqug.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3snpqbhiq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dvkebszi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3embzwxdz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjruhffy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zwvdnegk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jpljkpka.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3yppfrorm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3hrmuxesj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rgvbqstf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ahpekndk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vwjmzjsd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nusvvinc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3swxubvtm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sgeorvud.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3neytwwld.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tptxmpjf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3aamkrorn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3cfhfpwws.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ieddmtlv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3bigasccg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3dganvrkt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3nyftuyup.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3scgumnuf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3syxahpwr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpdxhfbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bymomovj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nqyvmvda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wuynxqzf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3axcrqket.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mcsnzrzl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kmjjrorq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zrbdlprz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qaojijpq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3adjgnmpp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3izeujjxn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ymedopnr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3grbouexa.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lhzosguw.html


<!-- 参考信息 -->