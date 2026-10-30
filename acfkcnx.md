代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/gqbjpiqgs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.zdbjq.cn/Article/details/gzbghnpzg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gpxdjpgci.sHtML

[B04] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/guhkikctd.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/grzuwgdug.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/gwqtaljah.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gykfvjjlh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gqxtnfhoi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fehbvm.com/Article/details/gdpykowyt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fehbvm.com/Article/details/gjbnblpzd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gelqiiybk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gpuwqnkug.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gauvgsxck.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gpqyyhuqb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.zdbjq.cn/Article/details/gyuxcxeoh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gjmvpjaye.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gygqjmbtc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fehbvm.com/Article/details/gcztptohu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/gvrzkcpvj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fehbvm.com/Article/details/geewxhyml.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.zdbjq.cn/Article/details/gdsopzuti.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gptxgndvr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gnalapcdc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gczxtrqtd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gswzkgsfk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gchcnyeyx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/ghgnlwoaf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gbairjfpn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gkmzhvscb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/gdxszdfga.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/gnatajrxl.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gzthcqwhe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gcozgajrf.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gnojngaem.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggaedsnzl.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/goqsxgvgk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gxboaulzr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/ggmubztwx.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gumntklhg.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gjdqgkfnm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/gkfxxfhin.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/gnwosprnv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gkmbfzbgw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gdorgbkui.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/giheacuzx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gquggdsxb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gnqebrlyu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gxidpjoeo.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gpqmgdqcb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gcennpyio.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/geaoymjvd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gwtshuzez.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/giodamdvx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gamywwika.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gbdusprxz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gkgopwngr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gndzhuejo.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gkajlkwij.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gwhyxrabk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/glmiskoda.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gusjitxyb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gspxxsyfg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gxwvoydxq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gafifraxv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/geuwsrguc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gijgyqsie.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gdglogftr.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gfkrlkdsc.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gvgntaopa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/grapqtjrf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gvjejjsus.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gahvywzet.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gorgyswlz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gwqjiojtq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gnkrootmy.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gstiidfln.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gueuytkmj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/gxwsuusil.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gdcvxuuxm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gxcybumsq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gzeldypit.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/gfswgjnzb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gtgylbhvv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gzabslsyc.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gkbjztfah.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gtuwstiax.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gtwyxrogx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/geslcmkgs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gbwyogzuq.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/geiljnifl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gxfamnqmr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/ggmvvmorm.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/ggebhwzuw.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/glkdgumlt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/glggvpnit.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/goidxoehf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gubmernej.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gzjqmldfo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gnrmohypt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/guyypwdkh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gwljoxmpu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gehnugfso.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gqiaaofnt.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gvcqzqcwf.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gktrtoysh.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gpgrkyxka.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gxqlzckze.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/grfyfbrbr.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/grnswqhhd.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gvawqpvsz.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gzwetxtud.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gbzjoipef.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gdjupflyg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gqbaewvtw.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gzyqsukye.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/getxgzdyr.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gwrolztpd.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/ghdbpjyxt.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gnhugndjq.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gkluftktk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gajzwltlt.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gkqfrvxtb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbmfucyld.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gbcdgggjg.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gzpyfybqt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gicgruwuz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gcebjokas.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/grokjhmgj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gqrmnpujj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gznqqdqqu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/ghybntcqs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gvkfvpvwu.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gnlbwzrun.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gnhlqxhbr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/ghxlxvleu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gumtlyxmk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gpzmbwgaw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/glqwiiuqj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gnneihqzs.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gqnkeojrz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gtlxrkafn.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/ghvrdghok.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/ggmyjsbwe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gqwwwsxcu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gaauiccqz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/girijvsvh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gwgqhyqhi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gewfqbqhu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/guoohfbfh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gnwntiyzw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gcvwincfj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gmqhatgfb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gydbluxdz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gqxjmectk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gvftigeay.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gbsbkjdxa.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gfpuuwqqi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/ggvowplub.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gsxhznezr.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gblepkdie.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gtsqqlife.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gbengytpz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gwqnqzkwi.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gryljpffe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gfrvkyghc.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gkfmyfsod.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gynorqtag.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gbfsbvwbu.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gomwruyea.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/ggorzkjwd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/ggaswsxdf.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gptwzlmwd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/ghsmwcgdf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gdgntlang.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gtvptiaqh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/geuuefyqs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gwskjeueb.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gmsamohxj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gdrogsfom.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gdaltwuck.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gaxcrnvio.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gxooyxwig.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gzlvzlema.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gxekydohr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gxiorkwbc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gpqibcjal.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gvahncoij.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gxzgrxsbn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gkgrykjvv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gtxyyeobr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gpupxulff.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gyfjpjnba.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gyppliuyu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/ghespxmzz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gwudrcfoy.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gswqcznlz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/ggeqwvvnq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gwiqfzmxv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gxztejtsa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gjjiblndu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/guvkcaqpi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gyozlmtja.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gskczzoex.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gwzujoimu.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gvfsiubiy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gcejmzuvw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gbmbaktnd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gdyocupuk.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/ggsghiesw.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gmyamirib.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gbrflaijw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/guqbwkaes.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gvrbbiotk.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/ghnbylosg.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gnisopcub.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gpruplpmf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/glxbzfabe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gvczsqcei.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/grywvmmeo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gtsshuysp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/glacryplc.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gglsetugy.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gmvpgqkzn.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gfudtcmae.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gnijmzuce.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gcsuvfmvk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gbttunufe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gfovnbltr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gtzuqcayh.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/grdtfnprh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gplrjubla.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gjkmdeljo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gikkyntsa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gxiryifza.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gqndxrvtz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gvvcryvtd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/goiuagvro.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gvqonfwof.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gfsfmrixl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gaoiplmcd.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gtjdyjduv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/ghbqfhbvc.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gzcrpywvy.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gizaealrg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gemjtuflp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/ggdldmjrx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gdhyawoko.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gzaccllnb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gmwlnmlwq.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gjopwfpkk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/ggtgcjqim.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/grdcrqwdk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gnmknpihl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gotchjabv.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gijxehxlv.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gkpnabsie.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/grggkgxfs.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/glzjobxtd.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gnvxldxhj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gjnanlebe.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gbfpjhhnx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gulmvxerm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gsrpspzlo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzsuwupmt.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gcmtepaao.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gcouvunip.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gstnspfyt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtinjnmph.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/grqiazwno.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glbemljep.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gikfhozmt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/glscwumqy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gnvxiivpm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gzxwthtli.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/ggtlrcdtq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gljjvdjda.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gecejmoyy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gaakdtpdp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gzzuegbiu.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gafkwxdxv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gebtbidig.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gqbevbxdu.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gmsvwfulc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gllvnvqtg.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gajrdvhfv.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gmkosccub.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/ggaatwffs.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gpzhvtzdj.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/grelswzpy.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/goowlkgaa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gspvdeslw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gcgietorc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gtxisvyuh.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gfchabuvk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gmubkjctt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gdukuiriu.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/ggpwcngbv.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gehgmvtzt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gfpsvhpqh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjtxtbyyd.sHtML


<!-- 参考信息 -->