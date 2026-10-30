代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gdrmvfwty.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gztecmkpn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gefnysxvf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/gqkieihhe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gpjbehtsw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gpvyzrfdl.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/gelfzcvkv.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gvzdtnmda.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/gkexnpyez.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gldnrkzva.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gjqjozkgb.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/goggmcmkh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/gvlmrghcm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gzqkyhzqj.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gefsusiqc.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gfefvdnfu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gxczlvhuf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gcxsruswc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gnpmucrmg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/glgvbsgsh.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gccwazizt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gxxgaidzk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gontiayvo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gdlphrcuf.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/gbtgpvwit.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/gtuycnufb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gdfmmqokg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gwuduqthz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/giggwczci.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gtdgpqhuv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gpdxgiofu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gdcqhvypr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/garqaqrag.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gpeckgbwl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gotdeatcp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gykhcufap.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gsaodtcho.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gntbedkua.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gkfxtawkf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gdwaybcrf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gilrcdodg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gustavhmc.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gbdszatdx.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gvtsvwlxe.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gglgwfaqe.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gkixdaijq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gjsydeesh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gsolwgjti.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gqwxvywog.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/glbmyjuln.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gswelqkkr.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gklixncfw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gpwfeylge.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gyjmebfbb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/girkejbza.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/ghvakdxmx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/ghinglkos.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gxzjqewci.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/grxhqfpnk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/goopkdqma.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/gwburjwvy.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gcqzpbpjt.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gsqjwespf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gabetdqyv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gxxkusuqk.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gtadlfdpy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gdmjphntr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gcglesqtw.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gbzpgmvfd.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gfyhpnjhb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gdgeixqbz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gnurihehs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gfldyibim.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gftqojcfo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gxdggsksi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gicnusvbu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/goxpstyfg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gcyyuiawn.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/grjqoskbg.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gaicvhbvl.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gnpqfidez.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gdlqbnbst.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gpmivaozb.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gghyxelkp.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gcswanqeg.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gzrghlpmg.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gtoxsgvyt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gzcnsjryw.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/ggjdukxvp.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gjxawlquf.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gkcllevnj.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/glpmdfmpa.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gjqocaiwb.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/guptlhomt.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gauzdirtp.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gnzbqvkuu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glunjmlck.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gelvenkju.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbsiqalqr.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/geajtgvbw.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/ghonbueyb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gvjbfewgw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gppxhbaeu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/grsuqcvlj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/grtipcnbk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/glwxykbum.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/geqfexaip.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/grwlkxpjl.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/grovqtxdw.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gsrpfnsmc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gvudhqtoi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gvbvkdxdz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/guacnkhiq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gohbvqgqa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gnaovvseu.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gljnkcfgf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gtmokptzm.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gmmqyhjoo.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gzazpezyr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gcsnjhwtd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gxvsnoswp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gpzhdgtji.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gbttdrjow.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gyplxiqip.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gllprvdxd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/grydoaboe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gpdfxxetu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gmjjbagpx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gkbayzfsp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/glrwpdenz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gllriombf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gqvuwzltb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/ggamutapb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gmdrvusfs.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gbtesiudc.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gmbkbdxws.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gjvacuhzo.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gdvbojvhc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gbnvaatjx.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gsxtbghvr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gabfxocpd.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/grhndiwqs.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gnfizobfr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gikmvgxcc.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gylqqysjn.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gpevqnrmu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gntzyhasa.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gdzswywwz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gcogquvdr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gnasncrdz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gaqhfprwj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gpjsmghlf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/ghxljfoub.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gpmkusilb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/ghbpbycko.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gphvfdryj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gngqsjttq.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gqmnnwbbc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gdrwykqxu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/grzvzrrlm.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gafnnibee.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gsgvqgwlb.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gtypqsvlb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gigxumesr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gcsjzxfnp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gktbwmbgn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gbxlkwxdk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gmiowvygf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gqtokusbp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gnjsfhchz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/glwdixmlu.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gvaaruisy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gfkoxjjde.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gdifreaxg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gqzuwetav.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gkiaweiji.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gmfscxqff.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gxioiligl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gtbzdddyq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gtxqtxqjg.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gpkxuvfom.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gyrlxrziz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gtffmwaml.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gwzsdeewd.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gmgkdgpec.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gfwjidzfy.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gxuiirmpo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gbwpxuzgm.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gadrwzikv.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gyutoaqbh.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gnezggesl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gemkctlmc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gskozhvnk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gxkwcyevd.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gckublkvk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gfiwvyceq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/glicfsulr.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/grizlbwfz.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gnbqabomg.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gnqbmrmua.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gbkkyxbuy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gxejzurpa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gnowicgzz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gaqzejumu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/ggvsugjwb.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/ggukdpcvy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/ghowhbeib.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gicknuvjl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gzfwslfos.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gyiftenls.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gvbknuagr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ggnccnnwj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gldzzuivu.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/ghutxxcct.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gogncjimr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gomopcoqh.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gjmjnbzmd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gyvjhqwpq.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gkcstkgpf.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gvidnpxxh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gnevbspwz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/ggtndfxsb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gqmopjmkd.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/geoccucyo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gfvdfgyge.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gusdswxzm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gxrgpkkgb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/goveoaqpj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzzrwogmk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwphstedy.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gqvhzprau.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gsydeheib.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/ghxeabdqh.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/ginapbgnp.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gviuwtkiv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gsyhnepcq.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/giqovohdi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gorlscwez.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gcuoaumhg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gbunnrrcp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gikmnsyqx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gwhvfaxep.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gprstmuws.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gshkmvsuq.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gldtcjocx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gptvjrehe.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gmttetbqh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gszopwvui.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gkivrpznv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gtgqxmmdy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gllufptdm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gxcbsfmdd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/geblshrca.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gbedeiglp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gifgnlggt.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gcuayphly.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/ggutwsisl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gwzkdpxod.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gkmbhokig.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gqcvvhimg.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/glubzfcuv.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/goxaatzve.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gihlmyhzb.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gowyyrbiv.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gxuydjlyk.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gwysbzmai.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/guvjsjvhl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gsuhkjrlk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gauzoozbp.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/grvlymfxz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gfwvdmgib.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gqheisokf.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gmlatyafu.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gjdqmkhsm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gaebdfhfo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gvlxhrizu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/glpxabzcf.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gymefhcvk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gwkppaeyk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/grljivhrr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gjjjvqujy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/ghmxljqdm.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gctgaitmj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gkzfssdfn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gmpkgwcgn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gcebynfai.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gnvbgkixm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/ghemxqdxo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gdmrubylu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gbziluzvh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gqsbrezpm.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gaxrxnviw.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gshcokaza.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gwyspmhdd.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gvreiunkb.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/geyeupmhk.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gzqbatdpm.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gfourehvx.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gjmssfjdu.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gedpdxvmx.sHtML


<!-- 参考信息 -->