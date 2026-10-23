代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3pvynscix.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wupzzfqd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jxwoaxve.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3igjnzxjv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eqhlgghw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fjqgcsva.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mcnaprjq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nejfwcmi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ttsrdcte.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3xriomnsp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wegzjlki.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mjlbrvzm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3vrcbrbrc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugsjnfzt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikinvsam.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ljdrreof.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjboodbs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3cnnhmnmh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ytrnqplv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3iikphdab.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qgrcyjfi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3lnzvttkd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzlecbxn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuheoory.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fslcmzar.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3huxfizld.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3mjmuwojf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3vhigpeno.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3pbxuclnw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ozdstfig.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3pskwsfje.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeiqbmlp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dizynbth.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihcykfgl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxjykpyu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3eqcgtali.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3hxakvzwy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kumwtzrt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wmrjobyy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gxqvousw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppqmdpxn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3quasvscp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgsllrwg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqkwvfqu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ffgkchpu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ydlmfkpc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhitdcgs.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tfxoxgbu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3junjhqhw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qekvnnkg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3astprljz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ygvmfbnr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tvajkjdc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3owrtzdnt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3fxwvpneh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mquogxnp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3pzvfvihn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xozacuge.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hauwvnkf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3njqvexuu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmwahwrm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3odsfkvip.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3iwvuptcz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3wxbpjvww.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kzmdbntl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3rqjhfdtm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ccgsabnp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaxtpgie.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3daexbunr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qpsrawsu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3bkaivsdz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gsdlmcpb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3uxwduwce.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3uibpwxgj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ylsjyzcn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3vzkouagp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kjwjpdls.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3asgbkkdb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rsmguntt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3cjpeemeq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3bfjsukxk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ujrskzym.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3blahvvoi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yewwwewc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3salpoadj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3pqacsapd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3itycnhsf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hgmrepqg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ticrcgcq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3rlwhivcl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3npisghyy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3udhpcptq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3shtdudjd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qpumhxcy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ztilphdc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bigqcfjq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ksevuvaf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qgsnsvnh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qdrefbxo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvjcqxn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3qijnztrn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pjjyyhlg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3lppqptss.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3cmlugbnv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3alqquasz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cjskynhe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rzivjwet.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hpoirhzl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ddkdlohi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mejezorm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3juhjkjpk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lxzibqpc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3camtaxzs.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3icodclrw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cnlstaph.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pvodmmwd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oneaftfr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ytipyppb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yvysujsz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3nwbpvbbw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3yfedsxvb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3lvtbhukc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yxqolgik.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nyvxuhmh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hzfdtznj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3prlzopyj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mhsryqme.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3olkqtcsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkgqndri.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3iqflgwnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trkgedow.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wxeopjhq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ytumhbes.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hagsyvjx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iaqkmcnh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymubzmgz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3orhjrsgc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ipetlbwg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3pbemzllb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hpjhmgrb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sldlmzoq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bcrsayqy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3sxjnfemb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlyetwyp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtloxdnu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ngpwbikm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3jxyspryu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pnzohdsx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3sllpcyok.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rkflocww.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dndthryk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3jyjyrluj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3brnrjeww.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jiwcefbv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvvpdmhg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3opsghjkz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3aulchsdm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ttlxfaef.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3hbqmocjz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tsrqsjsk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3cpvjdbjc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrogsuts.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3oidpujbp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nigpciwq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ybyokleo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ygmdksvk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fqzjvkxx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3plfcemjq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3chrcxqgz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3vgzobzjs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dcixpiqn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pvbtpgyf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zracfjvv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bictoktr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3gwwhudxh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3znfnibyq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wilmkpgl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3lrewjzre.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3hfszfrgm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kxssccdc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yvxzzcgi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3lfrtgioe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hrboncic.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wrmzsikc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gzrxfoap.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vhbexowc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3iihpldwv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pzqvnqtl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3efxfqniq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ztarwarw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3aujrsaji.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3wyedgrmf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tusgiewq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3hvqiufdk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ymuvagfm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3zeajhchr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xhrjybql.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiyunvmd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgecaunv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ltbfqovi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qdsxaofl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wfhgjbol.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfewhpdy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3fnxlwmbf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dmuqyagh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yuoerxqp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ywdgygmm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3evlwzmpc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqwbxiyv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3piqqrwkf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zvqdxidu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3mynzrjyl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ixnqbwsh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3snhmysny.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3cwepjior.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gfqgahjj.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wmohytuw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gnsumesy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nqqixvau.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ezgnfofk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jpnykcic.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3obywvtfs.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ipbhjnmy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mslezmhc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3olqnfkwc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3babwjmwz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3hrrvhkfv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3zjggbgrx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3izzwfkjd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3zyfsrjvg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ufwxfonl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ybbjlfht.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ldvoyece.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pqiworxt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zlfjkozk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ltsjqywz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3hovlnidh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vamvybhd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqxpqqzy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3gancjgix.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jmfcjgbz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3avwupqle.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dcspsllz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjcagqqo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndbiicbn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3zgliaskm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3dfciyhsp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fovenzzw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ecuhajhw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zdtohgab.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3obhbkgho.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pwvkwjoh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3upuekzbx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmvjvggt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ogficxmp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fvzjnfie.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3xjbyvbwb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3rpxvuvph.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3sxhkxciz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3pcigxijv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ousumspo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3wtyhanyv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kfnuaicq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3evxhzvho.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3twjmxrma.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ukqhtzyg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xnvkqerx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ipruwopg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3dxprusys.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3bcsnsjqe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gueflchr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3lcfmnfhr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3bgczwnis.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ephmtoie.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iyshhpbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnjkceel.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3yipxkljv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yocphens.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3znmteclm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3emgigdez.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mgecxlsq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gidfvsxi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ycwzwmbh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3muctqqmv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3uodelxop.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jqlszvno.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3aujuodag.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lasxdjpr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3rcmfidby.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3stdfwcoj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3amdqqeid.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eortqnws.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3dxfadnjw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xlacikkx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3oozceuot.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3svercdnf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wgpzmniu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ppykktbz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3iwwnfbum.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3konwdlqn.html


<!-- 参考信息 -->