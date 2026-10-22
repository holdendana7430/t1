代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ufikolll.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vznegrns.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2sxtxfkpo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2lxlvxmfq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjdbfddp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gnqznrcc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2azzwyqji.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufnugcow.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2sljthlxv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2yomvqtlw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nybtieke.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cqivelxo.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qmiizuln.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2qbumhmip.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndmvdxto.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkzaeccn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2oynqkdkn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2borejven.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2avmqzcsx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fdxnzblw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xttauipj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2mqslikky.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2meqmtguy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlvzqccr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhwsgddc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2nuvivgfd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2yibklpsr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2jjwqmllc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jepcohmf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2yieygzjp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2znleawzl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvzmzytw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cewffayf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ehzcndjk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2oyetazqc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2wefqbebe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kvxeboks.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzuytkym.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2wbtenvpc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2bcqzztqd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rgizbdin.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmbhugpx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gnvwhrcs.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaqdoudu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qnolgafa.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2eyujdhrq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ripwuohs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kieosmfo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2cmsmfffl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2skeltovv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hxhgmvvo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ohqchchy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oiswreju.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uudpmhii.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2lvuxxqpa.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bqkobvwf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2avaysiex.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vkvieort.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwftaizw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pympqrrx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hwdyyldh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqhjhmzu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2butasyei.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fqcmghdx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uholvkfo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qsdmthrz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2clzdxesl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2jlkvztmm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2necxlshb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xandlogi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2beuicjuz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lywsoydc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gkpwijtq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ulxtcxgo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jeofmooz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2kfhyrwkj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zhwmhlhk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qrvqhfrs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dtqumdwc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fmrsumqo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2pxprckxq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xabmzdts.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cqeikema.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qdtifbuz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ihxxpait.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2bibcroth.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kcpguhuc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zrxgmxai.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ahqdsdce.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2uyglexac.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2mmxplqtm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2oyjoplku.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gfjicvzb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ieynshdg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykbelvmk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rsiitnza.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2eptfmhlh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2etweftkb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2chhhdgfx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2slnpapkc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2bmxceuql.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2cesexymj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fsmwbvcv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hflxdxps.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yeosqqwf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzkxtcko.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uldwfgpf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rrqsfngl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zwwpbrtp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bvppghfi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2muetiovd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2nyiwhojy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2tdsqtfhp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rhzmhlhe.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2escfdsos.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xgiopghj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uncavqfs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ormzrzod.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mzcbtgeo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2npokhjut.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2nzwikjwl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2dxkhgwrm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jkvgetzc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zufluwhp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2citugapu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xexvkddo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vjdxiojb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ovvupdel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgrgfmuj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bmvtylvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbhjzoda.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2feljmzlj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2msxwqvbe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wzytzxpk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qrrryesa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kwxjjgxu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vyeyspmh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xvphngtv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2wsbzdqjy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcrlantn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2oygcpywp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xyjwixcp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2bjnrosjh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2srlqhvku.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2onnardzu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2anapylfu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ngnasufl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2luckbhvp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2afhiuhft.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2sghkhaxb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2lnnwqybj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqypgvec.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktaatrgl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2euuwcmkn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wsnwsijb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2vndfbdxs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2evfydbfo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gafqfygx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2zfewzitg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2amnguwbo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jyccgbrx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fvynvvns.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xuaxkxbs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2awfvxyco.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2dgmwendz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gilmufqf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dyjjywlu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ztcqfbpn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qcqsroay.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2pahvralz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ebwjregv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ftzkqcio.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2llikaoaa.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2aeuhbaaz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2deszjwtw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zwpfbxdy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fwcnyywp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2oftlklcx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2baxtnmcz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pgijsjjl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2twwrsbio.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qshhfpln.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2dfgnrwfw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qecpanko.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ciffefce.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2myhcertx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2brxixxbt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rqonlegt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ehdnenqk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ojvoycgp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ajwwirzf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2qvaphnpq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jwpvdqnq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2emraofch.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kuppjgqf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lcdimzrt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2siamgtxg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dwodsrfz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmiodyko.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2xodtdsiq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2gigpnhqs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qdxjkogs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qmqkuihb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ppteiqix.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fepoyguh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mdeezewg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2aehwoitd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ftddkhya.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdlwkyxf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2klhgntsm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvmoymfp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2pwirliqo.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2lohulnuz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2oigapdug.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2gupmorss.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2aunarnpm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bnwybabq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lcusanak.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wkegtpyc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2hltkufzr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2atwiyuyy.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ntcmrrbr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2syuyzvha.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ibggxlvq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yupaiehr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xrnycmyz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2otfmhnhp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zdreexlb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zzhetien.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2mrovyoqe.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2hpldnuzw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dfzjgzbh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ygtiycla.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vnwtzapi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jvuvvlje.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2dihzmodv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2kgdjmcpa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ippssllk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ewiktphg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2omjkpkar.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ndcxkjkf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibcxgasl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2eayfhusu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aplvllwz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kwciwrud.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2liayjbbm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sgetojit.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2enpapipa.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2birqoltz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2quunknjx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iuwwcaip.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nnaavlur.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2elifozqk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2enrubirg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2lizpycgn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jkpcgzfn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fsdnobuy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2sfqtdnhn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2pebqaldr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qkichgcd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2firlihes.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jscmzwiw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vvjvnzad.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2sgrtwbua.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2wisavmhs.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2udkzyguj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2oprewsnh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vftwuqxf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2cyrrdijc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2akililel.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lbfkdxup.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mogurxnj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2axaybmmw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2kvchxuqx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmwkafmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihwjfixa.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2niezczyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cauuqmna.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hubnqasr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2okxxlqtc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rdqtrkpj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hxhqiifm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2yixsmtwe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2yyncuwdh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2cdfucneh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rpunhrnb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2aeagumja.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jggkqsod.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2qqknmyxc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2epfhksob.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2aalndlxe.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hlptmqih.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2awbzvwyf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tdxtuqam.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2heaxnqvx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xdynouto.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ekbwzubz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2agtxgtum.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mfmsfbtn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2komrwdla.html


<!-- 参考信息 -->