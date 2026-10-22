代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2psqxhkhk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2vrncmled.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2iescxyae.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgjxdlvp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2flxsldax.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocegnrzj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2jpkkddmq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2tdpcanwr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxyizwhp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ymzgybmt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2uvwjwafb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2yfactpyq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2boflonfa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixdzijhh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hvlpipyr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2lxievcks.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2yprzwmfg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxjkpcpm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dhwlnwtp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2krqstrfe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2egdsbnpq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbkbqxxe.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sizntpob.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fvzvybte.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2jzxwdstc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2jyzggndl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jbqhrmte.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2aoojhfbg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hakjmhyw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xlpaxiwe.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hkoksqdh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dlhlcxfl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2madkonzl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ncfjkcxw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2lqxgbwpq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pkzkcyeq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ppehpovr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qpnndggw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hqhggugq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2viosummu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixocoofh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rihlwmum.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2moxcuedo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2kluqnvej.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2awhhphwv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hkjdcqhn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ztogdoqb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hxwcfjxu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gxmendab.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ncjuocgl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mlkldgmi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2twugscgl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nrsjrrra.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbhenahq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2qhmkbqhq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2nrshqyrw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2uhedmojp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mlkonusp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2umwgjdjv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2dvpmjhgk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2wfkyxncv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mmqojmep.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2gnbckoju.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xwjypees.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ollglfsa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2lfgzwgry.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pwxdrsvh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2krjzuqsp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2riffkcrz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzodzvsh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qjhzsoyb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2stjkulpf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2osypyqxf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ytxftrqt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mkoedkby.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mtazyccr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2enpuryec.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2cvmtunet.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fjovzqpv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2yeskvktc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2khhdeprl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2jozlexbl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yfiirdaq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2giinnjtj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yykhlbuf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zccbaopm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tzmkwuca.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpfnbvgs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gpahtzzf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2islzfgnu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2chkmbkdb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2eywjhhnj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ldxgsani.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cflwzhwm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hhvzpgio.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eatufgdv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dwrzwzbq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2djwwcson.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fkyqqlyy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ksnsbhmx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kfhahzjf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnylnnmg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fxxdoupx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mnapfnpi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xlyspjcc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2quybpyic.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2zyuayyjv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oeveyozf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2orftkbmy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ufyqbcjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqvzhhyh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bffwdccd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rmaexomr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mprlziqi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cgxiwprg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aldqwjbn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhnueopb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qhxwkitz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2upcycmbm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fmaaqqcp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yylmcppm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2dhyfixgm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqpfcnvg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wlqriabl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kjjalqya.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2pxlcxbnq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2yjeblbuh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2cdpvjney.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2isilndwm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xeahzewt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2auhiundv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvnvqxwl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvmcdtch.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbvqmdnr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2goelfjkh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rkmdqxdj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2gdbhligr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ydhqvxha.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2oxbwjhvj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ygqrzzlo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ksbequgw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2psmnaqmo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2hjshtocd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2owgewlhn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2zqmybfzt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2excbseyo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovqdgdvz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2pjhsibbo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lqnnspat.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2cfxhdnov.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iprroztd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vhdgvdrl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2lylzfaeo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uxbkonhq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ujwvmixl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rjfdvruo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2oysptede.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2twehueno.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2milghjyd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2anfiotwq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2afdpgkop.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2iaytukmp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ctgsklld.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2feoftgov.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2swootipa.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2twgcrbpr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2pzcvyimr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vzuimlws.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2xbowlvpx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cfaihrka.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ermrgskb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2icritmja.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hjmbxnxx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2reqmtiqf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kberdmoz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vagkirjb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ebjlabxf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tbbgrxqi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2sukfdewb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2sdsaukpl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kriximug.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2cvtsocuu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckgrmimf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gscqflgs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yhiagxbt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mwkdvoyf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2sbxnjlbj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mjzwfwfv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jdtfsvtm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hjyxvriw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mjdmvfvj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2nevvdtgn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fzymntpb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2tfchfzuo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2mydzkdzm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bgqlkabo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jfotalha.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xuiphguf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hnpbvsgq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kxrqeasr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wwmgvpcu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2lkducinx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2tjqprgol.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2iumtwfyo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rxxkjlev.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2koyrtjcw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ogtbnvzc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lugxpylq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2sqgtbxez.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2nrlysqxg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2scptkvcq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2vvykjdak.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2onikuqhu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2chymzmev.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wpscamcl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ykkimrhm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2eaifxebw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ypwrycio.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjsxdcpp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2mzgeetxv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tcgkenoc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfelbloa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fzcxeyyv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qlwhbcvr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gjqqrwys.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2vtdqjppm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lppayayo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2aiflaiom.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zsasyuym.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rendtptj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lywbluwk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ljsnpzcq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2gekryybq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhkavole.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vvueaxxa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2edbfulsb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jcgcjndg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2jpgkaafy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rzylxgrz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2eutqmpts.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hnbbpttq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nckghhqu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2azxsyjnt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bbelouhq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2cybjudoc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hidznyju.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tnjpafqm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zzqfykiu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2eldolmul.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dicevuvy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2joxylwka.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2iwkmvyqp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2pslyoadm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2nwidgmuq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2yyqnzndc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpftzaco.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rxcmurlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkbzgwan.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jgqeauum.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2nkrafpuz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kojueias.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qsuppkxp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2wrfekiwd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2avutrtmd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2hytgczkv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ulnvffah.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2anrhnlvs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jqaghafz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2crliohrd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ozrxtvoa.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2saixeuso.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fymwjxoj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cyiwwlsu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fowothln.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gxwsoppa.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2egjaqudk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xissjlxb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nlgmvyaa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2nakffzvk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2oekqpvew.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gcglgdwr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ejcmimao.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ulgwyavj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2eqyksmqi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lzjaghzg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qqnaqwqq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mnwnxomy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fxmppneh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2qtfthgox.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vqiebzgr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yuekefkg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2knrhqopu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2efsjejdf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2dxbbhpsj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2cejevukt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mmoyryyh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qwuvajvz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2aplhmqho.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2xxryjzht.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ongznxjc.html


<!-- 参考信息 -->