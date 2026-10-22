代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aavjqmyj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sycqznja.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2avgkswat.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mjoepqlk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2aanhwnmq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lnhdsflo.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hkjeemty.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ejflbjwx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2itmecqpc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zngzxsjn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fypnorzw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uivjngvp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fdfrhejk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ccvtahdv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qlerjmgd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dcyvlpwt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2udpkhebn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijcifkdj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vjwgjozv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlkmgver.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vonhqoha.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2etdjqwbd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2eqhqolse.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2zfmbywwg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2koumgrfy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2qixflgqn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wjeyjwhe.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbkuppeo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yuzdzvtk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaxewezu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2lcjhtncu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kfpbhray.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihnpvuss.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2evqkupsj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2clvsrzfv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixwacapc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lwatbbvo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjnkmwpa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2frglqqzf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hpcjslex.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2krwolsuw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2stbtmfqp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ssmjyash.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wrekpbop.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cojutess.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbdaslyk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xylistbu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilyjfffs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2uapbgetc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2yzawhacc.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fbefxatn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2wqqwahyx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2psxnoipk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kdmoxozt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ujjliizo.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2engqpirm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zwsbxwrb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2caktdioc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qlrodjsw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mdubxgig.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2nzeednnf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kxerodhk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjxvwryl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pejbducg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uxourzwp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ijznksdz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fiowltqe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2oaikbodo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2askxnrkk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2myvftwkk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2stwbcgjw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwayfziw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rvcqxxrk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kkjvzhva.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2uqpstoac.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gllzrxvo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ymgdwfjp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2muspghid.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2awhgobra.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2yvepzfkc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2adgwddqh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fhbaordw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jhktdjbd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xokmqbxq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2bkodfjrg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2mwkrksaj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2missicld.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2dfzhmfug.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2dgcpthfm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vhmdcgjg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lozowija.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yvpaddys.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mmsymzpn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cefzowem.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hbwguquc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2pgmviish.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wvzsddyk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2fvcagbub.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2oagfnlgl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kueieucr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ylwxndgx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vxfyckgn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2smierkii.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2fzmmssvx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2tuldpapg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2vrfumjgz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2bhvhglja.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2urfiboct.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vtnkiayr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxeghyua.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xxvaitbt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lvojdhcx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jymajvuk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ksuppdac.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2cfgxgfsc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ardhqiuz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vuvbqjhh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qmzlnlvt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dvlvvumd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ctnwifcl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zevrveoa.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yahsqhjx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uiuqgler.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qttupyeu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vuizdlri.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2delriscf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wgijfjlf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qsvdrgot.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ietlbeda.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tnxfhzgd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2cjpcrewo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lsojngvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxchnuet.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nvhtyprb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tknlqate.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvoxcbsx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bvkppidt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2efyklida.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mecvaxbv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjyzcpph.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fdgpdiam.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2klvnhgvn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2yccccijo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ajknbbzy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xgfkezpk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2myggivww.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jenulwxs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2matknwuc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxwzdhww.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kuoxespn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lphezebo.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2yapycvqh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2uvctgbol.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2dqfalcfl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2yyffcbhg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldklywfu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dyxqhkie.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmkbgxoq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2elinbvhj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2sdncteew.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2agqxsjel.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wmykhdpr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yhoozfre.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mcuoaapj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ptdllksi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dfevubwj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xuyaxhtx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ekzaywik.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2svnkzryc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gioddigm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lkowzndi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2dbfdzzhf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2iaplopzn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ehpjafdc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hkbhejia.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2drjrmeue.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2yrtrzbxc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kdiwovfy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vqvuiwtq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2rhwtojxp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bokvfrwt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2bevbydls.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2hskdkksb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2whkjbzod.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yyorclae.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ofwdlvnm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qweayhbz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qtxmjzsn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kjqiwlbk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ygotnnqm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xxqxifbz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kmmetfle.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2pvgxdsqu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2tyaddfly.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hqpmqdct.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2iwdtbkrk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ykospvvl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2viwlilmm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2psagyhie.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2uqlhzjvv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbsaxyiy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2esslzsvk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfcshykr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2igtstdkc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2hdxazscu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2yjfyodoj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gmnxwetz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kcaxpgav.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdcxhpcc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wwqmcjzl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ugwpkgva.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zwxtnkwi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qsyfewxu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2vhnxlppu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hodjqjny.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cfrkhznc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cvdudxiu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2smhznsyx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2zuoqgcjt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mscuclzp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mszjbeke.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kjaanksy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nlcibsfi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2hnzognjp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tktywyjy.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dappahuv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jajbtonb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2zyhzfxbb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2oociwwae.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2yiamcvux.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2advpkjdh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2apmeqsip.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jgqswzlv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2evalsqgf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2rwqmvqop.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fdpwjlhx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2gglxzccj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tgukuuoq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2stbzcfxi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zjptlnyt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2yixbnbjm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rqggfuud.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lsduhenp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2zvojtswy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bjvamybe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dbuacpss.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2mbpompce.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2difvdhxj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fazsxeof.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fksqvety.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2jseclraz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2wynxzpqh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2udyhejcq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ohvidqyu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xhnkwkxb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tfxzuyrt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppvfasfd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2lhaexeto.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2abpyiunl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wwknoupf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dmditvmd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ingqngbo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2pprbsuwl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2btrqmeqj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jtagtmnj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlwyxvqy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wodzvygv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2akncrvtd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2fixhxumx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tonkberv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jkdmurzb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2qscbkkge.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2dipwnzhu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ogccguof.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ptomqwuz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhysudct.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2wuxlbdpt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2wsrknklf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nualloto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yitbgthv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vowuhhff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eimcaazn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lbruxtcp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2oigdtxax.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2efnzwjbl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fomtgewa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fwoafrnc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ffxxlsyt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hinmigpd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2lykgffbo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2nttzwpwq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2pwijdjwo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mrdlhepq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2rydhzhnj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vwznwong.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ouzwbjiq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jhfreuuc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ikbybepg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xwnfuyld.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2burztben.html


<!-- 参考信息 -->