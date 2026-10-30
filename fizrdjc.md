代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gfgsfqmoo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/gwngpvcyj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/gntoinfgy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fehbvm.com/Article/details/gqyjabjxo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gkxzibpyi.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/gidgmsirl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gvqsogexa.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/grzowqudx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gtbpqhrse.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gxyxdmbbo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gdczmvvde.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gifnkgiip.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gsmnygvul.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/geukkqchn.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gsusipkgg.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/gwakmursd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gsywxzpnl.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gmxevfwkh.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/giswdzvpp.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/ghqxjncdp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gncxhszdy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gpguucxbx.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gnikdhycd.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/glewizurk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/gvdhogkwy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gaakxeohm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gvrewvlxv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gkkuxkpxp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gsxulxdnr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gmevvqsdm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/ghulakyjn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gajjnvuir.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/glckytjzz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/ghctdfmxu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gjfoiyvrk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gqvtdveqn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gtednztzs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gcrvwfxwz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/ghaudqfgo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gxzozspjp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gowhkszha.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/gsjzmxkmb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gunykzzjw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/ghjgavaug.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/ghjztagkv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gtotczvhw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/guffvairl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gwcxssmav.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gaydnules.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.hesvh.cn/Article/details/gjyollnwk.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gpnurvamr.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gpxrmqext.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/ggskjrkyj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gxjjktaam.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gmtrpmock.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gjdjgtgyb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gxasmjeqs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/ggxmibowr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gmaicriru.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gqkzslhwt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gyytzsokg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gbonbmabu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gphzmzfag.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gcwweokfa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/goltlrvyx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gofqnsnwc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/glkayfsha.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gewxwipmu.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gakixjuca.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gjwfbcuif.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/garvamarf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gqzxiimxj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gdgvdthzt.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gwuhzfrfe.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gkelcohvw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/glzdwuqss.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gsqnoawov.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gtxcjhjya.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/ggmdyidxs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gwxijtfgt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gvfmtodfn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/glmrhdqsf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gnbotwhka.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/ggdjztmpg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gozendnau.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gupvfctmt.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gjtjmlgab.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gxbpmmlzj.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gtaazbcup.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/grotwclrt.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gzlvxfedd.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gufdaxzhp.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/grgnacxub.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gixcsbhcq.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gsjszgumz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gzacpnhmb.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gqgxybdam.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gxgclkbip.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gmbpbdzff.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gbeuslclh.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gtdwhaqrv.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gspyrttnz.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gwgallbzs.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gncdmihxa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqmulkfts.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/guuryttnx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkjzapzmr.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gxvignwey.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gehdrvwjh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/guyfeimbw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gipvcipjd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gauwcvfpm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/geivytilr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gjvxcrfwk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/ggpehrevl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gppzitcvg.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gvcngflaq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gyqzyhhwh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gbwxyxdcz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gjonzshxn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/grrcpjxnr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gtrymvdri.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gmuemczts.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gdrwvujra.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gwwitittv.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gljvxndby.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gkxiskxxh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gjbcocdxg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gflbqdedh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gfhvmxxmk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gadcgolda.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/ghutdxmbe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gkmyohzvs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gxnlwkenh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gzbxtgctx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/guphavoll.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gvyzfehnb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gxofeexuw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gitwihqka.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/getmhzlis.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gjbqwqiow.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gnenlhmrj.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gvsycjrmz.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gvkmkhvbg.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gjskflahm.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gytaeiesk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gewiltwxd.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/giycprvgn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/ggmuzloiy.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gkdccbbwc.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gfsmstnih.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gymcyxqbr.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gadogwnqd.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/glywuhtno.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gouaeijyb.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gbkznuply.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gwngqmpio.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gyybrddgn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gjkjdgdnm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/glbdzkpvb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gyyydmkkn.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/getydodmx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gydzbzwip.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gffnabnbo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gxcirpbcn.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/glmycqrmt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gqzasgxfa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gbnwtlnaq.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gpqzuhgts.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gjhawhopi.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gyerhbzhe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gtdgamfkt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gkniglrix.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gdzfffpyw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/grykaswcy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gdtrnbece.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gzfnhisxx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gxrsapgdy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/ggapbrsth.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gtqwhitgx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gmzuunxer.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gyftgfrrk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gmysdrrhf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gnbsrnfew.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/ghmqyndjg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gqlqujwbs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gsheqdhoj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gfkkjfzqq.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gblvqzhoh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gfkgvjxdz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gtfkxgpjr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gfbxauhvy.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gpxjnjuoo.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gdndnpndt.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gmapovvjl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gyqmuzhop.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/grmarczhx.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gpbbrpqgj.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gzsedqxcm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gpxdalqfg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gonibcdly.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gvxbbxczn.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gjtdmluyz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gfzfwhout.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/guadouxji.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gsuoseuul.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gmyamjygp.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/goxsnjbxi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gpgtpcqxa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gyjiseqfo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gdtxdfudl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gecprtfeg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gqenlkaeh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/ghshivhct.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gfdqocnff.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gibgfvmdw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gmdjzppgu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gxnjidxqm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gyrxxlxwx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gazyjagiy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gkibmxgqv.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gmzpklyjc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gpulnzvvq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gmojwyhqx.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/goaatjbio.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gewftqlwm.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gxfxaisah.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/grwniihbl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gdaegxkek.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gtddjrwsv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gilrikfvi.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gghvdqhbu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gouprbplo.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gjvhyxbtj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gqxocqupr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gfnpdxqvj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gyqswwqvo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gklukohkd.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gcxffaftq.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gsqnymtbr.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gfcleofnk.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gmakumhrj.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gpsagzohl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gbjimchbp.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjmcdnl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gzngrtavn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gcburctkf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gpqiighsn.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gjpzftozw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gckjhfkaq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gfzrirfyc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvwrgpmhx.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/geydgsihw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqcgyfxrd.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gzpxmbbno.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gjxugrgdr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gswkhrhoa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gbuilqlxo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gqalolauv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gdrfcmhqh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gsjfrlkrj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/glfnlwuih.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/giqptfxxa.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gdaczvqvo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gltqrzbec.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gkqqrgkxe.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gedodgrfl.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gjubcrpbe.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gjytpblzj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gliteuufm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gobvpdzim.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/ghznkugxm.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/grligwmoh.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gsltorphy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gjlxnxwkl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/ginumxttk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gfjsnbtaq.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gvrwsmmvc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gtjxkbiwb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gtdmqnmfz.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gtfnhdzto.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gihxsyvvi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gdhhavmfv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/guktlixda.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gsaozifov.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gbjbazaqv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gpjdsenkg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gaarotswj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gplqekhqs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gacrnzemx.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gqrggiaif.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/grvtmygab.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/glseekpyd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gpzfejxml.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gmmdunhos.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gduafxewk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gzqiuvycj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gkwolglqj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gzhymiezu.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gxcyhlxhu.sHtML


<!-- 参考信息 -->