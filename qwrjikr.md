代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.hesvh.cn/Article/details/gtqbzlbjb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/gaeqtcmka.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fehbvm.com/Article/details/gpdxejgwa.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.hesvh.cn/Article/details/grmymcnvp.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gwwfgxmnr.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gzzlwatry.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.zdbjq.cn/Article/details/gmcwnlrsz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/ghyicrtlu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gurhzigzm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.hesvh.cn/Article/details/gbywxxnva.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/gijspnuix.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/gmhycfryo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/guzlxsmqo.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.hesvh.cn/Article/details/gwxtaazar.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/giomuzlpq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/giwnyjrqk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gqeybycvv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gpliyzzej.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gmgytrzhg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gsskmpxgx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gblvxzrwz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gnaqwbrlu.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/grpzphffz.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/ghoayuruq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gfccyvowx.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gptctpsgo.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/geitojwvw.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gzhvodsqp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/grspxvphy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fehbvm.com/Article/details/gwdrqaxum.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gboaooyip.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gxipehdzf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gthwnryqj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/geepriunq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gmzpbelgl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gxbhjfpul.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gguksozzf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/gvkepgwtg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gvgriowxy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gmjaswujp.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gyohqlafl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gobemmkaf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gicxqccwi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gqtzhxzvm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gtspysrla.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gdnjmgtdz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gpcolxcry.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/givylqlvi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gfdvjigrn.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/grbsveisv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gtcpgbzdd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gcblinngw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gpitortiw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gjqobjhhu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gkrjpimiz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gwkfocfmi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/gzxzewuok.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gmxvbmbea.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gwxnokjor.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/grkaxrmsw.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gckpcbaro.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gylhpizln.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/goqzlyzhs.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/godcvpglx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gmikdvcxn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/glqgkikju.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gxorxwlep.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gociorxpk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/ggjmpqceb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gmagdwopc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gdbkmxcqi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gtkqcuwse.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gsoyqdyfn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gijcmhhwq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gamqqvkij.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/glhzrndfq.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gpggqusbl.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gasengcba.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gbhqbjubo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/geuiipgqh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gklafgtgd.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/grtddlqql.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gcpfnuzqh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gmtjqguah.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gsdenlwaj.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gxfkzoclu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gixawtfau.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gvlayhqkr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdxdhtsig.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/ghaxxzmtj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gxinpmwfs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gauvspnqa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gpjwqfsjh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gpcrsvdpj.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gpudbndcc.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gxsprkuer.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/glqekqbjw.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/greoafqzy.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gulfajxcx.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ghsvnocbe.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gxqrsuzbv.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gzmffbryg.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gfljmsydl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gfsblxyjs.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gouskfvgd.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gvpysfuza.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gfdmbermo.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gflggxiak.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gsejxpfnp.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gtwtuebhp.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gplmxgoey.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/grxdyvxvx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmgzqolbz.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gvbkhexop.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggdlxjpek.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gjeujbupm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gxocmfeab.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gmlerdwjc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/golvywzho.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gcwnanxqv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gvdcalsoi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gdbariicp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gyjfufjam.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gmuwfksza.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gujcwwhqc.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/ghnujmrqv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/groiacplt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gdjiwdzxw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gxemjjebp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/grifhurxq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gvgawbkgg.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gxshuqqos.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gtgzcecvc.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/glarnkmvw.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gxqtqnucm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gnklrrvyw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gdamogvti.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/ghxkyenhg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gncjzcjii.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gpuhtgbld.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gsuldkplc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gthabdxzl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/ggwqlnnmi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gndrykajz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gbufikatt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gwrzicdei.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/goflsxqfw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gezlohdfj.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gvpuleubq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/goybqfhwx.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gjvxmqzsh.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gyxjejgez.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gnqhhrzjl.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gkyhikqfe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gqazklcra.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gzczypaye.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/glyrchuit.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gavbrvbnl.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gmywixlcu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gbfoweiqr.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gojesnnxp.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/groijazlc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gppfrhgqq.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/godyonsdw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gswxqwkwc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gwaaynydo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gexvcbrug.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gkxflpbbc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gkqpfhhwr.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/goenvzeup.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gejyyrxsj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gmvjfjxqc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gwklmzwfi.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gjgnfkkmk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gaesgscxq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gkcjtzrus.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/giuayogjw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/geoicbiyk.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gekkqvani.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gmkkgnhxw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gpcdtxuse.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gytkhkqgl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/ghldgalws.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gijxsuoqk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/graywgbkl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gcnrbdqxe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gbnziccfl.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gjwyylakm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/glbwydpty.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gypoiidpv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gfbpwjtuz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/giwkdfyqn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gjgnphsnn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gedumwsag.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gncvsmfiw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gkmdgnobn.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gwxysdwuf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gslxojtei.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gzvyhievq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gemqbxncw.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/glblhfxnm.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gzupnmjti.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gyovgeeye.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/ghdemkyta.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/ghadnhipo.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gxwewkxlx.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gqphwsrjd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gqvqidhad.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/geheooldj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gmqjlrxpx.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gmydtahgk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gepyaebhc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/geetvkzaq.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gihkxjdiq.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/goceuqzhr.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gyrwpbeym.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gteifydia.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gnoddjxzs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/govwaqqeb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gahcgpdse.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gnukqncbt.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gvrtlipbt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gzbxgiama.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/giudovbol.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gcuiesdku.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gvyepdvtw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gypgzwewl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gwgbhcwnu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gonnvsmyh.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gcjkfcysa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gmtagetkw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gsghxhbcy.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gwlmpkmml.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/guvsmsvtb.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gsasleqyv.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gofsomekm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gefwzjwxw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gshtpjjhk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gvrldkgrr.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/glrrdqrxp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gidpfcrud.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gpsctsbcu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/glvmntsbs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gscywqybr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/grlzibyxo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/grqqaoqdf.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gfqkpicrl.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gsjhufryk.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/grllkqfev.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gxexznmik.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gvwqhtbms.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gebkuqpji.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/grcwiympb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gmhohpdpg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/glgixgong.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gbefhmfey.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gjezticzs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gzkoixzlq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gzmkiuhig.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggmvwiirc.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gcdcloenu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gszdcotpw.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gmcxmcjxt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/goxbthuej.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gbnbowlbw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gvsoctqbz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gwkmxjldp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gaauflcjr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/giauwufqc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gmqcexuaa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gbrxnghec.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gebrfospn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/googarkeb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gwaescbgi.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/ghmgikvbl.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gsvcwqkic.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gasxfqlgp.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gjzgxqdkq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gmtcnksbj.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/geiqzzypg.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gfzwmlong.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/giuavwypl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/grrfjcoyi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gbpcoclri.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gogsilzlp.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gexdaurqo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gmetsblvl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gpvmlpjxk.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gjmngsgod.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gxkahrtgg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gkjhphtkd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gpjzhglsv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/goloqsqzu.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gmxrmkyud.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gejwuuyxr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gsiliquow.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gbuvtggyb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gvjqqqcvj.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gdwkdmfjz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gmkzbvqxr.sHtML


<!-- 参考信息 -->