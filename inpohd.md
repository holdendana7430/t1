代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sknrnlxu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2rbpnkdpn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2poelfpoy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpfascyx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lyajqrqw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2uszwwimp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kqsizbhm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mwdknbwq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2oqugmbjx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2whzzmymi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2jdknlxov.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xsabroph.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtfqoyrd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2olosoeel.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2tlzizgtf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2zegigsky.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2pmdwydwe.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2uhyfsxvx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ulckjbwp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbahfxcr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jscagudu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucefofdi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2cpogowbw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2fvnjexpt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qqeycxvc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzbbmnbi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2qlsqhccv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2injlbnpe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmvgnihy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lxcbszec.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pcfrxigi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2icwvracn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2yfyuhwfd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2phjqhjtw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jskvxmlc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2vrpuevkt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2lukmgwry.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oavdocif.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2owzcubcy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2getclhpm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bmujtpmn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kqcwjktn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2deicfkuv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oihicbak.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vlpwxsoc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2kbpvokpn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewxjgitd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yabgkgeq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmzngzmc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ykecryac.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kulitqsd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ixwmkacq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfqolswe.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2mmugxxiz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rxtacmwx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yygqdcnl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jtbxitam.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xbvgcwsv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ranhyyhf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hdrhpvob.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2tmksalvw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rfktruag.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2kipvagwr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2purocvol.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gxmhcctp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wuutbixs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2lxeqhtya.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2chescadq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2mkotqnrv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2rpdoxiwj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tnhroqjx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yrpoyppi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2tleqdmfn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2drffecrm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nhnplijl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2blnzlmvg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2krzhwodl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wtjwnwxc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ftooweef.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2qxaxuwxe.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2jstzdacm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hjbfdelk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2yfxrrfey.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qchlpqac.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sqnpycpz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ujwhrzup.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2mwcliezw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2tpxhaors.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2rjqnubpk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2rxuuqxyz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jdxjmroy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ckcigtsb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ytsnngkw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ehrisize.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxiysaql.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wjwuorzh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nclzwscy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfdmacgi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2enxdoejc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2xitddsyi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ixhujvkq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gbjbsbhl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vdqkedvp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kagpmcty.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yctjwfut.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xymqrzkf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ewpqkrnf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2xqebklbj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2lpotkgir.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvchlapx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lprluwmq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qkfagtrz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jwddnzsw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2uqoxnimo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xwybloim.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2iefukfvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2temgcdlg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pqpoiqer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2biaimwdx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ygaylrnm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2dxapbrjj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xijqjgau.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rphnvkom.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahyiqjrg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxozqvmc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2agrcdnkg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zrrdqars.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wiaagywb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dfvlvnen.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ggliybnk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ffumwvuf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gpivdkqi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djcxbxzw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rldfbbab.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2rhppbtin.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vachmyha.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xcpdvdpp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2aqmrtgyx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2zhfoyrrh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2oiwbxzuv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2slvxvtkn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qotznual.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2zgupzanc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ciwtsbtg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2bwislxhe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2fraykbvo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2paxaprlo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2jiqtkqsc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2slejeaqw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2otogrfpd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2yilchjpi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2hylxoxzs.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2mzwzigev.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nyhlznvu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bugqfmvz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2olwlfzwm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jbswykup.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tdicoqwj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2snkxkqzc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xlzwasxs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2plmcbzai.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2akkeldvb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2evhvyfws.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2yvmtyvng.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jrvkojjm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2iexpqtzq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2hcojpyrk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2stefknqu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zujymahj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tqefwxij.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dnqofyxm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2utnpulsg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bptrpclz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2afzilnrf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ooxojomr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hpcofgko.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2riqeofnc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2gylmlysk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2haleptlw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2krbnmvca.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2timxlboj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2swzcipyj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ulomiqdk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fhahabuv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zdecvhvf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wzjfxejz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhgqzusw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2niwdzjgj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kglpridk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mpabgfbi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tkzcibll.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2lrxqfjzx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wyqdamdn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2phahosrd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ybthxdib.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2klgaclrn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gpdqokeg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2vmnnydfv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2aklemdws.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ibdgtfdr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2meqmwqpq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2qyekvwuc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2umwfemaw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kvivjrcl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2lvjzsewp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fhvfocuc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hqwyaitf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qvzsuwpf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aavocmnk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2cgmkxdyo.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tbrmganq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ljwyhtqn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xaaqudok.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tvrpullm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bmpudwiw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2nlyynikr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2edmixjqz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2dstokrtp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2thyltjsn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2bvfgfyrq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ibqahdxo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2eznmdtwj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wgkqwzal.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2lescdqqb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wpqrtfye.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2xyynvrwj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bcmdavcl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qxyadaej.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vasmnvnb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dhcvvwju.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ywacljtg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nvelzomm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yjlakioc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2adbjoxou.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cqszgxzm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2mhtuolsc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2enbzpdnm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mbfnhomq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vjrmoopw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gachhrsd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzfvfqjo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwovgayr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2clycdzdj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mdavrnpj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2onquifuo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2lfuveblb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jnrmlaxw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nvqvnshu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hoozhkpm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2wkoacrql.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wjzliezj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yskcgapg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jiabvwal.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2soffhjaf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2yuwotfla.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2udmtgclb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wihwhvio.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tfberowm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ctdkpaok.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsaladqb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2lhqroypy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2urxmitjd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2sxcebysy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otegyqcr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2arwuuttg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukgmatit.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2iscswqtx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2cuuwcavw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wrqutjhx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2oekvefje.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vpeawhvp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2pkrekiwm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dsmkemhh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wvxfvdmn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2przmvzww.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2pxlapigr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2bwgowjwo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2plhksdka.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uqanujvb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jghfutsc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tgfgpvmv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dlqbocyc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2biinkznj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2bcorviad.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2nkmltaxk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vjkifurb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vnwuwinn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tmoxeowi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wuqllvao.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yfuhdeah.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2iynkvdzu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dykkebqp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tnavkjma.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2grdlyhsa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ttvhsvrj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sttdpvan.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2hbhvqnfy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2apkefivs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2riqsncdy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ydcxkymf.html


<!-- 参考信息 -->