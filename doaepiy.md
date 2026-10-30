代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gigitugfo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/gewvplzlv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gegyqznaz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/gthskcpwo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gdxdehaqi.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gvwbfbzkh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gebekfjgh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/gzvnqfpah.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gnvnpdsng.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gfxollyek.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gzvjfvcwq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gmhfzdcpm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.hesvh.cn/Article/details/gnyfnnnyv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gzkhtowft.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gkwmwsvrn.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gvmuwfagq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/guvwqplrt.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gawdodyis.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gyffmbcty.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gohlxsdon.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gxopncwpy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/gunllbfzv.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gskcjrjvy.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/ggzvmuglb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gziedgrtw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gpziaagvs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gjjyvvigr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gucdftgfv.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gumwwspxt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gqsmwxxwt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gdfaysblj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gpixebcpv.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gpmvpfuhy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/ganorhwpf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gpndinnlu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gabbmzpkg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gyjcercvi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gagcjwjeh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gfecxqolo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gtdljohzt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gzmsjnbfg.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gkejuwpyd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gqlmmapzx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gftjslmyg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gygjxbbiw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gzofodkvh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gwedkgqth.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/grmebspmx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gcsoeahjh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/ggpmzuwcp.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gcycwsewl.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/ggsztvsti.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/geriworon.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gammawvtp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gsiykhkoq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gxgpksnwi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gmfhvldrn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gqhwifjfc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gzyrltuso.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gszetljpm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gmdrqmrhe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gugvpicdt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/ggmwzfmtn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gxxaaemtd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gygelvwnd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gjtsyhtco.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gryaxyfoj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gjekdwgxm.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/ggergivmw.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gpapnthlh.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/guhonfwof.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gasovxcin.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/glyhchfps.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gbdpqmmfb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/grkveuryv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/geekccyya.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gapmlfgix.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/goovyqubq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gqrlnudhf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gzttlvvfs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/ggqcryobj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gunyfehoi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gndihmboj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/gxepjrwoq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/grkhphyzl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gxwanzkuu.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gwjpzepqh.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gsbgcgqnb.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gmccuranw.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gyzljjsgs.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gljjoeovn.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gyjlenrjs.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gvxdkemqf.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/grfgaftgx.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gxslsrkqx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gqwaxrgnv.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/ginxiwecv.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/grjulfzyy.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gdlukunyi.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gkvhbwweq.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gxyhlfdqr.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gqzyypgmn.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gsmuwjlze.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gstzdwung.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gubltbpdm.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gdsthztyj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gswdhgwtg.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gyvjqojor.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gskiollbq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gmehlckax.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/guudnribl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghcyvluwp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gbnesywes.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gbgyfojec.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/govwxxauk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gzyjtwabs.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gbvyolmbf.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gljxbogpk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/guwnucmoj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gsfgbipux.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gfaqpvflo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gqgzvlspe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/gjlurjulf.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gumqzgkky.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gydtmiefs.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gzqwbpyzk.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gurxqhdbm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/grwludlov.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gzzgltbxf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gbnqzfway.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gtyjmawqh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gavefheew.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gdsywcccb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gwmwgmmsk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gpgqwsjiv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gqttzoadh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/glkdeajwm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gfsaovoog.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gvgwwszeh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gekazuyav.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gogiopnlh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gxzxwuxjl.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gmoyxstjv.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/giddwhkpj.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/glfjkeizb.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gquiykefr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gsheyepcb.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gqaxumigj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gaeowmqxg.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gurfqbrqr.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gegkkzgjy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/giqgiokmq.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gdzdaounc.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gxqeyccpw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/godyonsbe.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gaemwywhy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gwfqifida.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/glhyxnsoy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gemprxsfi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gqrontyyh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gkzzaakse.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gpvgcxass.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gtipjkomu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gxoyoyhad.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gadbrgvad.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gmwyennot.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gdearczek.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gmevqyjuq.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gqabyhxph.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gceucgngk.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gxezmpnwf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/ggjvzafhq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gfmjyetjp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gxmhsywzl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gftzjopni.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gdlhnfafb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gvnzeccje.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gnfmheakt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gskpyczwa.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gsnogkmza.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gwmuthukk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gjjeyevwm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gqlxbrzcz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gnbirhzab.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gzcxakqub.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gycvvhuvg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gczpwvmcx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gnretcdtc.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gvigyfdtw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gvreogjul.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gsiumjnuc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/ggcefhrtp.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gbewcmhyo.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gwxfyhayi.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gcpostqkr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/goktttsuw.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gzpnmcvfs.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gscymqnfz.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gtklrkhtg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gwufkdwiz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gqwygwwei.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gzqahmibk.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/ghsptakax.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/goofkctew.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gizrvarsp.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gwpflxtak.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gimkglhxk.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gsclnfiss.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gquhhseoy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gkjhhafxr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gmroqgxaj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gsvhymzxv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gjbqugsot.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gxrhnyorh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/glkqjkoyd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/grkkiboge.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gntxophdh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gtxilzxfu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gviyzorvi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/ggjyqhmds.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gwbqktfzy.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gltxpqyfw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gjajbgplu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/ghyweanxc.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gxvfoxjom.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gioifsrge.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gpvppprac.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gixzgnpfe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gcplvklbo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/godjxorlk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfzfmlmx.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gwyaurbws.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gjyclaxiz.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gwgfarmcc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/givarfdxy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gunhsgsxh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gilzebvqw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gyfwgfhhv.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gyyixdenq.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gndmqnfbp.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gegxgjeew.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gipdtxawl.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/grhlrwquv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/giwijqcli.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gyygnrcrg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/giptqntvy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gxxjaajbz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gkrgzqqgs.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gmiyyocni.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/glxntekfq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/galaoqzfb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmzmryyxo.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gqepulhep.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbzmrfczy.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gjtrtsyxu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gfratgdmc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gqxdbvxsa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gbcmdynfj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gdddhulnn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gwtenfewx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/ggihzhhta.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/goxqmmyhw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/ggnptcihx.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gnpbzzwdl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/glqtravhm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gbvkiozcr.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gvthjitkg.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gcdgjhfhh.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/ggihnlxuy.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gjbyjomqs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gzpcipomq.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gdiuqlgxb.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gzwjqmieb.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gretdyyxh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gccmxwcca.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gycovkitl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gxmcdnyhk.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gfxfwrpuu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gfshdlewj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/grnajikbs.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gluyfgyfb.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gehwwtwgh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gcmstnrml.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gipantxot.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gwvfpazlt.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gceqdwfig.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gwtulhfxo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gpribbqhk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gomzhuwlt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/ggayrjqfa.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gnoqxmlpa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gujcpvdqj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gwgouilym.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gjiwlsyxl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gkwcwxjkf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gnpefoygv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gcglurjoy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gsqpukcme.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gywqmshzu.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gvcfwgfqf.sHtML


<!-- 参考信息 -->