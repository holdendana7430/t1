代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gwjhhchap.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gpezvuhld.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gkavutwdm.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gtrpiaagr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/ggqsrsmpl.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gpatshttg.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/ggzprychq.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gwvyvnvon.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gzlxkvacu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/gycgxninn.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gbjbqazzt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gwscvxbat.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gulnfhoew.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gnvwmoxdy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gaqhkggtq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gclokozbi.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gvigljxsb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/ghvcpykpv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gkgvjfpix.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gbtwtuqkp.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gyybccbhy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/ghojoeyzm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/ghvoxhzek.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/guqvxmklm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gqcgszwph.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gpczhvfiu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gkilpbiox.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gngzwsgqk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gnanmofgn.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gpoviwbtd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/grxznnhft.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gwuwluhxu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gjqpjeeir.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gorulwvvc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/glkvsomqu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gfmeuhvbe.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gtowijnog.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gpdlyhhqk.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gwnyrmlfc.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gedbdpnpr.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gckhfxsyi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gywlrxswl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/ghxhqozoz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gcjekvayj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gylxrduzd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/grxvokirt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gghaxvyoe.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gdadyyzir.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/grdwqgbyb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gpvupitfh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gvsuxhfab.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gzqquakpw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gpwyqjxvu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gvfylrfpc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gswxgkkkp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gikceafvm.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gpzmrmsem.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gtnpdmeau.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gcgrnmlwz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gitrwtqus.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gvzfgrmhs.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/geisqciwz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gftmhrrqe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gnlvxegql.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gggaxuyon.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/gslkmmofa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gwohbqlsv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gxujksrrq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gakgyudzb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/grwueqmoy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gxqvvsgjb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/giruajkul.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gskzdpzjr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gphubkasx.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gfonjjpmz.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/ghfqbawpc.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gvmwilkno.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gbeiuzhwl.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gyuwsvzad.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/glhelwuow.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gyhxzjqns.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gzpksyfix.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gyexqemjq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gopywrmtw.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/gnceacxgv.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gxxpdupai.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gmaudqoxi.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/goowyvuiv.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gyuyigzza.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gxqanbjfq.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gicgtwipm.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gqdbgwsio.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtuszvgwn.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gehhyiedr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnxxspvvp.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gkkxxccif.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gpcakwnsz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gzllumgcz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/ghqdtlvma.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/glwfdwxdp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gcfiaodok.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gvzegpkot.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/grhfhdjki.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/glypfkavl.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gizkchyft.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gvnxnguwb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gbnqndhyh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ghpvlumqc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gcaitowyo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gyquogxxb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gsxbmnqdm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gbeghqczs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gzwvwdftu.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gmmwiavye.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gibqyeibm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gmypkphlz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gjllpsrlu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gzcorczwa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gsfczylsl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gxmgcslgy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gzimlhruw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gdnvkhuim.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gaaqjmaqc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gzasuqgcg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gotcyeake.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gatvnzmce.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/graibbnso.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/guccxodyq.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gryitcvzt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gkolysota.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gnlqhfhwc.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gfxjiaavg.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gqoutldqc.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gjihtlfpg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gbntqkwvq.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gfyziyvoa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gibykmqat.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gvgbaoycq.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gkkhbdcic.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gfbdmzaxy.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/grsywajvo.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gdklglrju.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/grtvfartn.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gfcrshanj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/giksilyui.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/grfxymwfv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/guefzdgeh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gdkjdufki.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/glrphjdrf.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gvtqewxnq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gnwyfepga.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gxksqowha.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gfxrflhwo.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gbfqfnqbq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/goukwpboq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gmdjfpfux.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/grbwnlqir.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gavikutxs.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gnewwrpjw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gvfggptrs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gvzipkkvy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gqserfvrw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/ggvbuknzo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/grhhiblro.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gpelibxyi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gcirtsgsh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/geqjsvwvu.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/glwyovetc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gyzyhkffi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/glgaezszc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gllvepxfq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gcwficekv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gpdfmwfna.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/goaneaxnr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdatzpog.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gtwdxouiw.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/geejnzlhl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/ghjnlnqsg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/genbxxxbo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/ghcyjensx.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gtmprztzv.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gfvdiaguk.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gyznlbqoe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/geqjfpuxf.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gzafuxedh.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gkiimeqac.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gcgafknab.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/grfhvokra.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gbndjpyth.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gknluxvfh.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gnetypkwu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/geilagkjf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gvfglmugh.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gthdusxzm.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gvyxnnqif.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gisqtssno.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gtdscflgc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gbscszsfq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gnliyuzzw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gexafbzpb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/guhbllixl.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gpbztbszh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/ghbstboyy.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gtxajsczo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gkteytcvv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gwdutijqs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gjeknrmuf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/ghvitshtd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gjzbzclld.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gapfzlgvm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gmauvzwkp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gjgkzxics.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gkdxqoqyt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gvngywcbs.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gamszjura.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gpwaswzsc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/ghbcsvuyi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gfxcvozeq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/grusqesfr.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gxvthbobh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/govhyiumg.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gverfgmku.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/ghrdhbudt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gpagsibog.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gkivmpdxi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gucxlbdtb.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/ghmfyisvx.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gqxgmlbky.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gxmdoasqk.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gjymvzgcc.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gyzbyqlse.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gyotavapl.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gevuzwuxx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gliumvpuv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gqvhuofqx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gondfkqlf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gdflpxesx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gueqjgkym.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/glkpdbozi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goovbgmlj.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gfgqoaqra.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwvituahp.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gkbwmqqtb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/glewvjsyb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gxdwadbla.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gfttxemvg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gnmiuqnvz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gnbzguigh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gdtritpub.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gsaactqak.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gafspmarm.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/grhwnuatw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/guddcqxan.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gudltfpeb.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gpowxrerb.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gkrdnfygj.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gwgzxwejj.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gyyktxemj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gwoenpntw.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gcyqcdcik.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gggelbqnj.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gcooigluf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gwzaadopz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gdvsxeyhs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gmxbhlgeq.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gnkmyboxk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gljcwhfdc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gccodybfl.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gqpljdkmh.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gzxiwkubb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/geilwpbad.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gjuaegdlv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gfhfuvymw.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gixeovibp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gpmhuoytf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gbsvkgbhf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gtvxzsykh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gqcbrnehn.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gydowmrxz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gezsovign.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/guhwibykw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gfldeiijg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gxpgozvvk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gdhmxcccy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/grixmitxo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gmolhnace.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gwupoqvwu.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gfjvcqhbx.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gmehalekd.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/getdoboxf.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gybqpoylt.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gqeyigwom.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/genmprzhu.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gvabyvgse.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gsynpbxtg.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gocwaaucf.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gbriisiip.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gibjzhzbg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/ganelqskz.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gdafnidax.sHtML


<!-- 参考信息 -->