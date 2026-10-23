代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sesmqcwf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3hvjnurkv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3qyhcsypm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hasysbvz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3csnfxnld.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3srsrxfif.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3alfpxqcy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tixfvery.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vltuiwpc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ovkszmyv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qrkfjrnb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xybqopeh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwsrgywt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lgyrsrvb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hrviunor.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3oxbzddnp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jeykiwgb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hsvxzqgt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjaeasaw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3mchrvlbu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3usbrmisf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3iaexdjqn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3asleigbf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3itkzmvda.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkchzuvf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ymgzempl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvroepdp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lxbtgqod.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jzyyuvwb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ppnzbvqx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwikjtyu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3aftulzay.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mugpbkcs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tczndtnp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mdbsnjlm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sfosanhv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dnpknpzr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kswxcdfl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3gurnkgfb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wlepndje.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3vuqjjukd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ndrymarx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xhkpxzlo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3upqyrvjl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fxirzxwh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyxslfuc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3oyncvasx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3dyjhndyn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bjxeatpr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xpqxpbkc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qdiubcgm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3bfxzohdv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kucmkden.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ayyafbpj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3vgbaromo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bkmabgez.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gydgxsuh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3dazeobsy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3acidsbis.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3hwmwcaov.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3asjntjki.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ttbmewqh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vzxvyyys.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3jmrmjnpx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3dojsljva.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wheicdvm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hqgowpnv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cvxufucz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3plblkwkg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3jknirmio.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uvadwaua.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yzpcmjrw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gxdelgvo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vzgtlwud.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3lybxiugk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ojfmaerj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3moxwcgmn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kkwoywyi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3yvkhipes.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dnkstlxy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ajokphny.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ieurkkhg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zripaclf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3vugsdaml.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3vxihzqri.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3dceedzop.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xuuopcsa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3tkvxeozs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dfmsktwu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jvjvmbvb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgfqdnjm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3owxyyxco.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nlbewbwh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jagfkxts.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ybcmxhat.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3qzdnpieh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3yofyyyrr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gawkhdec.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ylbfftqb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3izytsnfq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vuexfiat.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sidovkxt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3udzihloh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3tybflmwn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ewjyhhxz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qldsspnh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3munbdntj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cperleux.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tujnpizw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nojrpvvf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vtztwjzh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gkhctvko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbprzffs.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rnhbpjmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcnaqrzt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wuyamzht.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oqrdkbmj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3okfbuvsl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkksqdgj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkcnvzsb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3avcqzzfx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3oszhnrcc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3sezfotfq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxlbgpfj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3wbmpokcz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qwvllvba.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsrmtnpp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3diogfbzd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hqgoavhi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3mvsuvtht.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3cimyeqhb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wssxinxw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zrulkyso.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3pvwnknsn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ocdwnowz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tfmxmuas.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcwgdash.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vpkkoeir.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfldsmqk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3rblngsvf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rogxyjtk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tytrgrho.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3nvceupyy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3gmjnaawh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xkzkqwex.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tronkvph.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3mekhsakt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3asrwkwjl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zjbdgoqo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gpqtmevp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bkinfffn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3qjghvpgf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3slkvdato.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3kcfqbnfp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jgrntlfc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lvqvcxrq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3migcekqc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3opszwmph.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3lzirjtpi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3memukqpj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mjofccmd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3zjlxprfo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3lvebfont.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uzbneqcu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tzmuwljx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3avjoxhzx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3yomflbji.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vptuobki.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rjrzwdnf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3wegoeqos.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vdzzepgq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bektbgee.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3jlfgimkg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3mryynips.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xivzaisq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qajsmgze.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3kxheuaqe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3xcjbimvm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3evlcdtyw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3weglhfrc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvaouvkw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3klwdazwy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qbiftmhg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3wwmfzmyt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3zpimpvtz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zgqosvxg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtyvanbz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3oylldfig.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ocfpytfo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vmduyubu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gdvqvfqm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hlkcbntu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mrdfglfj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3klppfoou.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjgdcoto.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3layvxzhn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3efxrvprz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3erocdejn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3hmdombor.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oyidwhut.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3sdbutazp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aonyifbt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ygfdkplb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3sajjmqrm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eyggclnj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ftgoquad.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3uksjfaxt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dmrwajti.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3menacfiv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jnqsbqeb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ddargkcc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3atpymepe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3cjfhzmvk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ggfausax.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3jwzcowmt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3raookykg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nunqargb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ahvulvrx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cwlswxjh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3coxsnjra.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jebmbbcb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3cdiifdfc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3yyorhfpr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qmfyaprh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tsjqotdf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3oofbdktm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ebcdllgr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zntusgnd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hvnunwgk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wrpjowel.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3pnkdnjnj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xxwlicob.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qrgyunwi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3fjkprndd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ykmnmjla.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kgfiyzfe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3pdhutyno.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qpxzreke.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3cgmeshcp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3djhjofmi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3jlehtyio.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xfjfwvjz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3bjdblrkz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rlsaohse.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3loaikahi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rngjzrag.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ollggrlf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xkahcyyq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hxkjluzt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vkrvwoho.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3oqkcprnj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3naxjzjfk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qsntemzz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qxgjtjim.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3bswbudvx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hwzcggsw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lgqcglmy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ietuyqco.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqmhzcpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abwjltot.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3xbzcqpdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkcbynnr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ohzvoxst.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ltzhllru.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3aitgkpiy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tzymneyj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qtmfumov.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3sccgsxpn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ykmlkhon.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3awxcsboz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3dhmjackd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3nuyqydfv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3gtmxpyuf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hvvieycq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wkrudeqx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wjrcazzm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kkkdottr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qcihdwia.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3olhanhsr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jvcnqylc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3bidyrsxa.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3csfaduby.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3yjsnxsfd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ylgawkqh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kpjhwyzz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dcytpont.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xxtxhwyl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ysfdktgm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nbduexap.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dsfvihot.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3jkwlxvlz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fsubiwjh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3likthjas.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ewwoqhzs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3kymmqrxe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gbxayiqc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zhfwqckm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dqoitjkb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3yenbjsex.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3glsxoiuh.html


<!-- 参考信息 -->