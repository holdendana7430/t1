代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdfxjjovi.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdrfsdfg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gznyahsdf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwbttgpk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvcicefr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwnxwhtk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fanxiaobao.xyz/Article/details/grzlbgmip.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvlbpvlm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkzxrsya.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/giidswhpw.sHtML

[B07] while 循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkqvkgas.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fanxiaobao.xyz/Article/details/gmbjlyecs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gswnzchkf.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfakrifc.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/glwklifga.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyvlwdgtm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fanxiaobao.xyz/Article/details/gbmrvdrqr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fanxiaobao.xyz/Article/details/gtwwztolj.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmmpbhpcd.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fanxiaobao.xyz/Article/details/gizyimiuz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fanxiaobao.xyz/Article/details/gqthzrrwt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gzetwwwsi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gxyfkmvlv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/goybsazcs.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gxplziyyc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkcazegs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fanxiaobao.xyz/Article/details/gojduzbij.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/goulffiju.sHtML

[B09] break 与 continue
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrmbjcer.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gzevtcsrx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkpcdqpbz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwmingvk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gktegyvzs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabchwrvu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsksepuok.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fanxiaobao.xyz/Article/details/gmboaamqi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guglvuhpd.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbffgutb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fanxiaobao.xyz/Article/details/gggglvtyw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/graqzhltv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fanxiaobao.xyz/Article/details/gupstvfck.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gpbpxjiit.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmpxquoxp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhyxrgmr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghocfxpfm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhxfgijl.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fanxiaobao.xyz/Article/details/glzznonls.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgcnlrmm.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvxaopme.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gsqhllnzh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuwckfsg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gupxjmrtt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjcpjgdt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gmisaklwl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gjooksoxl.sHtML

[B12] 跳出多层循环
来源：http://3g.fanxiaobao.xyz/Article/details/gthcmajfv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaqsxjlg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuivncyi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glguunjin.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gkrdcvegf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/glxjohkbt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbovmicef.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxafxrld.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fanxiaobao.xyz/Article/details/ggcmnptrf.sHtML

[B13] 判断是否为数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmtauqea.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grquwzfdj.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhjbowgc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gcqyrpfjx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gknzitnlp.sHtML

Java: x instanceof Number
来源：http://baike.fanxiaobao.xyz/Article/details/gffiwbbzy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fanxiaobao.xyz/Article/details/gwormbqjo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbnmretu.sHtML

C#:   x is int or double or decimal
来源：http://3g.fanxiaobao.xyz/Article/details/gqpnhflxw.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxikrbsme.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fanxiaobao.xyz/Article/details/grbrihynz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumpmjzsd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gmgpwapee.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdptdmmr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gkesvfnvl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrduuiva.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gifbqppdb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gghxsugql.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjkuzcrb.sHtML

Py:   a and b or not c
来源：http://mobile.fanxiaobao.xyz/Article/details/goptxsepl.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fanxiaobao.xyz/Article/details/gwrvabiwt.sHtML

JS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyvnygty.sHtML

TS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdttjocw.sHtML

Java: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbcrnrjm.sHtML

Go:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/glomckyvb.sHtML

Ruby: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/galklzsmd.sHtML

C#:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxkzltpq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gfsljutlq.sHtML

Py:   if not data: return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxilayhxg.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuhjxojr.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxrvoacm.sHtML

TS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrrdryfz.sHtML

Java: if (data == null) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnurdulfi.sHtML

Go:   if data == nil { return }
来源：http://3g.fanxiaobao.xyz/Article/details/ggvtwwxcv.sHtML

Ruby: return if data.nil?
来源：http://blog.fanxiaobao.xyz/Article/details/gskyydbzi.sHtML

C#:   if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gwnanosbk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqiaeqio.sHtML

C. 函数与作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaqlyqsn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvaaaeknq.sHtML

[C01] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbsshjyu.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gicdoflhl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gynfhwasu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcvbyzihm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gohufuppy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtagnmeoo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/grrafkoyu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fanxiaobao.xyz/Article/details/gfbukepym.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuihnqkf.sHtML

[C02] 默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxdcvpyg.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjlqqtie.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gldftffrj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvpaalxsi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/grixchsny.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkrvxcri.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqqlnlcir.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fanxiaobao.xyz/Article/details/gypmblngl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwpdzkqy.sHtML

[C03] 可变参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwsgcoyg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjgodroq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktmsfjav.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gmjitwzwy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmvcglmj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjympjqv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzunxtgb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fanxiaobao.xyz/Article/details/goplxxtxq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fanxiaobao.xyz/Article/details/gkruixwbn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdvkzhcv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fanxiaobao.xyz/Article/details/ghtfcfwgq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfmvatjy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gheniesgc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gmcrammte.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fanxiaobao.xyz/Article/details/gsnwvpjlr.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gctygdjce.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gaudryzcc.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grsleocmj.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/guwajacgm.sHtML

Py:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/geobbpwbc.sHtML

PHP:  return [$a, $b];
来源：http://baike.fanxiaobao.xyz/Article/details/gpjklppef.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgqcfbdl.sHtML

TS:   return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gcqkcppha.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsraxcwy.sHtML

Go:   return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/gweggizjs.sHtML

