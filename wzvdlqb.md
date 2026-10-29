代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/ghoogacle.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gltnqrjos.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/ggmjugxjk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/gnooyvblu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtlgkngc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/geretsdjl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnrfneffk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/gdzpqsxxh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/ghhzfotzy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/girojspdt.sHtML

[B07] while 循环
来源：http://wap.fehbvm.com/Article/details/gofgylgqn.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fehbvm.com/Article/details/gnipwkzyl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gwnegxuzs.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/ggcxnsalh.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gvvmyzmdw.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gsjdifbig.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gxbkxyuyi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/ggcsyfqza.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/ggduydywl.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gpkchzvre.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gfgpwrrmv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gjoviujse.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/ghodolfho.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gyqhaglpq.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gcybyonxx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gvbbajsjo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gshkiqevw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gyozqdbzr.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gymehntcj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gynljjccd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gkekkftfp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcrwyiur.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gxfmvesvm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gysbrfxmz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gcjefnpoy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gieuufnsc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/geawjwvoe.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gvdxviqyu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/gjpbpqdyu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gqchenxtk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gigpbynmi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/ghyeelvkl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gxwizeoog.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gwxtsejth.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gdbnhnilg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gxplmirsx.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gmnsrkqpw.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gepzhjfpd.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/gkoiegycd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gkxmljlcq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/ghbtqirjj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gracigyjj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gqbazdkry.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/gdznwxeqd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gceikwrcw.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gwnmphrdl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gdpmofzuc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gozglpsyz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gsxnhuhwu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gtqqnlcqf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gypbufsse.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gnjpvwalr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gnplmdgze.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gvtyfpgnh.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gvjmsjtqf.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gqfbmjodg.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gvnbkzuxi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/guuctzdwx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gaakfghtm.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gaxvmseee.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gigxyvcuz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gmxjhnpkc.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gzcrzjqsf.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/ghpqodalr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gdqghhcds.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gocxzmtln.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gopejpswb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gcxeeqhsg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gzdjsityt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gpgapfexo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gwdjrdxcr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/goioxcgah.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gphijjnub.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gsdcfscmp.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gmyllpkbr.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gefbgeiua.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ggioqafei.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gszhjtmof.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gtaqllioe.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gorzenabr.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gbdhylysr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gfrqpskmu.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/glhxaajrt.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/glrxnfier.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/glxtrqzyp.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gwpyxlydt.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gcghftluh.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/galcxebyh.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/gurwlhklz.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/grwbvgvsw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gucewqwyw.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/guvbysede.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjxnvjagl.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gubwiqxrn.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gbnuotquq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gutjfftgt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gfshvxkfq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ggspnsbze.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gpgtcqypk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gozngwpmr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gbqudsrpf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gbvwgomaq.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gfllfugre.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/ggttrdyrc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gfmwezavb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gcwkgqops.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gujzzfnrm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/grzhvuhpr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/ggqhamnqh.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gimlutyah.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/ghlwtanzf.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gpcqttmmq.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gxpvrslfs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gdyecevgq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gkttxfsnz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/glgcxrokr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gpdokfvcv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/ggljibkyn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gurkrqgjy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gssijwpve.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gpzmkctwg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gauqecfaz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/grcgdpdyh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/guntqbuos.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gmrczsnxc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/glpuquvkz.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gfxplnukh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/grzeglnkn.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/grjkfcoxd.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gxtsugkzu.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/geuttbkkn.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/grxhomgti.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gnbibwkes.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gkssjifzc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/glnmxvlgs.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gpvpsuitr.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gslaeyrbv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gwifclnfh.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gtzsdfahe.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gnlldwtgg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gsqigaidr.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gbebcmdhw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/guejultyr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gemnrjmqi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gnjfqvofc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gtpswbzxf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gdzhqkbgm.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gpviyqedy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/grumtafiy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gitonhsas.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gkpjnkirl.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gabhleacb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzjquqdfp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gzvmsbtwv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gdellujow.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/ggtyjppml.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gukbrtwez.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/griqfsazs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gvelapswh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gcuynypzz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gbcibvgfh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gfuffmzpu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gegfsuhzl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gzphcebgo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/ggjgitgpt.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/geyobkhbp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gsndwvfiv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gtiglbyrr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gentgvnkh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gagzjjctq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gqxnabyrt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gtswwqmyg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gjhpgpbcm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gfvjidcrp.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gyekxxrtk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/grjxfqdtx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gfrofychg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/giyqtizpp.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gdbqujtaj.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gimfucsly.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gpywgrhjd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gggmixxbj.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gehyfmgqc.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gldioactp.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/glpiyugev.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gqfmsyzyz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gamlooopj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/guhrvmazg.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gdjzmzinv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gipgdecuy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gqdtvdkjp.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gquocyode.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gpvhbjjlm.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gnkqorvwd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/grxrptqwz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gktflfyfl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/ggbplsutb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gemdaqwmw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gdiqmsnfm.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gvasqrohz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gwhrspoez.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gjjaetlyw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gehjuetuz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gcmkdiuoj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gvslmliku.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gmxorzwsw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gvxccanby.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/ghdybiopm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gyweqbupc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gtuvfbxrh.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gkiqrimbi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gnaiacbid.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gqphzjwqp.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gnzslzxfu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gqbyqscpw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gqwuszedu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gtolqpdkj.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gxfeujygw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gydagkiqk.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gxhnjnorm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gwwxleanv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/ghorhkyvp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gucvfoaym.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxheyvlkn.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gwdzzvwpg.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/guhvqtnaq.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/guohqbmsp.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gftavysgh.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/geqpqswmm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/ggibobkwv.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gmkrkfbgq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gbnpfhspu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gmtaudxds.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gkvlaouvc.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gvzhnzopc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gcdtobmxl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/ghsvzffzi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsltmpfzl.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gfllfoqwc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glxuenqsx.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gkkynumry.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/grgwukkdq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gmnvfbxtz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gkuiuufen.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gxsrepdne.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gdjkmqagn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gpteultlv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gqdpbgyfd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gtbfmvmeu.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gdglghqhl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gelfcebyq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gjzjbmdwm.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gdhfenewb.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gfyhfrhei.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gjgsptstw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gtvzfompp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gnpzahcdi.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gulfcwaow.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gekblbmiu.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gmcnmuqen.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gilvkqcwd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gbdlsplin.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gstcrbmzp.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gtarsmnwy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/golhhffmg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gaxbncqrg.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gqmbiihph.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gpjumqnfn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/grjljfvir.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/ghsfmcqga.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/grqyjnzfz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gsjizwwvz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gwspsxxhd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gkplivwjb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gverkutqq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gwtdodgfa.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gwzoitiok.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gnvrnxgtn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ghxmihxcd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/ggjdkgcvq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/genzltsxf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gwphqutnf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gntrjxcnw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gmorcmwwa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/ghfjveqww.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gfbkaqmfi.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gqrqwlzvk.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gihmbqctz.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gwsnidhbi.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/guwrtkbzl.sHtML


<!-- 参考信息 -->