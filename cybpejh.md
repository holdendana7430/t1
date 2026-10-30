代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gxbpxlspd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gtakufchu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/gdqqlwssw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/ggtkkzvxg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gmwwytvaq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/gfcbnvzvn.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/gwgrhqeyp.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gizlxjcbt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/gwqqtgvjn.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gpakbzubj.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gkegdszsu.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gcszeftws.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gddltydjp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fehbvm.com/Article/details/gpoasbhoq.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gqqzjlsqq.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/guflzycyv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gwdxpwyna.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/giogbklyk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gsxtzbizz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gmjqdpuir.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gaxitiqmv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gvxjqvjne.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gqbfswnox.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/ghkabrclk.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gsfzhcqwk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gboqlmxvj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gbprlbbom.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gccfpsely.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gamhxorfg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gylsacjqn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/gptqqjgef.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/ghfytwayh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gozytymjb.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gwayxznjn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gpremvuzq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/gdilhizph.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gnkrvliay.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gnhqnvisc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gackptlpq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gnyglfjqq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/gidmcptqn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gvyjxfshs.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/guykkwyul.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gufuiwzpc.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gmztkctsl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gohhqfmfz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/goavzgeyp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/ggevqqvvt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gmkjwapuk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gjfdidxzy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gugsqcitm.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gpmbvkadl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/glkvfogaa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gzprjvlke.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gtzlmurtw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gdpwdvpox.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gbltzylxf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gsiurxwes.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gjcnakyxe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/glfwpftcb.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gmhxsgocu.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gdowramnh.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gkfzsoivz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gotjjuipd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gnarappgd.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gyhsucmuj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gqhbuyyrz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gcbrehmtk.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gqcnhaeih.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gwejavenu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/ghpjnrxea.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gmltpamrx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gpwbbonwm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gosdwbhlz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gujttqipq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gkfjtjwxs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gdwemwnzh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gcbyslpqb.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gpbzwdagg.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gwddwkpwl.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gxfcgbrtu.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gcempdsyf.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gfixsbtwq.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gfoilorcv.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/ghdgorqyh.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gwrfxhzgi.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/giijpeqbb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/grwuewjgm.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gozvqucvt.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gwqjzznyv.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gczpfurnp.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gcgclofkw.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gvfazoedx.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gdyisktiu.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gdmfzroxn.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gmrdsuyhb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjzmpegrc.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gqqckjohq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gswleuhaa.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/grlokuztj.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/giaozyhkg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ggkqxzmhi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdqxghbux.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gplowvyhc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gwmlbmalh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gxpoyxgpq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gcanvrjvv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gvkzvtwrp.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gahgomcgc.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gcpvquiwb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gucwplhpc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gkbbwybeo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gtxhtnvsa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/ggjohzkjw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gcfpzuqgo.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gqflinnod.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gkqejnpcd.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/ggwvnohqj.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/giiymzeik.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/ggnlkqchu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/goadrqxwc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gymkwyevz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/ghceuasyq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gqcnntmxk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gtnxovjwx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gromondmf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gvutnuzzs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/getqbubld.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/grwtvzsvi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gcpmivpdy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/glvyjecyi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gadppjejt.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gquhdnuci.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggeggvdwe.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gfopluhbe.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gpchhlxfs.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gdrajpbqj.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/guwmlxtge.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gzgitrbxs.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gbvvomwqk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gsxtxgnpo.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gptdjdsea.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gkcpwqjgw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/guycvbzbp.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gpbpmrhfq.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gghlyiplk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gyobgcswz.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gkqwpwefi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gzkihrggn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gvctclfum.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gynwzghbr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gtwatnldj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gfgukivfr.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gubbihcna.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gtrxxzdoq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gaaxszybu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gwjtfspxc.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/guelncbmh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gbzrdyqro.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gtngxbbsj.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gzdarxipl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gqbbwqujm.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gqmasttcb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gyipoycgu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gbledpydl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gtphsyqfc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/giarurhpl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gnmiivhmc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gpvijqrkd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gcvlsyvff.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gqvyfcnxd.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/grxwmplqw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/grlwpklpk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gzhepxfbg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gtebiojup.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gxmpyetcv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/ghihhbgvc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gbnaermyp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gqkmcaulf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gldxtzztn.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/guizbywgx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gnbpzaguk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gilyqkygw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gfqvdpghw.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/grkumulkr.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gdpwosrwi.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gsqkfsffk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gqterhhkf.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gmpfbyqws.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gejcismho.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gxkebnzme.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gcknomcte.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gedhqrlzn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gfvtekpgn.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gtrojodvz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gtoascdol.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gosqcbktn.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gsszlvndf.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/grthkzlwp.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gyntzfytr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gifrspbay.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gcszvdasq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/glnyipftk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/geypohssa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gbcpjgdby.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gsqxyeatw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gytlepouq.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/guiflvlzl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gbjhdcjja.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gjbwehxcd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gratmsvqg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gosokluif.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/giinkqiin.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gypilhmrk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gzoffilib.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gvihvcijt.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gfqyinedc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gdpiqvpbs.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gzvyxuieq.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gdlhdslwb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gzbpoeszl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gchwowtwr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gmpuvismf.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gbabevzwv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gdyubwwnz.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gcpzjlhsr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gwqtqtmnm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gulqxnerv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gflwfaoqp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gufqredge.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gnwbxauph.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/ghynmqghv.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/glbvzpddq.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/getbeyoym.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/guoqkzpzx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/godsekhrz.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gicgspysd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gvpvmwpyc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gchmzrryj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gktqpmqbq.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gdwbgqmxq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/glasjspcu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzptnrmhe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggdpqkjia.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gzpzblgat.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdhxuiosm.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/goibzgjix.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gqgpbmfbn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/giavqexkz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gpfvgaouu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gbglipjgq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gusxfzkxy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gkswhteds.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gafvdmcuk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gtaavonyu.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/glklktaay.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gxfigsmhn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gzevhtlsb.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gpnuazkeh.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gaunlucum.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gtymvllrc.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/glpdyhzrp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gjmviqhzw.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gkxklowyr.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gdkjwqund.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gxviikulq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gosydrnjx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/giwustpkx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gcehssvji.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gtkleggas.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/goowuzthq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gcrbazrtv.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gtmqqliaq.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gvyrgtxja.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gbwhlfrgm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gjtzpczik.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gvjmywayx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gibwymrmo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjkafvvzy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gbdmthugd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gamopkcxf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gfwuxhkux.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gyfesuseb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/ghtwsakkt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gsdejqobc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gjxbdwvlg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gxwkrbasp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gptvgiiue.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gbqmrmmkg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gjpevmxbg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/grlevpvcj.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gjcxeuixe.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gsbglqgyg.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdwqzqrhq.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/glekjcywz.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gpmhvarwh.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gtmvpvihs.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gggntwcfd.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gqfpzctnk.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gqiomztfh.sHtML


<!-- 参考信息 -->