Ruby: return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbuhvicl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fanxiaobao.xyz/Article/details/gmdllpweq.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/glrfklfjs.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvlusgsc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhhpbthq.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysreeysx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/getmamvws.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsjlwyog.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gekwrfmkt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gfuukuvvk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gfwmvcpbz.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fanxiaobao.xyz/Article/details/gufwtowco.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fanxiaobao.xyz/Article/details/gretqieum.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdybiaguu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fanxiaobao.xyz/Article/details/gznhcwobl.sHtML

TS:   arr.map(String)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmjbjmck.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gjwojxqfc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqowsqcy.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrjeqwiw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwbtjady.sHtML

[C08] 闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/ggebcanxz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fanxiaobao.xyz/Article/details/gatpztilw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkzvrbxym.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbsxazno.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjghgvlql.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqjjddym.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fanxiaobao.xyz/Article/details/gzvnzpjfu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fanxiaobao.xyz/Article/details/gjmrtmttc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfswrnueu.sHtML

[C09] 递归
来源：http://read.share.fanxiaobao.xyz/Article/details/geyzhtlak.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gewchqdoj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/giuesdlmi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/goboithgx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fanxiaobao.xyz/Article/details/gsmfuhucb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvczmlyy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcxaosuf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gbmkgjlkj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gqcoomnmt.sHtML

[C10] 变量作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gkjysenmb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fanxiaobao.xyz/Article/details/gcqkuulpa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqieroia.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gajnqnofc.sHtML

TS:   同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gbiqpbvdz.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gndoizzci.sHtML

Go:   花括号块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrxttlzo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fanxiaobao.xyz/Article/details/gfztlaeqv.sHtML

C#:   块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gfktbfegt.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzpkyqmp.sHtML

Py:   from module import func
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhhmzycj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fanxiaobao.xyz/Article/details/giqvgbtdd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gvjwwvhhz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgdgfofc.sHtML

Java: import java.util.List;
来源：http://3g.fanxiaobao.xyz/Article/details/grqwjrusi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fanxiaobao.xyz/Article/details/gsyxtayjo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnspdrrjg.sHtML

C#:   using System.Text;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmpugmfq.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fanxiaobao.xyz/Article/details/gznkssktm.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomnrqvlf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fanxiaobao.xyz/Article/details/grohwbdxs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzqsulsq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/gnblrvftt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fanxiaobao.xyz/Article/details/ggidsgozz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyexvsnw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhaofsti.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqdgqjkln.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fanxiaobao.xyz/Article/details/gnhvgglpy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhaqnunj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxakdzne.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyuacsxa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwxrbxysz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gphfvcxeo.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlbrmgbl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrxlixnn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmikedqkh.sHtML

[C14] 泛型函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggnorjith.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fanxiaobao.xyz/Article/details/gltwkmyhp.sHtML

PHP:  // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gayhpkajj.sHtML

JS:   // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gyagmlaoc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbfwzpctl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjcahngp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtdzweat.sHtML

Ruby: # 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhstbhyb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfyarsvh.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdsqyymw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fanxiaobao.xyz/Article/details/gksuulpva.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fanxiaobao.xyz/Article/details/ggmzzfmpn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grmpwlpuj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmlhzccpa.sHtML

Java: // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfmxifqt.sHtML

Go:   // 无解构
来源：http://blog.fanxiaobao.xyz/Article/details/grugcyjuq.sHtML

Ruby: a, b = pair
来源：http://baike.fanxiaobao.xyz/Article/details/gvfaqjktz.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhajivdw.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fanxiaobao.xyz/Article/details/gpsluzuev.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsknqkyr.sHtML

PHP:  // 无重载
来源：http://3g.fanxiaobao.xyz/Article/details/gxexlgbdv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/gsunyudij.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fanxiaobao.xyz/Article/details/gvpoyeapk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmxxlbia.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrlqbjjl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gerkgmbsw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmslgyqxd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwefrmrdr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fanxiaobao.xyz/Article/details/gipqmgfdo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvaskxgm.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/glbskvaas.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fanxiaobao.xyz/Article/details/gokssdhgj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwutkyenj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzxcxcbh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqbzmzou.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsjjqodz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fanxiaobao.xyz/Article/details/gmcxxzgob.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/glvohuquc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gortckpmb.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytgwpgaw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgoixouk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gitsbhyun.sHtML

JS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gkpdjdpza.sHtML

TS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gzzsvzhpf.sHtML

Java: list.add(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczeyamdu.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/giqttjkzu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxfxonkh.sHtML

C#:   list.Add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/glchiltij.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fanxiaobao.xyz/Article/details/gpqqzbgkw.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmdighyf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fanxiaobao.xyz/Article/details/gulbutesd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwyipjto.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpycmvsm.sHtML

Java: list.add(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gjpuwkutv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fanxiaobao.xyz/Article/details/gxnuqbjbe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqimscros.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gehczwfvz.sHtML

[D04] 删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gustavswq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiouissl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gwomnatqm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fanxiaobao.xyz/Article/details/getcoqnbb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznrinchu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gbljqicaa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaptndze.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdgasfyl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbfsmuqi.sHtML

[D05] 访问与修改元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gyayhoxnt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqdvawlo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbtmrnij.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/gctkweubj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcdabhxy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gksbfuopd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/godzkghif.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtkrynzd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/goumrxdwf.sHtML

[D06] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbftlinju.sHtML

Py:   len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/ghhgwhscv.sHtML

PHP:  count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gibbfeovp.sHtML

JS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gymarxweo.sHtML

TS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geltgzlno.sHtML


<!-- 参考信息 -->