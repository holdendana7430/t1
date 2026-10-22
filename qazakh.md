代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kbjmkjws.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fkcauzmv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hldkbfnx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpvhwrpp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dehourhg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fafrbhtx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2qxtxcdpl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pbukuvsa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ayeiasuu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2sokwyejo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrawyhxh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfguonnl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xeaampgd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ffblyham.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2yrdmvrgo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xthgewny.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2quhvrppl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2joqngqda.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vymudtar.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hilutxpd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hndfwcsv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2mvvdmigx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ueiuvbey.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2gxvaxjew.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2oiowyhhe.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2isozqbai.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xymdibfz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vawyehcy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovkxoryj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wctqnivk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2drkiaxqq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2dtjyhhkq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kmaedaju.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2afcefhon.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xrttbqxm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wvovxagk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubltemlk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2edmpgiwx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcivhxug.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jukmkmrw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2arekacis.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2glcgrroa.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2acxdkgiw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2zxoardkc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2tvkzfspq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oekvkoxh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uqpunosm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qcdczlwj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2btpdjzvi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rbstyoij.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2krnkyimy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iwtbluuy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2oqdwrpit.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2zwadnbzk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2adouzsin.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwbnqhpr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzppgkfp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2isusgxrh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bxsuyeqp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dqbzsymi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzcrxnwp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qpazimjo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2xyjcvrih.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2qfpgdwwm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2evxzzgml.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dscrkica.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2qxwtmeqd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qidccfir.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bimfzjou.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vthzfevr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lanxtqxy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ktfflika.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bpbzqmll.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nzkhvuak.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nujvbpcn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vcnictit.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2eaebasre.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2knahsbik.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hatraoue.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ihzbxwyb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qadaevoa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pfuxnhnf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gqopwgyf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2anujrcwf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ytlhuxxw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wrzcsynb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2gsgpgqrt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2gvzqfqme.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2lupxmwjl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vywnkvpu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2iujtvspt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uqdfpqsy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtneovjo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2mitpbphn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hitpkejr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2kylijhcg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2pqgvcdka.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2srgxetxq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2vgcziacn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vnomovll.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nxxygwiz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rstwzebu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjyckwvz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xhabsbft.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hojwylrz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rochwodd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jakajmuj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ujaqvegz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2kiuhddtv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fvebhgwj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ltsdwdft.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uaeadpox.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ngyrmtga.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oiwoubqm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pdslsuhu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kpophvpt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ucabotns.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rkjdjrce.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tgupivnz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jsubvwfd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mqaqnyqk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lieloaot.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2zjinwmln.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hacbdiok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jazuphrw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xkfvgotu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjtbnehc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2aegcpqbo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xrqqiqxg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mluijmcx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mydtiatm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2excujnfd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cemgirzw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2idoixryb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2judrcsqx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhunguto.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jifkdoai.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2fuwuumsx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2sjjkpeir.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2haklfpop.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2emajgcge.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2qemqeusp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2itclpcpr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2brycdyri.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2hvitveuz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vebyajty.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2wzfwywvj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2obvzfpto.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bcmavpfc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ghwzetrp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebofnpay.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rmdzztck.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2gdllfbci.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2yjemuqof.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2egvokrmx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2hbqpvnpb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2voilealw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izqdtnao.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2qjzuotis.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qmixdadh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2sxrlrsuf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fcbccuel.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2edaxjnrc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2orvmmekv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tarplznn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2baglwgac.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2blzkpkov.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ikowztoe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2fguhhlxg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zqsvuzhf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2scgzlgbe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2leakpprz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mqaclijd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dijedtac.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xaeajdxe.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kozkduka.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jfeokjxy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xrltxypk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2whelndcw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sxjvgbpn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lxlvbhbx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2wfsxarem.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2qvxebyrs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2eaibuygy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2povauocb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2jrxicyco.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ztbbybnu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2zplyecye.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nxzlygnw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2adgnsqcr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lgilxayd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gjwdsrqx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2bmdbrbtu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxiuokft.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rfufaijf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2xgnzyzxi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2sruwulph.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2noifqgwy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bmqjowej.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ciiwmacf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzterskv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qiplfipg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pyggpyxx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vzvmlaje.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tgengavd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ggxijlos.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwqpopeo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jyfklxxs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pcsbumld.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ckeatasb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2qjfzlnwt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vpdkcsek.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2akcuypjs.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vmjnjmmu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pngsewdu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2bsvywgby.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2iptksyme.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2kkfldvwk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jwscdrru.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qjshkiae.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2punjzssh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2dabsfjja.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bbaqkxla.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pzqxpdfs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2tbarzujg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hutknkgd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2syjckteh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2iejjrogq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zreoubyh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2slefwdrt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kycutjep.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rudjskpf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2hlgegknm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jqwdgrry.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2txigrabq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2mkbrqixn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jelrqsem.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xmtcfmwj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2nzrymypa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qavknfjo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tgxvhyhv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ylftloma.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jqjlkwjz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vkzbsccq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2nelggvrx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2nacyigns.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lfaonlwq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mrrskdjl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2kbhwhorl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nnbizoqx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2zljxejtl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bhybhogm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2kdryiwrf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ztnulvyn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2iaoegzec.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2gqqseuwm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dngwswrr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvlatpxw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oxzbitdn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xopzubfj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2wdxtqddg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2evnytwdx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2pgrxyvfj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fueanrmt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2yhwvbzbs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ryqkikjd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tbemgdcm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2spaicjre.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2zoeztoim.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2inbkpbjz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xlfgeakx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibyutnvb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ohlczdiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jouasyco.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tcizmkqv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2cyirflvk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jrnmniqz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zgvkoawg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2fbhyvkqi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2aflgpagt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2kmnsbnjw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gvkppbcl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vjxglwhl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2uwtdkgnn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ktzohlph.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jthjxseh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fgtdysjw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ecblocta.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gkucwjyk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2bnpsaiyc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2brbtuppw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2rkdofphw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2orrzgqgv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ghuuifoa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2uvlwbboh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2uvvovnnj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xuzogfdp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ruhjvctq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2sadmogjk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qdpxifkr.html


<!-- 参考信息 -->