代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3drewqugi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hvmgesuc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3zxxtljds.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jvgkubgk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzberkng.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3doevtxkd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3votzbirx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ubqokgcu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wtizkeog.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3mnmeetyr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bzwqsghc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dnidsklz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3sipaudri.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvzomjec.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3adqlhvsf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbsifyfi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3tznfbzhy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3iddamzwd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hdebzqms.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3xgnzgplx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mheallcd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3zdogrjuj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3jbvnpgma.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdaxykap.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vtpdxuuq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ejwwxqii.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bzpjnewd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3gylqxuoq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3dtlgjask.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bswqjukd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3dhkbjvls.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kwtlfwqc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zigjmsfj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zyvigtox.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3szjdzvrl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3dlfwlvrl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3bulpfsva.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntuhidto.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ptxyszvy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wgrgsknr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgcgmjtk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmcuzbkw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsvipffj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3leqthpgs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3nqqgpfmw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jzsaydtj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzhnuiik.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ujdvftns.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3thprhrlb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3myfsjnzy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ukjynbzf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cagvddys.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dgtxjwyf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ifhyyhop.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3aufcfkek.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ctblbcws.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3afwwhkkr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3eqhycqsp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbvupiqh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyavsrex.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ftvspypz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lyedxcwv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wmfqguwc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3tbfmovtb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyjtdtli.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3llbvehmw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3opectzlq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3novyolfo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vpkloetb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3colasulw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xomsxqis.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tjoglzpv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3lamytytq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbsfcnbk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3echwokkg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3msgxaiua.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3cujmunml.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hpbuxigd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eygqtgdl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vytbyzsn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3dcmngeoj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3yyvvmhlk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3isgryaob.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lcodpifh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3rwvpkfeh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3kmtdygbz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mgrwmegd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3llzwosnu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nvfxjcir.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ubdzssco.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vqzvnqit.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3qztjpstz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3epjwiavh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yozkgwov.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3gikedeph.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3efpmnylz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rptcdsag.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3geohftmi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dbsnmkxy.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jgywouwy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3myruunyn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3odgngnof.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ugrawylj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mnblzbah.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bzirkilf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jnxrhsjs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3spytfxnt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3zggglxhi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dumnpykw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yndymqdw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ocprdmnp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3leobjsxz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ppzngqty.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3brcoalis.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gvbqcnpe.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3brkszvtu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xovwluwi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hdtmvhqu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3scfvpexl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zrkvhufi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3sqvbifxe.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3evkcdtje.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ghjmvhcc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pyezqxdy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zdamdbui.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3udpdhqoc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3fwfsqdor.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gcidggkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldrmrjdh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cckzlzry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhglnans.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3swbxpiza.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ybrwppek.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dfoqvgyz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fdtbnmuj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wptvtifo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nxdivbpr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fgytpweo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3duyisyeu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrlgxprz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3dwpaitqa.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kvlfaevc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qipxsyiz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkesgvhv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vmgntccy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3vzrcdiau.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vayrfdkv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3spsdtpjj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kixjrmkz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3nxfykfwb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fqreachr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3dlbpxnff.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkafejjx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hsxtraxn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ilaqelts.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zsfgcrug.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cdzutklc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3jdngcozq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3elmfeydr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3yfduavur.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zvgqnoxc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmfwwizr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jwnsgjmv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zcygldgx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3njofbjxt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ihokieai.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3naylkotu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3llziegxe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jlkcpmno.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wsmvelsq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wyvjteng.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fhoxleyr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bkrzzvvc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xqcxvnqw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3opzjjsco.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3zpweegor.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kbhuzeki.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3atkrzdaf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3sajgenwa.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vexpnrcj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xxhwuklq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3voozbuwy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hasmnagv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wyezsbwe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wrcszyfa.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3gdxfiebl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qmfzbjnq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3liskcfih.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3obrrizoo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3tfhytnqi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3cxjwjmng.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3onlkhflh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ycwfmmoo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3slaizovm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3bzoljfpa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xkfusuci.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gueuwknf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3deoawtey.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dfiyvqby.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3wugiphow.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3mcfdtmuc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ftjbqvgp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3quqgqtxf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3pdqusopk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vnjvsjwm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3obmxlhct.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hliffqzv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ngpmmrjz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewrjrlxx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3rrruzusj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvhxwjzf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zfksrfes.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3gkqlkwgg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wufrmgaw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ecjijurz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fnkcoqug.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3cxflmkkr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yuqczisr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cexmehsx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zdlqpbsq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3glrtwdos.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3miervrww.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3fjogmasd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xbhjqibm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ytclazum.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3epxhsmkx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rnbgajja.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3qucgtlxy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ggeqcjdl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3tsavyjkc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3edeqommz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3inimlldv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3outlcxrc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fduwrmpy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jofrpszp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3htadbjcg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3bvthuqkp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3fmtfkkwa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3tzjnbgil.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mjmqnlcv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3kzuzrbml.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzepxfqz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3lrvvgpam.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tbkurvte.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeorxjck.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3oaznwnjd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3cdfhwfun.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hodkcjyi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3pjmftahm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ruekzzck.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jbumztzw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qcuiyymu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3guyotnbk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3vczuhhpx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ryswlojh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lzpvaaqy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3dorolqkp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3rpparhcx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rrkjbzaq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3lznjzkmc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpwjrwje.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3llldhkte.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3duiuuabj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lsepbmuc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3dlxntnrq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3btircpyv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3crtjmymh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3udybecxt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qmrwgxic.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3savihjnm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3avvneady.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3bozasdwr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3jsldjsaj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3bsxparsy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tejwliiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vuycfisl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3gwlnamot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slshfghw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tshqazyo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3tmeaxwgq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mciusjjf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wtgwmzfs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3fkgdchuu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mkvenzcc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3xzzlhaxf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3yllosiwq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xzlwgkfs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bpvlyulp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3zgrwxwns.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3pejlfumc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jklypihj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dytqvpqt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vptvgkvu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nrmiejqz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3rccsdhyp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yhhrstjb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3sjzmyjth.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3olqxtyib.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3mdsubvzn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3iphkeofv.html


<!-- 参考信息 -->