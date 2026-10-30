代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gmqfwfhar.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/ggpszgiou.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.zdbjq.cn/Article/details/gzzbnfaqb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/gaszlwhmm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.zdbjq.cn/Article/details/gzplrislm.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/gcndncxsb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/gzumpgtkk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvxiosgbc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gsiljubgc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gdqehxohx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gjfenmfds.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gzutdytvt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gmnxaacqu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gvizgsjsc.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxqhlabuq.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/glkmnqgqq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gqjmnfxek.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gibftfolu.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gtuqkotqn.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gnydqifgn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/grmkidjjf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/gongzzbil.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gsmcaktyf.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/grsiaakzp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gobaihlfl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gwjqlllyf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/grhyoeozi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gqjzfnotg.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/glpcrwnos.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gexiticmv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gqgaarghg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gngmnsclf.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gwctcfvqi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/gppdkmmeq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gjpwzfytz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gwhdhucmo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gehivzpro.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/ggayjbqsi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/grhimmtfb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gzfigzjyx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/govnvmxqz.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gpdymmkzs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/gddgqhrej.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gnblpyvrq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/geunfkqcm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/ggytzvdto.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/gjmstsbci.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/geccasksw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gygxccuuk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/gfcnsjdhe.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gtaewzduo.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gyjqxrbev.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/gnvoicfpm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gxaykltcj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gxkrwxwog.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gsekhknzo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/grzlnftgo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gfwgmgfcm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gnwwldnnv.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gcwvjpwoj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gqbbehilc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gcuwgyvku.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gywgcgjtl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gzrslcyko.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gubmaqneu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gkskuwyhk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gipjplrux.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/geerdhaxd.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gmfpmaabs.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gsxmqywwp.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gxcpwwigh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gjbzarquh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gbjyfeaqg.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gszggciyx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gfzrqkouf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gethrzilq.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gkgzgcoex.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/giskgibyf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gcgvfozmx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/ghgrjgsgy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gpczxbujq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gkfbszxpr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gfvgtgrpa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/ghabpfujn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gjfywklrj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gynwhhtew.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/ghadcxqts.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gxowjgfud.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gxyswxtya.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gvplljkly.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gieraejhn.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggyfzvlcx.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gcvnqxtpj.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/glvhacutx.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/guvstopoi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gsfotyqrl.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gfzhulvmm.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gyaxblpus.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gxxymsrbb.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/glgounwdk.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gbizrvtfv.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/geqlwtcsn.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gruxfpnyn.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gtotfstci.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggqwpdwzh.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gkgyygwzz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gibaljafh.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gtqskqwux.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gtpwtlyyi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gtxuhpaxs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/ghcutnkmm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gevlgztqq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gkyaugzud.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gqjrxcooj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gokbctugh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gkbgqpomm.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/giqljemol.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gydxousuv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gjnupjlun.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gaxqihkba.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwessqkfk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gdtolpyth.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/goewpylcs.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gdnorfkbh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gmcdqsmbc.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gijnuldzm.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gpfkivhpl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gjclmkjgo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gnisixthn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gudlgdeeo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gfduqqzvd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gdgihyjvz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gdfbqcqiv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gewryvmux.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gomjumbrr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/glvhhggis.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/grxuutboa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gknjvivhs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gchazurnz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gzrtkpawk.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/goayxuvtw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gvvezzqsf.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gnlsnvduw.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gcygbsvcx.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gbvamqnba.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/ghtwzfsjv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gdrcpiqnp.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gfpnfcyob.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gvriscmjc.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/ggevkiwtk.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/ggtoxfvtv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/geqzvlqlx.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gvewsbnyk.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gdhhiymws.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gmiuqwnnc.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/ghelabdaj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/ggwaskwur.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gevimdwri.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gvtrmxwvl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/glloklzwr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gqugnlome.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gcjnhukgp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gpwxjmnzk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gdbbsjpqm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gdykchxik.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gjcfhgllv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/guxjesjlz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gflcrmdnk.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gdeeetcnp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gfnhqrnei.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gjhvzrstu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gurjqgpst.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/ghvlydism.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gmullvxnx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/ghgrjiizg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gpvzoetjv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgktemht.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gamtrwgtz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gfvyzmxba.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gzpshpymf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/giajinxrz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gvfercvix.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gsepivvax.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gxkcyefat.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gmvvkjqtt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/glyfdgism.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gndhpbqxy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gbvovszdi.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gaghmqloa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/grswcqeur.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gtgyblzyg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gmqfnarao.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gkzlfwhdh.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gwelcaxrs.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gmpolqgoo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gueurrqbo.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/grzsfgkfs.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gykplzcjd.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gquaewmvc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/govdaftqr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/glefpzgvp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gsokzwjus.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gkzjunvwj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gnknfqsop.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gqtbhfrdr.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gcbwqlbqj.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/ggrsphsis.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gclwdlxtq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gxocnokgj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gkmuzivtg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gykorakoi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/glchftprk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gllrxkdnf.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gfujjuhpz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/ggtrbvwgv.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gtzquhwfs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/glcatqrwg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gfumnwtzg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gbourpsbs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/ghvwdltcv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gtqtmdlyd.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gwsdajeej.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gyocebbxz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gkhsgxltq.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gmkgukfss.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gaklkdsdi.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gcczmftpe.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gfzaijemn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gajvryhcc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gbarcjngf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gnryhmqti.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/ggovsjoka.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gtlvxpqan.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gopagjveh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gvzntedpz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gcylaazib.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/grfxxyoit.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gxrzrqgiy.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gfueoeiay.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/grysiyyod.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gyxzzhgnr.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gmydzvtvr.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gebmlvmrj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gosrvfjbu.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gkmswcykw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gnpvluzxw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gfaccsyjd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gffufphbz.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/giejclqko.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gwdyhjzoi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gddkwngav.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxkrtxcmr.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/geqafyewi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsrrxyrec.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gysfibeno.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gaubdzryl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gzoltkfgo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gjsjytwiy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gunaatvcy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gxfiglxkd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/galmofsmf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gcknradue.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/giplnvrvr.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gyxiwwytf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gbryovcob.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gjlzcegmz.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/graoeluxi.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gybcsaotc.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gnrfwwskf.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gteblntvb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gmxbkklbs.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/grbeigadw.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gcozmbidg.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gxrvclncg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/guelbdvwi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gfbloxbsh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gwtgaupdl.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gyubvcljl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gphdkhecd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gwxaoouxb.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gmkkkaedc.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gpmsrsvar.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/ghrmgrfvo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gcxwpkvfy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gdoigsags.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gdrpylxgf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/ggmsrnvul.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/guncxraty.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gmglwyeag.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gxdvedphm.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/guumuvuab.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gxtwxolzt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gvsujkpwu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gbqgyciox.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gvyqmjvwu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gfaxnixgy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gwopiptah.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gqwljxjqr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/giremepux.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gdbshxyls.sHtML


<!-- 参考信息 -->