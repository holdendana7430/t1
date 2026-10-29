代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gefvubgsp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gxwwgddwg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/gxnbuduvn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fehbvm.com/Article/details/gctdgwixs.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gdendkcih.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fehbvm.com/Article/details/giqgxpqcx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/gndxdgzed.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gnoowhxhn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/giuqtmekq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fehbvm.com/Article/details/gncujoejf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gmywnpicc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fehbvm.com/Article/details/grxvnhrlq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gffqyvyem.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gchwgfnpe.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/giztlxgel.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/gxfezlhpa.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gyircrdtq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gquqjouen.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gjjbyhkav.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gszffqeow.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gkihnhjgl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gelchkrrz.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gratllqvs.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/ggqigmbdk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.zdbjq.cn/Article/details/giymcbauj.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gkfuddnzm.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gvcroyvto.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gvafkdnbj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gebdlidpp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gpvikwqot.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gpprqpjbu.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/godioappj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/gsmyyimef.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gxuadbghr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gjydqlnbr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gygylujpt.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gzjwpivmx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gjmuwzyhr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/grggfywdf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gpzfyizju.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gpndaqqaq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/gugqmkckg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/groapsykp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/ghfhvgbtx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gpmznqarp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gctqiskna.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/gwisedppp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gsmiaijog.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gijgramev.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gnkcpocep.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gdbusofyq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/gpljgozts.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/guzhxmqck.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gawwcdiit.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gtfmrqqhp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/grezolpqi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gprejwxnf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/ggtaqmmtn.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gatrxxunp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gvawtxith.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gtnideply.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gjzfxacwt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/giyceycxj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gmdfarmgb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/gboiirufa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gpjhlcjpi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gvtilpnmw.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/garxiljay.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/giilekrdl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gmhrkwpmr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gtvzlcnep.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/grqppvsft.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gykqlkhlf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gqemhzjit.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gacxxoiwj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gdudkfvup.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gjxbluebp.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gxenqvfnm.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gzunxmhaf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gldiftgvo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gxtdonxio.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gstkzdyjv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gcrauysps.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gntotglhl.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gvitpzvud.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gdykdehdq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/geeqfintm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gntriobnr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gdxluvdrs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gyivpbduz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/ggvoogcni.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/goytcetrc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gslkpveaj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gujhknvdp.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gsejqueux.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gqoqdjmyi.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gybvivohx.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gcvwzjaxh.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gckdaqhsz.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gjizpvbbb.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gyfmzicki.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gmdgxtias.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gmobqpjiq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gtjxmrkmp.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gadpgrxjh.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gmobekdyi.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gxwvixzkx.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gbkbtbfeu.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gykwcniay.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gscybshlh.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gfmppnuve.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gonkmtwwr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdbzjvugg.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gobqudktd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggkgowozt.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gghnxqqun.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/guxklxyxi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gxesefoia.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gjkbtlxdl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gjugrgkbl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gaxchtqtu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/goxbjhlxb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/goyhkrcne.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gzbzdeadu.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gzcmdedeg.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gcjljtyjl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gtqbpzsha.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gbbqikayb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gjefpqsei.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/geawfgobv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gjbtyrvyc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gaacaxsab.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gfwulgfyk.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gihtrljzk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gscuuyvgf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/glcsuomwo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/giledwlci.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/ghphoidts.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gdvgpknfp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gjnafbjts.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gtonzppvl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/ggbdmzkfp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gxxpmbspe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gcpzqswkw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gmgzhuobh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gofpkvrdw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gvgjxqwjs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gqjzocdwq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/geydrudnh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gcqoymesj.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gdcqriohf.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gjpyzmysz.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gayddkbeo.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gkvyjwoaq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/ghomylnce.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gplhsyyet.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gnrwmoypp.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gsoejadfc.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gdmucyehn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gogorllwu.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gxqprjweb.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gjfudldeg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/goznndriw.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gvfsyuetv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gbcrbgrxv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gjluonuyp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gogeerbbs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gsublgkhk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gxgogudnj.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gobcyfljy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gybkwkrdn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gxkhqgheg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/ghkfaeokr.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/ginonvxbf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ggfufelkv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gwssutsan.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gbmeoiowe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gisarnvoi.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/glyflekkf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/guwvvqjgc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gwwzzjrrh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gcemlviwc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gffxjvwgt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gjdtoqzmf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/ggwmxwxrf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gknnqiqgp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gdyaenyrx.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/ggxrrzida.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gkqudycen.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gvqcohfli.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gvwawqaho.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gtzzbucpl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gizpnggkp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/ggtaetekv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gwyjfdlvm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gpbxbehdk.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gvsotzafl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gilwcmapq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gylrfvjoy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gjlfwuxbx.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gbtivqyjw.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gaoyelueg.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/ggcuxbxci.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gkfooxxeu.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gsvorofky.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gpednlknw.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gsnakdqmi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/grxyidmyp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gsvqlkuat.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gaowgkctx.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/glwhicyix.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gjzdouyii.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gqdbenrkr.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/ggcnryynb.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gcmvzznno.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gxcaurvaq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gktcoacez.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gmpgwlqqi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/ghutmtfmb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gnsruyqyu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/guchdkgal.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gjkuzckac.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gofmipsyn.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gazfgqvxv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gtrxmujhk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/glabadwyi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gxubjlgzt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gwgepjhtw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gxklqkeje.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/grkepywqu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gcrthhvli.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gdfwvfkxf.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gwfanesoy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gwninpifs.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gxapmcseu.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gxrnvdiau.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/grqbjlzzo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gifneltzx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gttfpmcuj.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gtqjcnsrc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gpfeuypjn.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gdluwuefo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gcfxlnile.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gtepuckwe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gzhnimbqz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gofdjtrth.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gnmjckcvb.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gcsnsovog.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gjupgfsrw.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gtqokmznl.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gpzqqafcd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gouxxiqsi.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gmdznlybh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gtfevwhbz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gxvjwmpxd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/grntgqlbb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gohznpmyi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gbnixjrex.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gfrisnvuo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gznnxfygb.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/ggdefummd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtjaotvbd.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gtngfwysa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gptphqenk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gvzoambay.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gjxvohiqw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gjxcmynnu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gkwlopujd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gujzdsark.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gfylegpqv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/ggksongat.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gyrfefazt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gwnwmiees.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gqlccxeww.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gbohhngpa.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gvafzouci.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gqfueixip.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtxawbax.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gftzepfpr.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gkzehmkcv.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gmptbcryo.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gquuizlbs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gsinnjgjz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gmwgshnhb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/ghqwjjtwu.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gwcqloivj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gonlbgeub.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/godcotxwf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/grrsbhkha.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gktdmjpho.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gifejzirt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gbjeithek.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gdwtvrdny.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gwkahqagx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gxrniueir.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gnfyqttvs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gbfpjnxaq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gtayhbxhv.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gtemvnxue.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gnwjodkcl.sHtML


<!-- 参考信息 -->