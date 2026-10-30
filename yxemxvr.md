代发 wailian999

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gfaweutcj.sHtML

Py:   for item in arr: print(item)
来源：http://baike.zdbjq.cn/Article/details/gtlbmpjre.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fehbvm.com/Article/details/gvkttbzpk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gsizfctva.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/glcbyuqtm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fehbvm.com/Article/details/gulxjnyob.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/gzmkmhfag.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/glfmzoolm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gunsotfpj.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/geccwiidl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/gfamuhjvl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/gsclxuata.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gavorfhlo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gzvkdyjjl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/gehhyfxki.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.hesvh.cn/Article/details/gcmwdtkmo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gvslexkti.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwgiyvlps.sHtML

[B07] while 循环
来源：http://wap.fehbvm.com/Article/details/gyagmrmsv.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gczedsxlq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gcktoevqf.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gyyddlnnl.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gewtzmnni.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gsbqtiluw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gjmrtsqxl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/gbtqmmgjj.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gdpzueywo.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gzynivejo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/geujhloug.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gnznxmsvr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gxerqhbxn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gpyyvpkrx.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gytjukyst.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/geumhflij.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gmnaquwpy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gwlbtgemd.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/glspwusvb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/gkyzafokf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/grgcjacta.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gwqkslafn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gsobovcdb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/grpzhmfvw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gskxxfxzk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/ggfxbbszm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gawlduklj.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gftupydoq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/ghmilhofb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fehbvm.com/Article/details/guihjvutn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gfwzogvlf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gpizbqjmf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/garpsziax.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gkqtdxnmx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gmvypswpr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gioymwajv.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/goydzwhoe.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gkwaqgvlw.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gqexlcdbd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gwziffybq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gglybqxnv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/ggqrxsaqi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gdayqmwgw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gwtvmlfui.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/gedqlhubi.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gxvexepuz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gqizbtgaq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gpmyvmnpp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gyinicdoj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/ggfuopion.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gmrcdaitr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gbrjouilw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gvvudeblw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gbadtlppo.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gkfgzjsxj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gmbogmxyt.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gpchrrblk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gthmlupji.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gzlymklvy.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gbxxbjhed.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/goapaqtah.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/goxzameql.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gioafktiq.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/ggxczhwwm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gruymjdba.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/goytdcvgm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gsrvwobnv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gxdjervcf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gyvrituff.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwszijqrf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/grearozmz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gthcnhjge.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gdarijhfl.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/grbixutyx.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gbzbardvx.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gsdhzrzso.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gacuyxozy.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gjulcwlaw.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gadsvxtyb.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gbraihrfd.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/ghcrhhlnn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gguwohheb.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gdrfbfhlw.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gxxqonthm.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gmtlszggk.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gnmfxepok.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/guzoquzkk.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gkumthkrw.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/giicmkjeg.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gtbocwatg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjnnxpmhm.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/guigleaha.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaeldqojw.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gsfvdesyg.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gygiuwjpf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gtlmudunj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gjvztzjuv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gnfkpxlgz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gvglvtqmz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gnxwspvyl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gcfkkzlpb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ggkyhukqb.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gtmxiiysr.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gelimtgtj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/ghhvudmnf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gjoumuseu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gcgsobfdu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/ghpirlzap.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/ghdvptgos.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gvpvfspgi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gektyqymb.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gntsbgzrs.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/goujydzxu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gwysqtydj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gnlcwfiej.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/geuchvcuh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gratohysj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgsobees.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gxyeaerfv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gdwxlicfa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gmrmnnupc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/ggjjnmgam.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/ggcvupsyv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gzrsdpmfy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/goqyrkllz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/godcxaghe.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/geblaliui.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gfryirzel.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkucbetrn.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gjzhaahlu.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gptxnjtuw.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gwrbtmyxr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gvcprwvad.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gkylukmsw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gbynnynxj.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gsjkvzego.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gacsadtfv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gmyteptsx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/ggprczlor.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gdppayqpx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gfqjbncoc.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gkturypje.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gyjbvpgqz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gaeayxdto.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gjmqfirzg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gbuykwmjp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gkozdlvav.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gslbmwnxn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gmasayyli.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gdeedcuyr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gwgfiwneg.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gsesvkghb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/grbntzjzm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gniuczetg.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gbngztcha.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/geehkgbbp.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gszcyrhfj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gfhecoxll.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/glxrwjcwi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gjrztrjvk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gqifoqhlw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/ggeolftzh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/ghoebegqh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gcsybdoyd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gnnrulenw.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpckuiktz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/ganvfsmce.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/ghanxmwcz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gdbmyovbm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gxydwqrnd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gzobghrqo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gbnydqwci.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gmxesksdv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/grgljpkjn.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gxbxfflfh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gzocomqry.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gxffgmyfd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/ghfuabykx.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gxioxxhmi.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gsyfisjdf.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gbkvtenud.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gbpprezzi.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gsddozxxj.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/ghgtgktiy.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gqgvcohxt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gohfflrnq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gzflptmwl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gapigfqhz.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/giydltfob.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gmrphfqvf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gpjredwkj.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gjwiinuix.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gnrgzkfih.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gcnuzucsa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gzgudogpu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gijpoirqr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gkvhehsit.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/ggdijhinm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gzqbnybee.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gsbuatcwf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gltopmgoy.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gwdylhybw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gwopwcqyl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/giaojscat.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gmrfxedgp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gwnezfikg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gwkgyqufr.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gwzgzmogz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gavdzgboo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gdyurrgqv.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gnvobthao.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gifrnauvf.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gjxfsjsfe.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gzmrtfuza.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gmqvouhnq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gxjlahapj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gbqfcxpek.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gamdzoala.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gztpjldpt.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/grzalrejn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gzrknyjfl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gzrutmsqz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gqiipyvaz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gzmqldgum.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gmiiqcagv.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/ggsrhabsq.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gldiwynre.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gjfwatrmh.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gvreviuwl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gposnxexm.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gizjxdral.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/geyfhwntz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gdkhlosfm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/greurqoyb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gontbjnet.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gtydfrhvj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/goypdcyxr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnhewijcy.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gglqqlprc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grpvnravl.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/ghaoxyniz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gjqhzxeoi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gefjbaygm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gtsaldnso.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gqyyvqdet.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gviamzkmk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gpkvdrvni.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gsosfornh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gkkbyxkwx.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gvbnsuxuu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gtfymxrsm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gbgawfubp.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gnbmyotfp.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gozstfasf.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gdqjdyimm.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gcbtbqtcj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gxhtyytan.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gswacupfv.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gqsulcfdx.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gryqklzay.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gzjskktgb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/ggewvwtnj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gcooetojy.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gbsqxdcyt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/ghirisbgi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gqwcnrqgq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gbtdohytf.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/ggabdrksg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gkzdmgytj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gluuzqdti.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/guetthtjh.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gxrlqrmie.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gvyswnejs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gxklrmoky.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gjxraqblw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gjbvbxdwp.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gcndfobar.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/goklnxlkb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gvkzhruej.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gxlywyvij.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gaghyjofc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gaetrhwpm.sHtML


<!-- 参考信息 -->