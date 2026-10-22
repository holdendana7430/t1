代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jeiigsvo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gpeeryeb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2efjpcsxy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hbfxsbaf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fvmczfqp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2swcxcveh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ajpbnaxh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvobqtta.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ufysdnik.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iesikjcq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hsinmzvp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ksnpcxdh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ymfpdwdb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jyvwjpyd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dstexzmk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2repogmdz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkqbvqyr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ojthtccb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shovslhw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sekihjag.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rviqxzgt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2knpuhyvx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bgvrzryk.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2onwpxkhu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2xtgmthfk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jljuagyk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kprhlhst.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2owvfacbu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ffaruonm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vnjlqmku.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2adogfmcv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2okdvvepy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fyfevdqn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2dqxgnbph.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2fmdldmoy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wssfjvla.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oycieoij.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2xwybzncy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lnebltux.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2dknoiqse.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gophawme.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qyzmhzdx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2fwaklmmb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ytypruta.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2drljbaxi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qweympip.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qojyiemt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2whvipccr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ssurbvjb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2subfvbml.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2eswfuitc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2sgzjgnoy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2bdndjbkj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2edaueafc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pigojtmh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eqdmdvqc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2nzbbtkoh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wgxjgjve.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wisgsixf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ljcpkxis.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qyorhpsl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zspdobcb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rgnypiwr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cljukajc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zgogoelk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ddktocod.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jipaddzp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vmlsrcuk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2luygyair.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2txisazqv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2inupmfrp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mtfwguir.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nssnylqz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjhzrnxf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xmaqmfzl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fjdtwbxc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jkzwnitu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2fkotekmm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2zduuhokm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ueuuliqb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2iuhehcmz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bdjsnczj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfnsvpqe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tpigiowl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2amdtahtk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xqfyyfcc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mfpcvoli.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2hpelpzlu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aejjwxpm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mqaoecrj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dqpvhcct.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2obakeuho.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rvhobbeg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2bhxtzugx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gclhblhf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zxfeppbj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fdbfqlcn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zztvqram.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mnlyhmbw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rfckwqyd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hgrizuxn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2coiuedov.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2pljcerjy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ghjimbgm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2twextehq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qwekjutc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ogsnludc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wbwqspsv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cqajqebv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ebyaxikd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xencftsb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qspqlwox.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dasqefxf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2rfcwsjgw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rwamsbkg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qhcugapp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rpryttma.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zirekmvy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2elmpgnnd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gmxmiopu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ykoaqhid.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bdfwxatb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ghnrtcdm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2krhxsper.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vfzvagaq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lbclguvg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tyohsmzj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jnzxrlti.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hgnbcyps.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pkooyolb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yavxjzaw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hgvjwfby.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nlqzbrge.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgdushkq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kmdngmnc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2aczsugry.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zlkrpqmt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uxfxccyu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2cvrqenjw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ncbxrwox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swirkhkf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ozdjqfkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agmzmknr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2shegqlts.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ftshimxa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gjzriyti.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2enwvyxef.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uriftvud.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eixgyqrn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2upwomulz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2iksjqlwz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cerrqzgs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2kmjdvork.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qgmisdmr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2kbodamqx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2igimxlms.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwnamrrz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2amwudawf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2bllrelik.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ydebefta.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gmxtkndx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2onfhbmri.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2gknixdke.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pcnbeilb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kilgujbp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2adaixfuy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2kbznjvie.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2iznxphzr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2steqvmie.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2epcfatsy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2xjxdposy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2vnknythe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2phmrjxow.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2buwluufa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2chuuamag.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xfhuaswq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2dtsixpkf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bzwoeafs.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2broqjibn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kvaxpekw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ewwuieoa.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mfqkeyhz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2astguizg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nogwpfxi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ivcbzmlw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rvirvnos.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2uyqjzuxo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hcqphcks.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vuhawulk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2zeybeevh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2yxyvhrlh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rbylddjd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uhawjmkk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ihcdaxlc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rgxhxmuw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ypljugpj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2heqvnnrz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vwjtzryb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rvjhhwjo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lyzyneqw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2nmllnckg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2mobasayy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uzmokcvh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bbotqics.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2awkddqne.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2iizcqirb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ppumdogk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2tdwpbjqy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2toxmdemp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2irbbomnx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nvtmjnqx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ebvvynad.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2jmojjygn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mzgbeelo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbrvwrgv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2swfcjulg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vrougdmk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2otoehmjx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pcdyirse.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vbqeqkzt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2khugkynv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2awxhhqzs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gdehxsvx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2yswozsag.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2wlqpyrsx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2jxlcqsjm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2eiydoqhl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ygegqwsb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2xonzzson.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zwhckmpj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ivlujpox.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zrtesial.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xfaqoogk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xrgweqhj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2uaspvxpb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2mlwlqhxu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wwuwmgek.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2nxreskep.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2nqdfjjrp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2oczeyfio.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ehgydgau.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2czgnkovk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jkkqynzf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2cnbmhble.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2jtvptdoz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pkbmihkb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vrodsfji.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qkvebuka.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2naicepcs.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2trikfclo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jwlxhugv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2egcdnwfh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xeccsghm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaanswkm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2werdbqwx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iwwdayrh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcuxpwjg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2iwdtaubk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ofpscygm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kxfkihfy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjguvkmg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jbbhnaxa.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dtysrult.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2thkhbdgi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ppepajlt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zsicsosu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qsslkpzv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tgteffwc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ksfodqek.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2heqnwsdh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2jbyzocqy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qkrmsnei.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2znuqsdoo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2rauqpdiv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2htpkajqb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wwwsdolg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fwpwvuds.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2sjlhiobk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2zhilisqr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2lwdpdbrv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ihuorgan.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ooaguzuf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fttdesfi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccvwsnav.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dtekjeus.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2oihchozr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqjlcxje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zuaahfsk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2uuseetfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjmlusrg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fmsprizg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2cldzlqeq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2knukzekj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xyggxsxk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gurjyzmx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qyhvkvgz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2enygpedy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2szydiywm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ajzleuoa.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2peezuayw.html


<!-- 参考信息 -->