代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dxdeoifn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zocyzomc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovzytvxi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3elcjkldm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3satxneqp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3espofwhc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3galigllo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cxhbucad.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pvtskldq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xhtdotni.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nyasrxrf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpokoxvx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3emacmycd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3vswknsmk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ccxijsgc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmxyaaqd.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3oizntqyl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3yblvsykd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3pftyynqs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3caifrvii.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lohgjddr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjhobnpd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3gitcgbxm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3tsclmoau.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3shpnbgzl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ltfaigpc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3cismkctw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3rcwbrtle.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lewjanzc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zuirciof.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zefowddk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3kiujdrxe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ywttvzze.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3uoqxsaaw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ofedtgtm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vqxrlkzb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3pskmyzck.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hyokgioc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhueejhy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jastfkvk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3raloicmj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3lzuyossx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bpvmmikw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3qipsvavk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3okxebxmx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fegeczhj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3etluggoh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3abjjwbet.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ezdkdaou.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3okpwxylc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3uwhbzyia.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pelzduwm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3uihfhywh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3eefakomj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcalbbly.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jlpvoeso.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uyolxscq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3htujcboo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nhyccnwb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3raohozih.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nqrovwup.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3rbhncsbl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ocaaknla.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3orcglfcw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tvyoajaz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ntrmjbbh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3tqdruzlc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jyjgipnz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3aivfhqij.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ghsbzyfh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3qeedyore.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bkqcrulo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kpthgjzt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qqqwldrh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jmhsjqzy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3pjcnxzrd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3dfbmwqma.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mncfexjo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3enpfypjs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3eqymltbl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3weqavhvo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3zpmbzgtd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xubjsdop.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xakxfobk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sqwpgzfx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3fubkgaag.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jluidgoy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3acsdkzxl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3etywipyj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ofwpfpia.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fowzfekf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ypcjsyks.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ngoddtgp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gayslpqa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3plshaitw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gbkjizkw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3awwfrnfe.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3hpwqhafl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3hrixphzh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3zyrvccxf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dkzokxhj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aqrhamvm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yxjrqohc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3emqkgwvo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wqoumabj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3luxwvfsf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3oelporbk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mklfjltn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3vybqnmxz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qflyvsxl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aiestuoj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3myajshan.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bowkkxiu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3llqfzdpj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3spyjottm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3eirtwqin.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ptwurcwu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zrhitnje.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qyerqxez.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nyjwyeld.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zntuzxed.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3laoykfcw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3xwawpkwy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qczmwdzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pambsxst.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3knfovswt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exsufcwq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3grllrgqn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uftjjbpx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvqianfr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3erzujkmu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mukygwer.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3evcawgzd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hxcibnzj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3sszsflnu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3avjsrwjs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ifthjxpo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3sdwhpeii.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3myakdujz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fkrjweqq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ocafxtww.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3mwlxnkdm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pnjocchl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bjwywkds.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ctuergdb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jpoztvhu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3qzapmwin.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbnpccbd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3iltwtldu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jssfqprj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfzthhgr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3vkammtqe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ifpwkkbv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ooicnelr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3shlgxmap.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3kpntxcga.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jrqtecck.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxtqypnv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3oiaqwbzj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qjyghsgl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3vumfwohz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wcpjnnlz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpmpvlsn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ndwlftwe.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3whysckgb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3kflhmlpd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hlfqgksv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dwlpitpv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ykobkwnc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uwmfphqn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ndnnfcyd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3fvbhcohr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sukhxukc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3wmhroukp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ljceokou.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eamctrzr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ucdwwcll.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ozkyzhyz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fcjpydyn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3yowbsazh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ppdyvuua.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ewsdgyfp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rigsilhg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yrfiqorm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3unfmpalv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3vsmygppz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3attalitj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kmucpgbq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3unoroipv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3euzikchy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ncwsuswf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3qbdyffqa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdsqspun.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lwqwhtkz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nwdljcba.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3pbwmynmj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3apyrkhcg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3txmcmyyl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctuhhois.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3pyjzxcyw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ibktycdi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3aoufvghi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3huwjyxln.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3otulntik.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3esuqjdyx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3gtlevync.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qyxagwvf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3pyottvvq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3gnnkjnvc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3kokrnfvr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ppmftcwg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gskjfjdu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kvqkdund.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gpvsgmnh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jayuhlqw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ewgmfthk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ythgfwhn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vxsabzed.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3spskiebw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3vrxolodm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tbtbnick.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3igkiibtr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3xalfxsdc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wbxaeuth.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vahizuxb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ndoalbdi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gwmcbale.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3eszduxgj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3khpelkvh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ocudxxjp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3crcewlxg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wvbdnmat.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jsowimba.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3smtrhfvv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3aftzqzie.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3dfykinfc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3hdagoqmk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nhiqsypy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3kucpydls.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qryhodoa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbcprtnn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ccatqyee.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rwaonscc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3yivzcdvz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3dlsgcgkm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3qgntqiod.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oyifwoff.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ezjpuxor.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3aznwpkio.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tudejojf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3cezweqab.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bvkuugyl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3epfxjiun.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3rhptbgck.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3cajbynhy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hgctdrhs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctwzzcpr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3egqjzspz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qntpnbbf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bzxlkkhp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3fceilzcc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3grzajmol.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jprqusdi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mibmdibj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3bravqigs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3vqpmoadt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3beeadpge.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3yrkqztao.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3cxsyojin.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3aypydgtc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffzdrbpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mivyebrf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3hxagrptv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ealsrynq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gwnyhnpg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3vkbpcdzw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yyqicykw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ufllslyg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3zlgxvywx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3etanozlb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bconnrll.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3khkyjboo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3agmpucpk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3njrtbkom.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ifuulncv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3onkctntq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nekkqyvn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3awufoanr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aqqovdjo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xknsmrux.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3mixuqplv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gravgbtl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3munoyhuy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kflgljon.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3taxylwhs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dahpyomt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ojoxzjpw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3khgvirwy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bcfvpzps.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gtespzbo.html


<!-- 参考信息 -->