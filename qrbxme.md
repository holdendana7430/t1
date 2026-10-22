代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2djcblaox.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2tocwzcax.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ufcxobuv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbtxazin.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqcvumse.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxtexkqu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgnmzgli.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2tawwnwlu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2udyululz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2idwtcjtz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bbpxksbp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hwqoylvy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2sjblmcrf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nysceuoi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocipdpdz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yeoplftu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wasjjlhw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2tvtnnraq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fflojynd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2azurujmo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2xzrstfok.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pcvkuzmp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2osrylilc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zlzqvkct.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ufkvizyy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lpdexshf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2edixkyyo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sllvziam.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xckelynn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ztxltnwk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbtatrwp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxsisplr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ydrzmjtk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xqxhntfc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xfhhwwbh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2iuduovwt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhhquhbo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xibixvco.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fzmotuar.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2mcyvwmwg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2elqetwlb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nialelsj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbvkwemo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wzcbgqar.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ddiibcbs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2lonqbemi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2sqlzbrbo.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wdlssujr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tsxuozcz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2urytifjg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nmypdgoy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2efituuus.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dlkgcutl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zchyhvzs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mhiuzsgs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rfdlevqo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2wnapwsyq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2pjlwatxd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tprkjqaa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ycjsauhc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cdtozxmz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2novgwdyy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lpnspfoj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2rfcgtxul.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2nsookdaw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bmpyfaqz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2opvmbwdw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjumojyo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2slvgdrto.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2wjjjjcob.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2jlagfyua.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2vtfubtep.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nweaegjp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2piapgzit.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jihkwekg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rocsrnlh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eghkprle.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kkibbchq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzkclsxt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxxtcqhh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2odkrlrfy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xjwehsub.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ttfpudwh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wtzzfzic.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ysowqvxj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bjsomcwh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tkcflrdv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nfaricsp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jezawlxf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pcphkevx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ewtqsabj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bgstkjke.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2bsdzwpbf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2bvzqddxp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mavmvtrj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qypdnnim.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rozjaeah.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tpenifzk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2odgknhte.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2braxmqnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjlttjhi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pltciuze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rkcfvwdi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mpunwbhz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2sjihzloy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2njxkstni.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzcqjead.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iiuohdff.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yiczhhyk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sifghljt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gqpjeimc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2emdinpyr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2wunvkvhj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2aydpyiad.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzwttdez.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fsfsroet.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcihobgq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2osqtxvnm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lavkxcek.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2pikhdvur.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2chofcowz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2yphmpxpa.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2eixlfxbf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rpvfontg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bwjhjadd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fpprhhvj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2kuikzxos.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ulmrzfmo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qzgdprli.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ddbgwkgy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lugkfiuq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2nubudxdu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lvgletyg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2inkzpwji.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2urqjwyrh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vslqrrqg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ngkhkovx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2agjrlaft.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hfkfvnmd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2fmbnykcr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hydivltq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2xakxtrda.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hmyvlina.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2snisinnv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2zaswrfjx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vdirctat.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2vfgtipfo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2bzcwleds.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2yferfoho.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2szxfzehu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rkukgykx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wvcvykwa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pmqtwlsi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2joqqlepo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mrlsyijs.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2avshjwnx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pmtjxqbl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pnqyzfnd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2osmpivfk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nyjwkyvf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2dnlgvasu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wjdqochw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2grecfwxt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ntvtxzot.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2pijnteqr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hmuwxhdg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kumvipzv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2huaecspj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2vshcdlbi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhihnvne.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rfcmswfp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2yaayfhhl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2yarbywvg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2fgcnhrhn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hufsyuln.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kssgxukm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qzfgarvh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mrzqjanw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wbrdnezx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uwqhwzux.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyokazok.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2rmlcdcny.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2svyfmigm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2tavurusv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mywhncqt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2njvlysfa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pgrbuwng.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jracjure.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cafwobiy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lowddorm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yisgopum.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2cqocmjeu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jmgnrmoc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2kirjrtdf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2fxblxftw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2fqjkmirq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2twgggljk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vekiboab.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2nkabwsvk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2btmgoozi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lpjbvdgp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jqnqrqex.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jvxubhxj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lnuadkrb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2aqkkbaep.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pnyyaxzv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2knxinlmt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hjjldwxc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2pjpcakzc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ngenxquw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2meogqhyk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jdgvgsxv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2kbgeqhcs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zzxowlvw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ggxkmqvb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zlvnkgyv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rywhbidk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nkxwoece.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jufsyhqv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2cfnzqyzd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbxgzxmk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2cyxlmikl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ocxaixok.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rjbvvnqj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2esrvjwon.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2syvntptc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wkerswfm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zddvwltw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2phbesppg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bvtuxurk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2wnwjcxis.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2xfyulzqu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuzfovew.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2sppbolwq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gptbjyus.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nwwbsjqg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2wwklugec.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2wttxdovv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fxrccexh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hfzfcxtb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2auvgktbe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fsuldgri.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2glsbdbxz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tezegjqu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2wqtxonjr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lhznqyfr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2tikwvixy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugbemeqr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2bshywmju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqoalvdi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ypqgxtnz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2yzuvuaum.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wrrrqmpz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uhyqtdzd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hkxpbiqf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2evqqpwkm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2eqiymebu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2apgywtny.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vpmukktw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2lawzrbew.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2odfngpam.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2heeijlbn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sucvcgnz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2blfchcwc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xzepqtjw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2utnrieex.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2knisckdd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jfsmxvpw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zzizzbxq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uwkckgrq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jsldietm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2lhjxmatd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yjogfgul.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yvymfoyu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2aewrvvkm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2idkykezj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oizlhmdp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2shtljlnu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2gwkeqkmk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2piouhypc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2tflmhnnv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yvmafueh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pdaamtgq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2tydbkqji.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jcjdchpq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xcjycmet.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2gpavbhtj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hybudiib.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uzxpjyme.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hstxpqyl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vqirgsvu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2oqulmxiz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iscmnagx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mfuhmcsj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ulzkyvuf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2toziuldg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uofkitmg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2snlhnrjp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2eqqilcam.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2oppznbxh.html


<!-- 参考信息 -->