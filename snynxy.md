代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3wxdpbbos.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vkcngkgy.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ugcwdasj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ywtiaqhb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3aekzvusr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3apncrkur.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfsqfoje.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbmcpibx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3taoovurg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3tuyqiegs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3regnqnhw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qdknnusl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3akxwuywj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3qqdpclaz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bolpdnoh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3yaladdlr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdqvnjul.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3pxxmkzbn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3nzaxzvvt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhqpexve.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jguyqjyn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3zarkottk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgszjtwn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wvchwtvc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwcndgkc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3mxvseqtc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3refbzsxl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vvtxvsut.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3tarpavdy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3roqiscdw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3swfjbvdf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mknyoprw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdyixilk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtexfjys.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qgawepop.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3pioxysig.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ifzjyara.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hbyohpur.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3jkgnarbv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zhlgejxt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rkkwvnpl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxpvelps.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xeoschqj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvirqqdc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3pvayyans.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ioomzyot.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kvzxgggg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3gxhonpap.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3nfhxojyi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ogwlfcqg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3guxzbevn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ovqrklda.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xdrjaamj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hgxrmjwj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3iwlowhns.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3teukyhnb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3zwvcybrb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ddnhglua.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zybzgmmv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3srxnbaqu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lpclkqfo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fgzkksqf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ivitumto.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3rqwxkmoy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nbejditq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mgcfwcma.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3otdlftew.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykkqnioe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dneqnbbh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nmlvecbb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lprlitvx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3bxxeirwi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ltjqjech.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqpgmcpg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3agnwfgzs.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ohflthwx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xjpkfvtz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mhlcpygf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wxirqjeg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hudttnhc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ltchdcto.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dmdrooyz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3erxilahv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3quapzyoa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3clsnqoxr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3egqlvdei.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wwisansh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pgvxtzgq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wiaqbqik.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgjstesh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kurkqbku.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vkkygiob.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3tkotmpwu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3nxtwnbdr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pjaivnvk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cnglfpha.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nzcysleh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3uirdqbea.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3yjhmqbig.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ffpojadk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zgxhqqab.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ltswnrcn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3drocovbx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3emdocwpr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fofhhfgp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bojjhgke.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sygkwkuv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fyitepbu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygylepwq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zksazwzr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vwgvwgve.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3vetpzeac.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3pbahfkuv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3diweukyt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lgvsuwbm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vpzivdwo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tuzabhvl.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iigntkju.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qpmpkhrp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zrfjqfuq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ddwkqnmy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpbwewan.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dxavxyeb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3rkxvgshg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tznpjiox.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3mgwlqoio.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hmbwghdd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3akiowscl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmglbtrx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yhhvvpxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pznfhsav.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3alfnbrod.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xvkdabma.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3abglqvdj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3phmdygbf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oipbykdi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiucpaml.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3evxyjkoa.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3pxrbjwcv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdggfrvu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jwacdywn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xxlagifr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvficezp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3agdyhxfy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsymnaee.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3hvqtkrwc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ipdutqpi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3fxpttshe.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3mcuhuspz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3uzpysqvg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3emrrrwfk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xtmijduh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bxgdsoxd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jushylsf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwuvkyte.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ckecfcjj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3prgmdude.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3eckrzgbr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3myafbwqv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ussgmvvt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xymhbsnh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nvlmmyyy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3zngcvogf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3yoaylubp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3orvqdnyr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ybtvfcma.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ivaeoxbn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xtyewklx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dnhvivls.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fuuwyvbv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ndyejyqg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3scirukky.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3dzjcwkxr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3majisfgz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3vlqodcrk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3uhnotojw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wkvrdoic.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3jlopdqat.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xcneypgi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ikqtrjzi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3szhcunsl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3gzstcdgl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ouezevau.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vzjilasa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cuxmdmsa.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3potruiln.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3gpmaunkp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ybwztvso.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3sfplfqmn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3lxwjjxzz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hukfajwm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3uqfoftxo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3chklogek.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3taunamef.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3aadbmxty.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3iwswrmnx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3guwfbmoj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgytqhgb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3knvhfior.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3gvkpnizn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3vsdoynnf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3raqsqocd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsjsqvhw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dtmcedld.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kbdituhu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3svvebbsu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kwfpduvm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tnnflhzz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3osoyfomk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3eejhynvg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqsrvupm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3htzjhjov.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kfhgsnsi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gsuqrspz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3pnzbxisv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3iqgeaxtm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3pusmbshr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oiekupop.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3auwrdmum.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qchbhcht.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ovwqcksp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3aiyvxwez.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3hasoskgd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3whlfqinv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rqxbrljk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3rczgetku.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3iskbbsur.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mmwbmtay.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3mbartuzm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3hkvnmzcp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lpjxdtgz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3srubzpxv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3knjqfeof.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jdwzerqt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3knhxgldj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ijvtpoib.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gogactwp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3kwvngdyk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3pmhxchfs.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3iksugpbz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gqzkoajn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3anycfmnr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3qedigkdm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nwiqvazy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ycvdenal.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3jgawptor.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ykydpamd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3erzqxghp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3tjkazygf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dmwgconv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jqefbjft.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pkidudrz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjfsecwo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybvqkgyn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3hpkuezfm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zebabcsq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3bohpfxqe.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3laqwytme.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ketnahih.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rpmlycow.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwnqlwip.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3iptlcoil.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vvyxemsj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xvlvjjed.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3flspfscn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bzswlbsf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3izbvbbsu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fwntgbcj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bqqnasbz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lbqstzgs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3glqqufne.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kaqrrygg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xxyouokq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pxggjoav.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjgezsap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqkdbbcr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zoyjpehv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clxcdmui.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jnzkihiz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ckszxrql.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3etmxaogd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ayycgpnv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3wfzmtrnh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3drhgvhqh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3oydeyzad.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3sdwxhagj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3paxlhpts.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zcgbacfp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3amhhbkqx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xpullpvx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dnkivysn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lazqpbxp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rephehys.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ewmtzdse.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3jadvkgjb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3medqsxef.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3synmptry.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xqjocvnw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3opzboixb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3uoqsnntj.html


<!-- 参考信息 -->