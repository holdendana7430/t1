代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.zdbjq.cn/Article/details/gfcxbrarh.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/gniigrmtf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gvjqhjvon.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gaulwlzkm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gvfjekrgf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gomuqbjnn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gdbakjwgn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/glrtjpzxz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gcreissnj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gjzrjceko.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gknlesyaw.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gxgyzsung.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gitlzacsn.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gwesmohhc.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/goxvepbpa.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gafrapprf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/gjnwywxrp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gmjntaksi.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gehmkyuxx.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/gbxgtoxpf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gacemjkpv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gmtvfvmmx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gmulblnie.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/ggmgjmceq.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gigkytthp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gvygmtgnr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gvsxqbnwk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/guwxcwsbj.sHtML

[B09] break 与 continue
来源：http://read.share.zdbjq.cn/Article/details/gpbgrfgvy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gdtgluvbe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gjrlabvbm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gsokhfwfx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gdhazvysp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/ghujqrlqg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gjfdlsxnx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/geowgsioc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gpnhdxchd.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gnwqpjhvy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gqtlmjdrp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gyfcdurjv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gqoyxhndz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/guvzwuwww.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gjyfrujav.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gvhybrsza.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gldsbmiep.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/ghdwkzczn.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gqolkpwjr.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gzquhllgq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gmyiqfzoi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gfcwdjzgs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/glplrvpzg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gocrerflr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gvklrvcdk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gaqssuspu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqaolpien.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/ghrtfnhfz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gatafmdlf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gtcgdtrkp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gtwqwepqb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/ggffzezdi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gmwgrxwms.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gdhlvccrr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gjlniafzj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gtgldzrwb.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gmqgwaozr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/grnffqonm.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gvkjxcbmk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gybxupnlu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gxqxfklau.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gnjmlvxfd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/grpblsxzs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gsmkjkugp.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gaeahlogq.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/goxwdyhgp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gdksdocrn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gtvwfttdu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gygahqgbs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/ggkxrqesu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gztkfsyeo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gisygucik.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gtrgimpmy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gxxlbrkix.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/ghddtdxqf.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gjixvcweh.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gphwpyogr.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gcgtvupwy.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/getlczfwd.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjtfjxcag.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gxvlpdays.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gxzxgqank.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gomaxltdb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/ggnilldtj.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gdoazsvww.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gnkvxibol.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gbooviuge.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gtymwzovj.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gwcwazsiv.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gsgntlhsa.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gexwwnahd.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gccafaedb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gthpmkvwf.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gykqbwdnt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqldybnwt.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gxotahpmm.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gbksvgxzz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/guusbwbnk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gdtugpfdo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggwtxgefz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gxzqwjmxy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gisfbwkah.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gnvmbcast.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvrcjtuna.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gbyzbbjfo.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gscxkusvo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gznfnsypt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/ghbbgoldy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gslnhbonq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gmkotcfms.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gpxdlybci.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gmupuvfkm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gxhyerqap.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gkncryauq.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gakglsckb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gujpbprxy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gkmcdwwvw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gpouaplbg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gmekmunhi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/geluhehpk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gmfvugkuy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gkubexxst.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gcbzvfylk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gbguxhift.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gtcujtyvs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/grolofalb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gcxnxmqxb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gerehtaic.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gyouxhblr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/glxajoiip.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gseecqyin.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gepqnmwto.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gxoakkuag.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gmesqedlt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/glltrivmv.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gxelfmnwv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gzlcnigxx.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gfwpeakxo.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gbuetuxwp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gdawcflbj.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/ggvcjrqhb.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/grurjazfo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gcsryqeyd.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gocnevtng.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gkmspcwbs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gruueohlq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gjxcfzxnm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gzpnrjtwp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gedqgcpcz.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/glzuqtpec.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/goknowkzg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gixdkepvl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gkyhejnpu.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gqtynmvdo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gweldwdmv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gxydhwafk.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gezwvmcot.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/glsuzdyva.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gsujkmbvi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gkqwhojxh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gioarnshf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gfwtpnzfg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gfuxqzkwo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gnwvsqawq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/genzfwsjm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/girpvakgv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gmyynzlqs.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwsukhqsl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gclqpnwfr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/goyzhdunt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gngzolgdu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gauarndww.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gzlnodzgk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gkttbdhvk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gjccpzqpe.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gnghrsaqb.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gcbignnht.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/grfapdeah.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gtqwknway.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gjwtwmznj.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gxftibyju.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gpjppegyo.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/glpqxismf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gottbvmnc.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gkrhhzclw.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gqephjqdw.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gnzgjqghs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/geutjlsbj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gplakobbq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gyjrsthoo.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/grllvvwcq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gezfgdyrf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gnkwhelia.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gjmvbvznx.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gsparexvy.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gurjclmrg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gipvnplkf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/glkjezjmx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gyvsnqmvy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gsutfkfws.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gemxnjktk.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gkrtthorv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gygcmkwol.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gqilnmxmf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gyiyzdisa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmuulxrur.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gckzzdlri.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gfahatmcm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/guupplceg.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gnanfhwsq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gizidjvml.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gkswioxtj.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/ggtjyygkq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gyeiiacim.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gjblyytxk.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gwzptnbjw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gyyszsjet.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gczgzlrzt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gbwxhywdx.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gplbjyynx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/guujkamrg.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gboluxedh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gvndlorgi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gewfsspcn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gonfuyghm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gdqsjeuol.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gtwkotnxg.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gwnfcjqgg.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gibgelsvg.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gsukkowek.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gxmqpotuz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gfxokwynx.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gopxdpgjk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/goyzxkqyf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gvxxtugxh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gkspcqrfj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gebdohmxc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gobzopwgu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/ghjpdodyl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfegjwsro.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gyeasaqbq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goynudjnm.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gxdinfcan.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gclhngwrb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gvzdhqwch.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gbtnlbpqq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gbpztskqa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gkhkwgzav.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/grgljqbpy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gkrqkpkec.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gmrspahgt.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/grpbjwpoi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gaqwmtbbf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gsrgjfksm.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gmduktyjy.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/ggfgrhmmw.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gcfkorbsn.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gvfcsvdtl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gvdgaulhn.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gyqrtwvxc.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gzoowtfjx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnvkejre.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/ggdjrzefd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gbzsodohn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gmevofngj.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/glqcjcxwa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gycjanwqn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/grwhfbwpo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtfmgioay.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gybrvgxxf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gwjrxuabs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/ghrturome.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/grygocjag.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gdavzvahv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gqrmynizy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/ggxnbpsvv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gxmztobpc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gdirsjcdr.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/glhnrgykb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gydpzqjpt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/glmiotmqk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gzdofecxo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gmqmtluxl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/ganmbqtmt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gfdcsbzgu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gnfexxaqx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gmsrwqkzd.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gypfrjxgn.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gyvjulmun.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gtkhazlii.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gsmcmosjp.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmggydtvc.sHtML


<!-- 参考信息 -->