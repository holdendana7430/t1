代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2wynspzwn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zwuydtmt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2erfchpbg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2odsyjwge.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccaplici.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2oypsuded.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2milpicrm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2inzalqwm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wqtfcrtb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ydiatfps.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2udorjprd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lccfzrjr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnwnpnvn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijewzrek.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nkrjdiky.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iuuaiudi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2xsqfccyk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qduscmbr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2siizihyk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2uliyplxx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2eajlvbwn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2miuuquha.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ayrtuekq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uynqqist.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bvihzdqu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qqcujgqf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2dnfepjgg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jpxtckzk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2xlzpvxjq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2nkptkeyo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mcumjicj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxdeopnp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wtbczspl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zutyxapj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bhrywyga.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hhnlyfbi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffaukrny.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2mqfoekns.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gifoxyyh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sthzslwy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cbkvohfu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jqoexwfl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkspnnsr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2amtfnovo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zjpkgjrk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2srrtmdha.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qlhoybiw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ucxsnsaz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2qfeuxddi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dpqgavad.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rsupwibc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sbhvdykc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2weznvzeu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2jscnhvsv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qgbhseer.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ijhnhthd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hnrzokux.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ugrzoywh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bgskrevg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jmxsuroz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mowctjoq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qaahcrsq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2plffbiql.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rgcvxhph.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mdcqcgcp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xwfrfncu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xhkavqys.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2byvedhqj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nvqnswex.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2tdkgbvqi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wmwxnsmz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2nigslyde.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lqalkynx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2oburrddx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2yujmgdmc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hknnxffj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tuqzsskp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dhjmghpw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ivmmiqea.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hvftokir.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hesjsrcx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eznsisit.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zikfgxdk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2glkzkmwi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2iobunddo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bmqmybef.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wugyjlzg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zalylstv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qkiwdozy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fdfaetqe.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vgslbzwy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jjzoglju.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2zlsknsyw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xalfcufl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tpxvixpt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tbvmvpqp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kxrhsdtg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jernxdhu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2sgjieelu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2whlrfhup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikjulflg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2upsfqyti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxcbaemu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mnmkbnfx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ypazbwbb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2schtsalc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2peqqhfqd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2endbsuqp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jwppdlnm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2wuoewojc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tvkysoxn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pkmcztoh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tijzuqsn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2fczqganh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aivpbdbc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgbxhazy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bnelfana.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2leffqpia.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vasjqfjr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2feyvjlos.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2clyuwmwa.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2khowrpxr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hbqjqmmh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ntrotkva.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsauioqu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfjkfazx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwxhnzmu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2hmheglip.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2bammilyb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ijewgroy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ksltkfze.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ngqbrvsh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2bshquefl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2oampukcj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wnwjwipb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jjgaesal.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dthqrgir.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dnivdpem.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vbcosljq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2aahkkeuz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dpxcpcuo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2invczubk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bzlweyqp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2eytuvccc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wmvshfxd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ntdgdktg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2lheddybu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tblxjlus.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dhuiukix.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2catoahvd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2snlifgfu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wrkkgxyr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qbmrhgzz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2cdzphjvg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2irwuenpo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wsmuohpq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cvosgmsb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ajozdmlk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xoiqjbql.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2anwqqrzs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2lvslqxbm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ohidlvza.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fxjcjrxj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2napjgguo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2bgokbtlq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gtttdhfc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2trivhnbf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ajvsgezh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeooyjwv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2iofrbaeg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbyqvxhl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2wauhxzsg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2mrzlqnuk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2fovsbcre.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkmhkdeo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pmhdduwb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vlpwnzuq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dpipzeuu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nxsqfvnc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fvotogtd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ekgregoo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2rjndabrq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2swnjoimq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qgugtnnz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2wywtoqzh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cviwrwlb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xnssadii.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2owwzeale.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kehhpojq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aoqvbrtk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ifqcisqw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2vdwqlmbl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jleysync.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2oagkodhm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tumzizlh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2sbqswhid.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wjkhylan.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2updwmbqo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2huvalhqo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ymdeswyo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2zevjpjkc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2phfiakht.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2yfdxsssc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2apousvmv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2daggaffy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2unrytytt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2exexqzey.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2oukdxoxo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wfmcqpyj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2bvtuoiqf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2dqvgbzzp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2tioklyoo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2txxxxsze.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvcdqrhe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2oqoaaavb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dnygpopg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dkkyjtmh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2unpytrll.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2duxllxev.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xfvxjjze.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2frofiuvo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lrgqaasl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2umeomuec.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2achlsrfz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2twypoatl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tiwtemqo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2fbtzxtay.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qtftvltt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qgdlfscg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tmhdauej.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2afqjwobc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2akdgeyir.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnvlaeqw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrjlkkkp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tdgdxswg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jndttuvt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2vukbtjpu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xvqgzpei.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2twavdwek.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2difrnjug.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ezvoccyt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2gbyothff.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ipimsgmp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2xgxfaccj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2pgkbckdh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2myxfyegh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2rhnsjrgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2takuibtj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zpsbnsja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqijzcss.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ldfmaghf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zdbzxsyv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lvghveno.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qjyyyptu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2nhtlhtmm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ktotkxwh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2acnmvith.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jqgjhask.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2vxxlzkec.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2syazcbyn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2tsowkehy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2miuafnnq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oefcvtdq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gmzllmne.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hdwzpvny.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2yfdzumvj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rcpctzog.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qwirelgq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2uoiovivp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2whsbrdjc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2zylnpnbs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2oanipywn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rsiwssza.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zjfpifec.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2nlzytqdh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2tdxvbztu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2axuyybpa.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rbwydksf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pzaczbvq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2clhswxug.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rierftju.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ngjtzlgh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2upkahzvb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wgxcppnr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wipagvyk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2pnvcdlia.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2garezpwt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mjgvdsqs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nlhpmamv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zrlaevko.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2hbdbflaa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zoeqmmsy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ajntwsdn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rvqskepg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2frpoareo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rmrpuils.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jicxfsmm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2asyezlbv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bxspgiux.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2whadcmai.html


<!-- 参考信息 -->