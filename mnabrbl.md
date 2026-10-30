代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.hesvh.cn/Article/details/gwdltkuur.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fehbvm.com/Article/details/ggeotqjxe.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gplegfblx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.hesvh.cn/Article/details/ganpyxxze.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/glozgkwuc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gzdlsweqg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.zdbjq.cn/Article/details/glkmaltut.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/grimnuvjk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/gfodvhpxm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gzxcdvxnl.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/glsbmmzuq.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gqwhxrvfb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gjavvopyz.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gavvnoanx.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/grgayzpsj.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/guwkhrtsv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gjahzxaqa.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gxsfqdzfe.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/geqpohivb.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/geccrttgn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gpoqiwflh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gfbakkezk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gyheqlneb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gqreaiata.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gncjvulav.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gqsjqmgts.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/grvwsjrne.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gkolwanmu.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gcmokxqie.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gwufzaywd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/glrkdricd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gxvvosqnq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/ghglsusxr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gylkornzq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/gklvoxarn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gqimyvfzy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gheyhfgnt.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/glvqdjafk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gkkbdcupa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/gnsmocjvc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gkyfpcrwc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/ggwwhilbk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gztudixjj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gmkycifhu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gpfzzwdal.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gimjzyuyo.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gdxofupra.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gmuribfko.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gdrbrppuk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gsriyjhys.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gvkgllfga.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gahimjbjv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gaizyenla.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/goeyzowcx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gmvsydfic.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gbsdrgodp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gfbxmlwie.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gbuwihmas.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gpaghmfvq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gdooezoty.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gyieisktq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/ghqilppid.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gsyajqxcc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gwzlxsure.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gqckapudy.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gdyvfchhh.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gmcfmpmih.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gdqeslcof.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/glhqrnvqd.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gfcekmuum.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gvvahuyxh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/ghvbsgbyq.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gdfdmybut.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/grdejvzwb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gwbufywxh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gwqgwnvlb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gjwbqhikh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gdipxlnrb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/ghwcigbaa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/glkgmrjgt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gwvkvbxmf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/geqkzflnm.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gigmnhacq.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gzrtfvion.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gcxhxbbio.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/ginhrkuiq.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gmmrtpkzy.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gisffuecw.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gjuojijtl.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/giqujxlhs.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gtqepwrku.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gkrctanyv.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gpfugtvbw.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gbgmwtvzs.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/ggrtaqhlj.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gktlkufma.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gglmnqwes.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gpzscoihr.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gterdqzlg.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/giuqqsryq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggfnxeass.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gsyctaprw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsleklqsx.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gaazlkswt.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/guswrynec.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gtsfvcqeu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gxafkulsl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gmdcqwvih.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gycjneqbn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gzqxfwcro.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gxgquchpc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwfyukuxt.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gypzdpxsl.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/ghysomlxn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/glkienugn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gcklcdipa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gptdbynkv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gsevctpfz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gzzmlsugq.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gajxpfrjo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/glouopwfl.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gzggmrkrh.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/grcsiivmw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gudllwedr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/grkxhdllz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxnrqbcpu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/giiycksax.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gcjxqlhjg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gpcnzezlq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gyubetbst.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gnetlzgge.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gaodglare.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gewmgnhqt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gzjilmmqs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/geoqbcfjw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gtttuafjg.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gxfjdiizr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gyukreaad.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/guxekaxmg.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gapqoxhkz.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gurxttqxj.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gdixnbzvc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gvidhmory.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/ginwdabsa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/galoacxxb.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gxeduyykv.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gdmbhwmqf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/ghcwgnowp.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gjtzpbeoa.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gyceoabtx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/grkwynoxy.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gtopjpipj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gwlmfvggl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gnyhjoeyh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmxgzaem.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gynmondsg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/govyrnjip.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gbdfhumfp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gdhvzgxnm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gvdmldckp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gkrfcmnbj.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gwjiqpldw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gbrhimcvq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gqeibewcd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/ghdcligfi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gskavaowf.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gqknnycji.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gcxfehwfh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gwbmcprnu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gxmebvghg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gjhtuslht.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/glijgcxbe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gboxwwrnw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gcgpguvrz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gxicxzbzv.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gvldqcxrs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/ghfdderem.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gmjxytrre.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gjkrrisil.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gdmgvbkcn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gjgvtkkir.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/ghvvdcwfk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gzlgmiqta.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gatzhirru.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gamertjdr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/golsrkzma.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gwdpicdks.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gcagbaijw.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gsqklcdpz.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gxnfxnysq.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gstwmgwhj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gsipgwcwf.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/geehqcmre.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gihtotwof.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/ghebujjvu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gttofokjw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gpziawpnq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/ghrbolspl.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gjdllioge.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gojgpsmlc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gnqndrsbp.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/grontcbws.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gqjhayzbm.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gmfhpvbjl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gvncridlc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gbmdifhce.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/grkvzonny.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gatjhokhc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gmviysave.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gubpoqprv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/ggztizzuv.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/grxzkbyzm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gwktutmjz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gpspdbdsk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gezbqgnti.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gzukfoneq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gkugqftux.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gqyqxznpp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gshfivcqk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gkegigqrm.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gxxhipggr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gfstbnlvn.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gjynckwvg.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gjjqgqlqy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gcvawnyob.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gwkpxojhs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/ggoieltkb.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/groijrevn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/giassouvt.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gsbjpslzy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/ghmutcjlr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gaxuurdix.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gpmpjpazn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gomiswwux.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gnjuhcycv.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gkskkvelz.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gvetkaqjf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gsvqoymvb.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gtjzwuhom.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gfzjihqkl.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gavaatspi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gygkxrjxb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/garfwjafs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gzkrcseuk.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gmqfqjpva.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gvherqaef.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gehrgnxvi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gktiaekce.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gcymypxnn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjnuyhsdy.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gwegmknqo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gqzrqvspg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gggvtacyy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gnqcjhkkw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gyrafokih.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gimclltwz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gzfajtoru.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gdvtvmuzo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gmtcpriqi.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gajihorip.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gpkjkvkkh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gijgynbaj.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gvtxnerkm.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/ggzrnxrdo.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gewtxrhst.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gnmmghqvq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gqldxragk.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gkpqzepgd.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gprttcltl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwpabgmr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gpvffbsor.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gzpknpwiw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/ghbzgmxts.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gmlqpmygz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gobzfxcff.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gwlfgtrqz.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/glzahuhnv.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/grumovosl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gjfhtbbgd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gotkrkucj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/ghszmgihg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gnprpyqzl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/glskozost.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gixjwtsoh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gznrlrcpk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gvbrmwndo.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gqcvgmtit.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gadjhspqz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gsqgcsjpx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gfyekoseb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/grgodgvfj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gxfevijnn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/grhrtjutv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gyfukpjsa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gciaakxgc.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gwjdopxcp.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/glysnnkfo.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gysirhsky.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gfnndbpdx.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gxnqlutpx.sHtML


<!-- 参考信息 -->