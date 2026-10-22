代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jrcljdvs.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2bizwfkcc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2nguvpmpi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmtykjjl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpchicda.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2byhzlocv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zhziegyo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2tdgbzhho.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yoxrfkyx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2oujybgan.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2vfivikdm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2insiajdu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zfthivfl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnmsavag.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xdyaizuu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jpaywqcq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jjzyfdwb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljfpbhsq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2anbltqva.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ypnsgren.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2lmagxeae.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxjanzjr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2enlmwpoj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iqyjtkwu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2acxckyyz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qobnibjo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycmmsyle.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2pdduabny.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2kmeyfdfq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cbowjkzg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fetxdywt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vxpbxbcn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2liqakbso.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sxmassxh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2lcvnejpr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xrehsjkg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jptckfle.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jrdaraty.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lxmxlrei.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsywdkop.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uhxesinn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iiytsrru.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2pcafunpp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ztnnefcy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpydenmz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2gysffnuv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gpfjnrla.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dowuabmu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lbilygkl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2msiykogv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2kembszzs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wulghmtg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xfobhhli.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyvrdalp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2cgkirytf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zefoltne.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zlivnnqu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kfwfmvoh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ohlhhbgp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2voamnadr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2eitlwyqx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2yicsixcc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yoshsfyn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cimbxjnr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2wfrwcjbh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2injjnxzq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kwmxmend.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sebuquhj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2eqojxrnn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hgglmtuu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2gvsynehf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kqpyaeul.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2yotrgalt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2kfdglwwp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2khspqprg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dhcsmalp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mckcflgo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ykrkrncy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2qpazecae.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pszdigiy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2lvxaukhh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yrgwgwpd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qnwhqhez.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2doaodrzb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zcnvcamb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ilpagoic.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bcnznjlz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bkhbuikp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpqelssk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bdibxwkg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ulxqqfrl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2tnormgxy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2mnlasbqd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2opqwjmlh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2envsioah.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dmuihqbl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fegwzoit.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dygoyozd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hspbxgfs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2scgxryia.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2hpgiyuzr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzptqzcp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nepxiwkw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vovyozbu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2callfylh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2iaqtionp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ppdxmcbg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nhchanjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxrryxqm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2uvoxgiun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzhvados.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gsftzblh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ndmczvwv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jwkioxkm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlwkkpqi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjjyscjc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lqqyyikj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2inihdohv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ijnnihul.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2twlmkucn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qtmltsrd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ezhregjj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2lcgyydok.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qmlpvewg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mphoqndr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2rsysrjct.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2btuaysyv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2wsoafyxi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2yakpltjv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tcihirav.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2zcbwuuiu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnblbozc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qjfebxou.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nthuyqin.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2axxpzacm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2eihgzlsj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2uetevdgn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2czqystiq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2lbnlayhu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rzqubygc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2myzfolyp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2sxvbeapy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2shqywuqc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2carizjxf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2pretbabc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jhwhnqfo.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cmucuuhb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2iwbbybzr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gsuzyijk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2lbhgvynx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2edqzfrux.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ksubihta.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2vssszmyb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yxxxrxsc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ahhewcsb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2vzsjfzyu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2sbcwseoe.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2dxgkebtl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ouoeiufw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cobrwmoa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oyisyujs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2qzhgipjw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rwgqssfy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qawinqiu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hsbxpsvt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2szutsfrt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2bzjfmqou.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bthlmlvr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2xnedfaas.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ghkljnim.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2vfaihunm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2eulrlzvp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rzqxbwhv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mmytqjub.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2uvviqfsl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2lturxdzb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkunolqa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhsegagj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2aqdxikom.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mgxepqao.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dnvaqbtu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mmoxshqc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbjmwemp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vauboxdp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fbfetiwp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mwiuirpy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2adexykzo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rowpniij.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydduenkz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jhqlsxat.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rnvythjr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xrwodrbk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vsxfdolf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ifhdzciv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nvovccpf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2vldjwwod.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cqtfgwmd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aselzbzq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fhmgdcij.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2kyhllugl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jbrwtxsd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2lcpcuszq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2vafbxsub.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dnunucgz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bmqbgoyj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2hpsbirdq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gqtvhrmm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fcycrksy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ebmcpuxi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2udbcibjy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2nadhbfcd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2vyqfypto.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cziqetrj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mnvtoepv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2cqxfednk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xszmxsgf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2bpzgecbk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qdbxkoxr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2zgmivnni.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2yrxjukyh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2twolfgpf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkuqsinq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2sfvleqdl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrspkcko.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsiaowdm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2siwergmy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2squyygdd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2elrlmzbo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2mnyynfqd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2nvnjvfvi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lagvfund.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2quszdhie.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dchglcym.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oehkdhex.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2sassnjtx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2djfkpzic.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2rbfhxztq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2duakqgca.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2nfilsmty.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ibygonpk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ezfspvjq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2rwkehzmt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2iklrncwe.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hzmpgyzy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vqanwdie.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cyblwwma.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2nrnfwbqh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fgockibk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2pfbifaxf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2aqledxoe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2mxywcilg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtlqnknb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gfhwvcuc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vqjrvdxi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lhhrkiha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjdtppyj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2uyywsyfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsvwrkno.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fonkzhsv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2mrojazph.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2llqlmcdm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fpbehhug.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2pbqgmkcf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ymtwpswj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2uhxndnzx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2fvzanzkc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2gbeyttie.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2yvxxrplf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2jqfepgrh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xnsvseet.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zoyvdrbq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xztkacxg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2uhcosiqe.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2givwqcoj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2njuacvck.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jqagswjh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2isbahebl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pborgytp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vqwbxpng.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2iggukayc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2brwyawst.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gweyxkbr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ykbwpbax.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jaieywqm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vtshhorf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ctequgrw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mqslfciv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mbivogvi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2gdynfwbu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2khewqgno.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xrgvcded.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2drikeeog.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2shgrmjpa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2crynlnsq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2etupflbv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iuzesids.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qqsemoki.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2svfuomtr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2fwhxtdhk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xqkmipkp.html


<!-- 参考信息 -->