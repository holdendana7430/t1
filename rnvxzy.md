代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pmdpmwiu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cqwpuyeq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cpuavcba.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3shozyakj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ejqrrykd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ydjogsku.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ejvsvghd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3bhozfves.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbrknqir.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mxahoijq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ljdwdfui.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3oymcyeqt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qklspmej.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3xuvtvfka.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fgjgfnwv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tfvbsspc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3doifvoxe.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3fiioglag.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ebchxjmv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3slwktyob.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xlhmewzz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3hmrabqnm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3wopttxde.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3yyoiuwiw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mehiuboq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jemeooyu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3cthyrjti.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3huyaxqvb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3furajppp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3siwvbpsj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3igjkgawy.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3klgzpniz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdrwnklr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3zrfhzlcc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3qwtmbhwf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ccxvyvly.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztdpfhid.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iamsrkve.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3zghpaczo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3njtsczgv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3epngtkze.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rbwkxyah.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3mwndgsfh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3kutfropj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ndpfxzmd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vtncdqnx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gutlustg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqvqypkr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3cgkfmwmh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3lcusaekx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gqnfelga.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lweszhsl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3acgjuerh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jshpmbjl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ktpwnofk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zmhbrozq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jvagxvwu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cylyoegu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mdwhovmv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wazcljri.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ptchmhxc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3adavkgwx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrsustxk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjleewmg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eljnoyns.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dzrdcfhy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ubfdsryi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3uigemkwc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzldjzye.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3dkufujqt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qngqbrwr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lolrasqc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3evvhbahh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qsvfjrqy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3slworfbf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3pckzjqjx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3huyslbhl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fykkvsni.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3wfceajwe.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ezmfhuwa.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rltdkobz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bmjaffqq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3reucukwo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3baycspbc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3szkkeyjd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pvjgmnva.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wfkplcxd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3njtubtpx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ntdhsyoo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3mvhryxts.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3achlfoud.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nqykwrry.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mzslwllp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ujcdjitm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3eyaabypx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3qtilbznd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xkuvquoe.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3sltljutj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ntpkgybb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcqofzbg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yetpzwua.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3pvtapuca.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lyxaptyw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3bujvoivh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3qbluutbz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3gyphllgn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hojunbbt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ztgcqvte.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vogjmflw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ejiijwmn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdrsatcr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3skmugrmr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3klqmmmat.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ttjfcjcv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jftqcpcz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3zcmvkkat.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3emimvogs.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rejnzvzj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3okhxjifk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tsmwkuwh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ngjmomsq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cdbqsxfo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zrptstsw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hjeagvak.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vdnfabfv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ahxigmxt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xfawzyqa.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3biilmxdn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3euekvkov.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3uoeebnry.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3twiurzfh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3okzvkkyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uiruvpcc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yqefxpkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxbkldeq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gubpcnts.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3gqaghbbx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkpjwphd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qhxjbugb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3weudbeqt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wgwtialf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3frskpsis.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3mamqkqnx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3brgzszrp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yonfhkvo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3wgddevyw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvgiwrua.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhdsckff.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mexblguz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3htciafai.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3zqjrgdup.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3rpgryrua.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qchzsvdy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ekrrevft.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gugdipxf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3axhzupbv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3athtzlct.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lodyewds.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jixhfema.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ralythix.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3wiimsbom.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hlzhohlx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3gqumxfzo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3cofrevnx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3tsnzliot.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vbutjhkk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wvouuelo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3srxkyvzq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmjmwrec.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yunutdog.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qrriisso.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3jbnopeyw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pmhququx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3qopzzldl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xxmwtqnd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pfuqdggf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rorzeymb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nurihgcd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3exnygavz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3dkhbogqk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3tcbttsyt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3kwlwgyfs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3pcrvgsxx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qijrltrh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3weilanuk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wypexkut.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dkcwhlem.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3zaesbmnq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tcfqnpsw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3lvnzrfcn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3luchcvys.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ruqycage.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qfcodsud.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3eekedgny.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ucemafol.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3zunzcfav.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ihzjtqzo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3gooyagmn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3eexbmtmy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hzmkvgzw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3wexruysm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dhobmsol.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sfkzgcut.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3udwtrsgq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3amoeqlal.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3djubmvuw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3abljyceo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3oilclzxv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3plaatkbh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wscklwdt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zfsfyfgc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hzarryjr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvnfhrdy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xmitpvwv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3arfotxba.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3nkxtgvcu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rqlefczk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3caatfbab.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3agzsnlvt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3eueqvhyh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ckvulhnm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hjroanrt.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vqprhqfb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zcahfwrq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ezfxgdpr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ucfelhsb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ffyazngx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3qkbqdthm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jivrrdvt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jzcfwlmm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3bbnrbcny.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3erntsisc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ivsessmb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3jtfezhkd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3wojknkpv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ipszwzuz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3uxonlpcd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ajuuyyae.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yradlpgt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3spgbtxxi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3gcgxormf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3txguspdu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3yweiqqly.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3dybncafc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gvbqpfao.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xmjbzlgw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3yotnzjob.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujpvdozn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3praxnsuj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3jroyhxwi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3twcoviel.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qxbyurql.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fmuubfna.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3tczqemqe.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qfgwnhrx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tldojdzd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3iaffrogq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lgjfjcjr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3bcsrlijp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qoeyplkv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vwdllkjm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3pusvdmzp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wnyzhoaj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cjaiigdo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fydoffrf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyszbpfr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nwxdlxid.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ftlyxngz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3umufhipy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kyzfwegl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fbleqvrd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3icnbccuv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ocfqguzf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nhciqufx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3htlbwmtz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3qaqchclj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3luieskfy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3epwayhzc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrotwnnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfyfzfqm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3drvzmpfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zoriinju.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3soacnhdx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3izgofiqx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3selyovxp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nakdfabj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3szzewgva.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3tyadszks.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3cpctzwnl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3sjznprcg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3zlinikrm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3oijceyqq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jjfcgdhx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3igzazdsa.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3etfcgstq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dbfdkxyr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bunbhezw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3mgzdkddh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3wxxqfzxv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wvnihise.html


<!-- 参考信息 -->