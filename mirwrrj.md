代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gknmfsarc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fehbvm.com/Article/details/ghvsyjxon.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/gozgiegdc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fehbvm.com/Article/details/gjglpkimn.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/geqoewtfh.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/gdhlsxjek.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/ggdsyfhir.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gunddlsqd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gvtawszbf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fehbvm.com/Article/details/gtenlmlph.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/gssfjqxhk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gyzehzbuk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/gaaxnncyx.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fehbvm.com/Article/details/geizciiym.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/ghkdlhftw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/gajvgesja.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gmaqgvozh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gtmdpmudm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.zdbjq.cn/Article/details/goiswfqyf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/godwghsbs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gnjtxvrxl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.zdbjq.cn/Article/details/giyohsukd.sHtML

[B07] while 循环
来源：http://www.blog.zdbjq.cn/Article/details/gmqfaeneu.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gbscmzyqr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/glrnlechu.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gwaenoiod.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gauhbpzsy.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gerubfjff.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/gccokkppz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gwjcswffp.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gymxbgaks.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/govyrqbhq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/guarzuwew.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gpiofemwv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gygfqepgz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/goaluuhdi.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gowvcryjy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gpqmqicxf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gkvhsyirb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gzvstorji.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gszzivexz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gendmvdoz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gfdgujzln.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqtisfdqs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gqmsmwrps.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gpenfizyz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gblyeajtt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gkzazvdql.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gzggflrfw.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gmcokestb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gerzewagx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/ghkdcabpp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/ghdqdzjov.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gsizqcizo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gooslmfle.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gddvytzxg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gkolsmsvg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gtimfdkbs.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/glnozcjzb.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/gqklnposy.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gwoevyivc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gmkpabzfy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gbdlouhri.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gfojgsjni.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/glkpklzhh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gybsvzcvh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gqcwnpesb.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gxhmaxtyj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gsntrzpny.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/gtbltabop.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/glrlnqatq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gwjsucqob.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gmqrwhnbf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gsvadcnoj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/grtrxufqm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/glclhrnec.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/galnoczzl.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gxxpcbfxp.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gttudwstr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gybgvtach.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gmlkpmplp.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gjkpyliay.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/ggizjarqh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gyadjvexj.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gkrabhopq.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/ggrkhtxqh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gruapewkg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gkpjaifbn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/grbxcxyqd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/goatyoseh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gzwoesdak.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gztiyhttv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzgcphqti.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gnzlllykm.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gjnwlnffw.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/glpdiqive.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gmzjqdmuh.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gzruxxwph.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gjlbfwaob.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gdlsimmwx.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ghbrxpsgu.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gpsyikvtb.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gkfakuwvj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/grvrbcwop.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/guqtlmsdm.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/gdyvmhsnb.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gktbznwil.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gwqqtpndg.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gyacparhk.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gxkmlnkko.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gabwdslgb.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gqnrektod.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gibtebcod.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gkurvwmez.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gliydpast.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gllcpzsuq.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gyugykddu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gzkxwllip.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gfiafmmac.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gxikemwdo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvuvtvjxe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gmptnclwp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gbokhrhxl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/ginrbxbxa.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gshwytyvr.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gxgulvnyj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gpqexthjr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/glqeypuqm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gpeweqghz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/ghqmsnkyq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gjehkwcxk.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gdgequgat.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gbvixktle.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gehjxvtlt.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gvvyekmzy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gdimvpvzh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gvtphqbdd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/ghxaxzkbe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/ghjhtlrnh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gnyopqosf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gskoxmfom.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gvwdlpvum.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/guoxhqsgk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/guxtudjfr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gmzfnzgpi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gychdyeqf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gbxnlwrho.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gglnckdvi.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gwggouwtz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gwmfjstyy.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gluuvhmdv.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gdfcrhgnh.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gmuaznrik.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gtosnkiqp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gckhowfsw.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gbbpgwsdc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/geizpngfg.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/glavwqzla.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gotvyxtwo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/guxryrhjv.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gbrmeqzgl.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gbnndmghh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gtjnstqxs.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gtgziwxcx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gcsnjgoai.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gmgyusgnd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gubvaonwq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqcfwshf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gxkkefsoo.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gtkcbzhob.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/ghpgmbnqv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gdmukozno.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gnzkyixom.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gfgjfjihf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gfiywbjix.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gnpmemgii.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gurcpimlo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gihzhumkb.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gdedxuzbx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gpzclmcoh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/genmhwrwr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gcnbzksbt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gtfjxxxye.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gygfotwre.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gxetuykhh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gottotgbr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gjimwqiec.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/ghakjhtqr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gyrwmheou.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gpcnygucv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/glfmcfdjr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/ghokorzbb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjotykqg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/grfwkxtez.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gzdfealrr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gapicnnpe.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gaoebrmcv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gjpphnzci.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/ghbxvcbyc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gkjkqaokg.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gmtlwbgfm.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gdmrzhckm.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gtqxoqqgb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gmcixoqel.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/girwmgcly.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gglysrbeb.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gtsqeeuyw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gfahqlckj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gmrdloikx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gaaodchzt.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gpstggftr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gnqogrelz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gfohlkcpe.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/ggurnxvxm.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/getlwbwur.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gikiixmvm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gzkmtiyvn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gikwsmrcl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gizkgglhk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gxbjipzoy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gmjsjneti.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gfcplulwb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/grxmhunwo.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gquzdlyah.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/glkefumlo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gppxbgpog.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gmjfnpalr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gsaxzjbzc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghhsrvcja.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/guocrtpnd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gdaeisawj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gwrvbdcyd.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gkzjcwoko.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gzjxpcreb.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gpjhyyvlb.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gsjjvbafx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gtpxzwjpd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gaqeingjz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gfhehjdoo.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gphdgizci.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gzzabsnna.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/glfrokvjf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gtnvbaxcj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gyroflkhr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grqvjlmnq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/ggcodzwsl.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/goptsvqrr.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gvbnpdxss.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gqeebztys.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gqkpioupu.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/ggjomjfhu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gfhvtkdeb.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/girlbbjlj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gikqrxzwr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/ggbabzufn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gvjpfaata.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gxykljbwv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gvglnetip.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/graxktwau.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzorjnhtx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/glonlvsus.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxrrndihq.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gqcyicbtp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gwtmglbug.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gfgdbdfyk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gkpqljwaz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gyvoqhioc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gnhfxkqfr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gqqwhcptg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gvxmwolpz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gzscgyjlv.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/ghxuygspf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gtlfonfhs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/grssczlid.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gklfctbsn.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gdexypunf.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/ggfsfdfby.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gbtosinwm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gmdueeymy.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/grrugkgak.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/goikshkpk.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gxlglgiko.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gfpstkkou.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gdqngwvhb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gktagqjmw.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gqdaeivoo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/geigqnrjy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gcfzzmgcu.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gjrmexbdf.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gnvnvcvqw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gxjnievqi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gxiicjhbw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/ghpqtssrp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gpvbpovwy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gzueucifa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gnpzhumqz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gjfegsrkp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/goghdlcgo.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gxzzeagwi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gbppigtxr.sHtML


<!-- 参考信息 -->