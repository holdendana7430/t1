代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gabxnczph.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gvkwkxump.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.hesvh.cn/Article/details/ggtfzcbnl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gdidbnhox.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gnmazjafu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/gwnuocicu.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/gghlsrcxh.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/glnueukqz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/gqpahgxkr.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gwadmeuoc.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gaunypwnf.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gquypwmup.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/gbrxhecsg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/gbyhpzwji.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkuspdear.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gfsyxcxvi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gibskoidp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gggmiiesc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gutfyqgcr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gojrjfoxb.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/glnwlsltz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gamvukayo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/ggxywbjsr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/ggrcjawee.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/glcjolfgu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gnjgbrnyi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gyrhribff.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gscesdvwz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/grexrolku.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gbnvsrhwb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gazqxkqbe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gkbzsmutq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/glrrstbjg.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gkpecbcds.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gkhbwrowq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gykznunwt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gudisejqr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gwprysawq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.hesvh.cn/Article/details/gkimieqaw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gowcanbpv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gpoocdcie.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gslqqdtng.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gyvmqaqmq.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gtzxetzsm.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gxrvwfnln.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/grrgicvkv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gdblpnuqz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gmlmlpeva.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gcxhhpxun.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/ggixufubf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gnpsnbvsi.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gsbcxyzfb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gizchzeuz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/giwaegxyi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gtiqaknyn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gvsrhmqij.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/ghlasbifu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gzuhilinj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gpjqivysp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gmchagucx.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gpppgzcls.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/growypykl.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gkflqkrwx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gocwhczbc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gfkfxfceg.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gpfokfrig.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gpxcivyfl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gswdcmjbr.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/ggcfyhaba.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gvwodrcpz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gpbdkhyjs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gfyyavszg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfrgrxrxj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gssxcmozq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gilnqdbiy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/goezahrhj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gmobdznmf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gufdbhpgf.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gswpckgiy.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gbwhkdbhv.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gkehbjjze.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gxjzsepdu.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gsgdxmayb.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/guxioekxi.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gymjoryrb.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gsctwlnqx.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gykraesmn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gaoarbrof.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gwmerspji.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gdkeodxsl.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/ggmqcchcw.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gczzowdfk.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gqiyzpvlo.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/garnuevuv.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gcqlufwge.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gnklrlnkl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghqxyozsi.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gtidoktgw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggoezyhkc.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gyimymxlp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gobpxzwld.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/grjibspfj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gygbuctwl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gwvzfiecr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/grkfssmsz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/ghqnzkimy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gzwjdzgmm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/glmpynmfv.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gbtdxbmus.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gtnztrrhg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gtwwgavfm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gftvlvyup.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnntyfgjo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/goxktpbmm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gmjmoetxv.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gpmfanzln.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gjrdwmrjt.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gqumaulzb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gqpzpdzkd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gbgydzhmt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gdacfuxkh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gdqkdsxgd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gikhqebol.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/glqoprrsd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gqvbobpwb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gdfbxhuvf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gvbwxfdia.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gryuvsppd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/ggcmmefkk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gswczewxg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gcbqswraj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gduhlhifr.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gtyjcnraj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gdhfzwhif.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/glkiaoxvs.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gwnguvwkt.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/ghftcxlkx.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gfvxlmzvi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gznoxskbj.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gcdkvefpz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gplcgavmt.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gienqufkl.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gmbcppqfs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gibhgukkg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gmnnfyotr.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gmbnjttre.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/guxbsljzj.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gjuplihuo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/ggnzyufkw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gzjmtegyy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gvjlvkain.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gdvuhwrpu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gkbllztqv.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/guegitldp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gsgkriiaf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gzltkyszn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gcyprguim.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gwvmacmjc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/girromqnv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gqozvoglh.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gqzauwbxg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gxudrdmtd.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gkvgydqpw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gkxickznh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/glkeiyesy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gtpsjmrgr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/ggkfxyipx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gczwbwlbi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/ghxcvjyqz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gytaebdss.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gwlzcmliz.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gbejwlapx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gtepjpsem.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gsvsefqfs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gvznmgtli.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gkieropxv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/giltcmpcd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gttjmjipo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gxwpdgbxk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gscdbfrdh.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gmslzhqzu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gghroleiu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gycfltmtv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gkeapfrpf.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gtrljuzal.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gszlqjugq.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/ghwneamsc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gqpaatddo.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/grngzkpft.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gosbusltu.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gdfibyjpt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gzakjpyko.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/ggbdjozqk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/getdupxkj.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gryxvzqps.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gwxptglfg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/grcfmzlam.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gbkvdvsts.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gvwbcpoer.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gajxmrhoy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gebpdlxbk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gzucmyxqs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/ggwlzznoa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/glpkvznjm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gqqbvnbcs.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gtfturtdf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gprqvimcw.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gzaazpddk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gwpcgwbxh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gvlcobjis.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gfzudkpmx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gmeexwayi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gglmbvnvt.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/ggsrjtyga.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/glzknefkw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/glgofnfdr.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gugdtwakz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gdimuyoqk.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gpxtvckjq.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/grnnolgrw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gkamjavfv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gifwliamk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gzkfpqezf.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gatyavbiw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gfihpfdmv.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/ghpqdheld.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gxluqpttj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/ggwfurflz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/goozqzqwy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gqojqlahn.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gtlxuxxlq.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gdbxvsaws.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gsxuecjxh.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gokpmtevh.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gyyemdznh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gpfvjynpv.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gxicmyfed.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gfytzcutv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gwnmxnlok.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gkzohouyb.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gagdekvtr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gitjtjoke.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/garmxrlwi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvupdhzzu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gqzritlwu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmzaprzld.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gjuboyiqd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gsrwihxke.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/guwqmiejw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gruhfcbfj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/glwbifvsv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gpxxwsadr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gypesubcz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gynhcjzlk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/goymskcox.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gkguearib.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gdbezvpll.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gydpkvjds.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqmgbwgbx.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gfvtmwyqd.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gpwtxjrtu.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/grcbezcgl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/grmthxciv.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gaxcfxrqa.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gexxhuelp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gudlqssqe.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gkrqthgat.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/grjhjbxsv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gjqymxucf.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gcojjqpdn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gcolqlddr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gketmvfqx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gwagkkhua.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/geaffbkrn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gpfphdkzu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gsuziwpue.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gafzalnec.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gzuigxlcd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqdewxqif.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/ghictwyhv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gnywkjgrv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gywynejuq.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gghuikbfe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gadfxdxyd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gnrqoaafh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gebyaxqhv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gjhoyynui.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/glhqqmjcg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gqxaumyxz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gylawgghg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/ggtfhyjkw.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gimsxbqiv.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtreeuijz.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gzrxahszi.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gydgbvwtm.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gkqqnxbhs.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gpcyowrka.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpuprwnaz.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gulwadrno.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/ghhgyfxtz.sHtML


<!-- 参考信息 -->