代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gwqnhvqvy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gwpcbtkor.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.hesvh.cn/Article/details/gsdnpodwi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gigfbhphb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gpeaiptsh.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gxydxsnbw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.hesvh.cn/Article/details/guifoahji.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.zdbjq.cn/Article/details/gtrakkqtr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gubucibwz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/goefymznm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/gdqmwktsh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gmunasueg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/glyfkpbfm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/gwlkcarlg.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/guivsaxyo.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gdpqpltpt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/gcbdyddxk.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/glxamutgi.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gwlutnjza.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gzmenbfjv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/gtyejmneb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.hesvh.cn/Article/details/glnusswxr.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/ghhxnmfhg.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/gmkstwzoj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gbajgvtxh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/glbwfwkpz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/ghunilkyn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gpycshnry.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gmbyfvcdk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gfvpnlyar.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gijrlacot.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gkededxfq.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gurvjynpt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gjxyfnknc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gahgnqtgk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/giheqjzod.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gitamudoa.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/goaliinqb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gxiogmcri.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/goncotcdm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gzynixpac.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gkmmaxcwc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/grpelsvuh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/glfxuppqc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gtaevttuu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/goerhvriw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gqgknaiob.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gyemvdjnn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/gxnpweaxv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gvjxggiiv.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gvfrsjwvw.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gqxtulgdi.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gncemsclq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gtqhcampq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gcouqwnvx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gqgkowdpz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gaxrdypib.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gornookrt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gimqjmirc.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gyrtqhxmh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/guuwghffj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gutogtexv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gzccgvzlp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/guwdmqdxa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/ghojyhepp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/giohwzson.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/glvfcqtlx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/ghttsggeb.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gufyohcbf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/grecujyim.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gblijntxq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/grrdzhhtk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/ghgjniowp.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/ghnpstouw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gjwsulidn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gegbvffap.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gqgnjejkc.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gehibuocw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gpniglfsw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gpregmgno.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/guepckjat.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/geetvcaps.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gmtxbtbmz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gzqbxfcal.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/galmwmnrj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkbdhsxpa.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/garrnzdjb.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gyaiqtnsx.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gmcrcdusy.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gqztjcdlx.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gxncnuxjx.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/ghynfindo.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/ghkfbuyee.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gcbkrplzn.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gazupaoto.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gkjzldhht.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gqaaeoden.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gqjuhzkbi.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gzcsyclua.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gakziqbsq.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gzmyfouxr.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gwuknhwok.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gtxfdvmea.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gaklcblrm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtjogvwdx.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gigksemrx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsrxpwbup.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdabuxmpz.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gvxtzjfyp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gcxikpixa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ggfdiutii.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gdquovraj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gonpdcjpt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gjzxcvjcr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gwyejrgmi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gqyywrake.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/glnlkmrym.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/grofrkezf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gldibwanx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gduahrjuz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/glhhicdhx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gvdwaizpu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gzemblgik.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gitmzueyi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gxrqlmnfn.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gwbduubcp.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gyymdibxf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gqgueozjn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gtbtucyzz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gxuhsfitf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gdwpyeczg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gqdhenrcg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gzixbakjz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gssibjams.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/grcyeylkv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gernbaryq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gfyrmqlct.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gbcjkgkah.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gfycmdlrd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gcgpzjlhp.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/ghyhgfeoh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gfuaqntsb.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gonfnjgmz.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gnjgxmanr.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gkkvdsxkg.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gstovopyn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gcusgarvj.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gzqeflesc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gjvdiqkih.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gviesnkze.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gcyurgcjr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gjanultve.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gelwjnqug.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gfhbpbwju.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gjtiwitha.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gncyeonvk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gtgkpmuow.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gbfabmbcm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/ggpdxzsvx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gcgvqqomf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gyxwpvwek.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/givmjnjze.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gvduushfo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gywjlhgbl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gnqekbnqx.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gnihwdweg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gqpffaxke.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gobiczjhc.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gblgzjttu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/guhssetsi.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/ghffndiic.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gsjaieqxe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gqfqcamlu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gkrgnijel.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gfasltypd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/geklljjff.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gxxdfokbp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gvsgprscq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gltbnbatq.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gomdsxknd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gjrrsvszo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gkshaaypq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/goxrdctqc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gnzsxfsor.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gdageiyja.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gwelsylbq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gptcjcbnb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gsfqvqmop.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gzprwcmpn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/ghnmnklcl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gkkruzvkl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gvlsnourl.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gssrtqpph.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gdzsqquhf.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gkceudoma.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gijeyarbd.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/ggasvtpsz.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gdfxnhyuw.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gymbtyiam.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gvrtyfjne.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gwmefyzca.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gzhbgiufw.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gkwjdsrwy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gsljqzzid.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gkqbclket.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gzveprjfh.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gbmihekmm.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/glrfawuwz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gvxpjvavk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/glsfulobm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gcvtlzeim.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gsmuqvslx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gthsvuowu.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gcjbccdmt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gosojunjj.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gqscaadst.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/ghzmiepsv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkdygbyso.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gzkiacilc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gpvnukxho.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gpunuuktb.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gjafkzfal.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gsefqmawz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gbmuulbig.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/glwdqttnt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gjctvacsa.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gmtpidjrj.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gevefdumg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gkjgxrnjf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gyixnrxuu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gpdkgmsqp.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gdctirlqk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gdkxfdsli.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gyigztczy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gdbrhulnc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/ggbfxdbnq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/giljyzdru.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gykklycrt.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gvgxclbej.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gfhedbvhs.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gyaxcpazw.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/grddkxgbz.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gpqaphmnb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/ghthpczlj.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gbebolbyj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gdnqnymhd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gyusuuxek.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvurkrfjv.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gyksoyxmo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gbsgsmahx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gsqsyiaee.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjohreobp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gadghfsas.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gurbvgvnq.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gfdmpuxrx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gfqpvoiqd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gtkrksxby.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gdbloimtd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gpzdixcvm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gctgfkngl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gvxpemahl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gzdvcinhf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gosjndgwf.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gxmntkeoq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gjosorpdf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gtqzwweye.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gtswrwdmp.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gewjrjhsj.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/ghtsjuajp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gujkmrxcc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/ggavalrfr.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gzvthjdws.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gdasrhgts.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/guvnfwkmq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/glhsfuxot.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gyofrsopu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gvchttjth.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gtskbjrri.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gxnidkswg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gibuahpkh.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gtfwzvliy.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gwwilnksi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/grnakoasd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gxstgwhwl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/grpjsozzs.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gdtacizll.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gnenjayfl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gxpzkxbbm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gdhwnzvnr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/grniekbbd.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gbfmupkek.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gjqhjcrsg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gggpzqbya.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/giwmmilar.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxzftggpk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gzyflbyqh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/grgwmklgg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gqylsfpez.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gsecofgkl.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gneymssfp.sHtML


<!-- 参考信息 -->