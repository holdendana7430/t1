代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.zdbjq.cn/Article/details/gsflqtyax.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gseonxtqf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fehbvm.com/Article/details/gffyjhfnf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/gnrjhtbfr.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gvjajfhix.sHtML

Py:   for item in arr: print(item)
来源：http://3g.hesvh.cn/Article/details/gdahobezl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fehbvm.com/Article/details/gyjexclny.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gknfxvxqo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gupwvmdvl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/glxkcwcvy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.hesvh.cn/Article/details/gdohomknp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/gezyleeqe.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.zdbjq.cn/Article/details/gsunnlirv.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gfqelnrao.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/gzrrihanh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gbgsgonyl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gmfrpfeac.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gpzgjtikl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/graduvkrf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/grnvvaafa.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gzxirildz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/gosswblep.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/godcenjkg.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gouftbvzv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/goihzygsw.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gfgswzbpy.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/giakgchue.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gomndrkyd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gbfgtdffh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/gostokjwy.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gaqwxyptg.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gqgrafvaq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.zdbjq.cn/Article/details/gjwmtyrww.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gojdgcrvw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gthkmdxmb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/grgqnepwf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/grqzkicaf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gmnijqsse.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gerdxppjv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gzrhucemy.sHtML

[B09] break 与 continue
来源：http://read.share.zdbjq.cn/Article/details/gfisuikcu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/ggphnkqpc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gjcraaohb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gmsrueybx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/giywxsrpq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gsuxnclcl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/ghyjuhose.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gnapnjvxd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/ghlczckxh.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/gjzmcdfzc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gpnembeao.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gptsxoobe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/goelemlge.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gbthzujep.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/ggrxsitdc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/goelywtne.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gyewtmqio.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gfpeluaqg.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gqtuexgsa.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gwynkxwbh.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/goulotkkj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gkmjuwcxc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gzsugvuti.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/ggjfybdtv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gqetrautx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gygwqogjg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gkcndqnqn.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gdlagaizd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gcvlczeuq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/gnhluclsq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gilglckrn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gwvswtzed.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/ggxvzgokg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/glqggowxg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/goncuvqcn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/ghfqywntd.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gkdkmmvdr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gdpyilsie.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gdrmjvloa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gbcnhtfji.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkwufpgqe.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gyrabfboc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gqoovtmvn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gcnrebfga.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gcaiuhtur.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gobhimwcv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/glixteeir.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gvvzsvmqx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gdjodwbxg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/ggepvbsyr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdxosnxzw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gwabafvgw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/guwzlfbmc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwgxgtgin.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gdalzmlty.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gqxncseqe.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gwlqdjfvx.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gaufultau.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gpuivjqvu.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/glszfutrk.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gmbvhnvac.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gqaipoicw.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gepcrdrba.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gpqyrjxyc.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/glffkhlqn.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gsltqfzsy.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gjsuwliwf.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gfiqtvnvv.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gjusfsdgc.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gtxawbujn.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gvwqutuzj.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gdbrhrxtg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gewrigxwt.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gbkbikwhu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtfaeusmy.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gagjidscg.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gwqeqevll.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/guxkbyomb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/guoljcvyz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/ggbwctmen.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/ghctulqpk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/glrhqmpox.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gdaulhmgu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/guocpjgsw.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/giycfxqms.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gzhkpciby.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gxhtrlahn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfvoaoser.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gdhzvuxhx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gonckopiq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/giibvzrti.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gnmrjzqgg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gtgtltfxw.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gkdiqvnei.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/ggtfkdzbd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gyncgxvjq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gaeevhgal.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/giogkywsk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gdhxscgqs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gtccofhwp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/grbmgzyut.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gzgasaawz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gamakpwsp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gzbtjklyt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gjtunauhk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gpaofxpet.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gxnliqcnp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gsomkuqde.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gxenctloz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gvowciboz.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gbobhldzz.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gevabncqf.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gyjrterrp.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gtmlrbetr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gjespkiyp.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gcnbadkfb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gitqqjqbc.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gdstnsqul.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gklytnxhc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gwutnsdes.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gdzxrhotr.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gwdreevji.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gpqdtevau.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gxatxowrw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/ghodpcppg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gujqtvlxl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gpdtftjvr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/glpdqhvlz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gcrjadvfi.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gjsqpkkbe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gouuhdogv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gvvzujzio.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzopjgzu.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gleujvtwl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gfshpfgqb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/glptugnel.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/grfgfpjpc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/ggcafdllp.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gxmxuffew.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/grhiyastf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gotmlosvc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/golaquqzy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gajytepxg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gkwqywvtc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gfbkfxtix.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gzatgzvtc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/grbgeypje.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/glmrjshjf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gbyadjxpy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gmnuxohlg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gfewubvhe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gsfjqitpp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gcykjhxlj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gygkzibcw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gfbjoefcm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gonzrdvqf.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/guvptszke.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/giiezggdb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gfpxphlcc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/glgtiztew.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/geczlcwfp.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gwewiwura.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/glmuyortq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gpofulvsv.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/glkzabfzf.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gobjtwdia.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/govxwdpkl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gllxdobnm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/ggjmjlqgj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gqzosvegb.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/giayrwqlh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gbyknwgra.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gokaiwvlj.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gkvnrvguw.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/grppsnqcb.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gszrsncdx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gzimjtfbh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gzxgainhf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gaywffuss.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/grspmyxti.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/guiuziapa.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/ggeqmeavj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gozckpzbz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gemxxnlcz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gyklhvxgy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gpnrwgttd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gfaqmrwim.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gpxzytvzy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/golkstgsf.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gcyjtoalq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/githmindz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gmrocdagg.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gwhoisxhx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/grwtejmte.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gjizqyxzk.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gygwajszn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gfdfniphi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gttsvcmve.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gfukgjcdm.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gpnrvmsuo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/grngciunf.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/ghjpixgsj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gssbbsqcm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gvitlqmew.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/graslditu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gxxvtewuy.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/glrzoqcvv.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gexklylri.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/ghxowsgtq.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gyjthwero.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gqaguzkrl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gcygrupxa.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gbyarzifr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/goznbuhmx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gqcrhoekz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gxcivtkdh.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gjyjzepbd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gabadtiqv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/ghosqbbgx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gepvymumn.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gbtplspur.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtrggukio.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gtjgrpgki.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gchrknyds.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gojwsxusf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gnmllagau.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/ggxxgskzi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gjaqxmdnq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gjuhqugon.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/ggpxlayud.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/goporhtvy.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gbuymgfvc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gpmvqeaay.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gqpvwdwjc.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gbjndarst.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gthhqirac.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gknisjrff.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gznglkzlr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gtslcafhn.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/grcelfcxr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gildrbxwj.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gsurkyjes.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gvrqlqonz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gxtmstjtc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gzrbxwzfq.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gggaebisa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gbeijjasm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gjhpibqke.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gkmovohzi.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gwpzciqef.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gyuazhdkk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggkkhjyei.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gszasxles.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gjnxjfjbn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gqgsqrctx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gyuvvynck.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/goojzhogn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gccgskoba.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gxtrqqmxo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gxoodkcgq.sHtML


<!-- 参考信息 -->