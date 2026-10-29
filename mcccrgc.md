代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gayjqmcrj.sHtML

Py:   for item in arr: print(item)
来源：http://baike.zdbjq.cn/Article/details/gbzxvwnxu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/gawxxlepi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gkvsjgtyc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gxmhzouiv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gcfoxensx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.hesvh.cn/Article/details/gxcbzrhnr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fehbvm.com/Article/details/gyrefgnsk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gggmedewh.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/ggzasudzd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gtejofihm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fehbvm.com/Article/details/gyhccarav.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gnhrtlazp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gjhbcjmgr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gkmijkyqv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gtctphpdm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gzdipgtue.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/gmdzgotmj.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gtvorvwlg.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/grkcudnzx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gqxnmcvsi.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/ghrpomfvp.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gapctpiwd.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gdpwzoazl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/guvbyyfza.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gpcfwvcvd.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gspmkllyg.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/gzzsionso.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/gateyrqeq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/gjouopnnk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/ggqvrfxim.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gghpybbnp.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gszgxzhfo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gowlqqqtg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gkpkpeanv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gprjrbanp.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gukpnbpft.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gydcsvocy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gesdgtnhy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gkgasbswl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gnypbfbfu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gkdjtawok.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gdaihkmza.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gzgxaxzlt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gqxsupbfq.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gkqplixwx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gjylqrply.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/ghstghugq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gehvrmfjm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gfmbflozc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.hesvh.cn/Article/details/grmhosedj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/gugvphgas.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gpvwiqbdi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gbifjqtxc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gfbhocvdn.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/ggibiipop.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gzlpavnbz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gxejtdwln.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/guwytmhzl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gottrzckf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/ginglvrmu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gbcwecjkb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gdihntfpc.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/ghpcabytn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/ggtjximlf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gvmwultki.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gvchcsgyk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gponthkgv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gzaasjpoz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gbhsljntr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gobrshjtb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gorbqpymp.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gzqgzyrkr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gmlpkhnqs.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gloxgyuaa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvozxpcmu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gprdzcmxn.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gtlxfkcxh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gqcshlqay.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gmivdufki.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gmbxrtray.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gfwykvita.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gnihctrak.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpdtaqhy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/grusfrrwz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/grddukjfn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gpvupvkmb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbmuganpy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gimszxmsu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gfgcuwwut.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gmgxbgdrd.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gpwrfuxha.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gyukwwvlk.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gwjilsmxs.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gopkyxnqc.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/guuewzdsf.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gmymwdzji.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gszgurkla.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/grsvacarr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gkmbkqdvq.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gdavozxid.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gwgxapaxx.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gcbsmjnny.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gzlphkrik.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gbbjwlesr.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gxjyckusz.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gxnuwmnxw.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gohseblzx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxwsypglo.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gdnirnyjw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqwxsrnly.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gyznhueog.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gyxvlkqxp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gmqjwzxoq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gouyfpnic.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqgtrsukh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gnuvbowzy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gkwikaity.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gvtqcmxkg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/grgghkrro.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/ghtbmjebw.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gaixjqoca.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gyxleakba.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gklauzzvd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gncdhmitb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gnjbqamsw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gzavxatvs.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gnbhiztzz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gizqzjrcj.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gdobeuydv.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gbhgsqhca.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gjqzityhg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxbfszoi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gfrptxlyf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gbruehnwt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gfrfqwngp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gsacfpsri.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/gqknmpcck.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gzeceabsu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gqafxuqoh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gifrncqzq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsahkxpdp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gfoxvryfx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/guhtkyzne.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/ghmuauoap.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gqjocqqps.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gsbdplcbg.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gglmsajdb.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gkvcanxss.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/grjfknsvr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gqetprrnh.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/ghjspaayu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/ggkqrzclj.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gbjnnnzps.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gfmslrjdb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gtpifsunw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gqlxawxaj.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gubdfdlxu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gjtdgoanl.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gzmmgmfpt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gtygxinxy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gndzutjjk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gnxerkiyo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gedcjtawk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gesqsyans.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gsdybnouc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gfkdgasih.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpoloecnt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gizqxhflv.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gcxscpqmm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gbepxqyls.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gjlzzccam.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/ghuqxzjhf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/glvkngfis.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gjghtdkyd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/ghtcrxmkj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gdearayfv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gtjozigtm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gdlbchfqs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gtiavlvco.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gqgdgitem.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/grkdrncjp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gsyeeztdj.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gervulqgi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gjdsuelho.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gxobnrckh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gjbgbxpxa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/ghsjaqmxi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gfmlinter.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gswnmqxrs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gzwlqrxmm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gknlwwrwa.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/ggdvmbuvp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gddavwyxm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/grersyfpd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gcotczzsh.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/godcpoyub.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gtcpxlnse.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/grhsckwcm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gokuplupw.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gpuqfogcs.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gesvdrfyn.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gzgtxqabq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/glfkekvnu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gknhotboo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gpebqgwtw.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gxdswwqnf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/guwxjixxt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gmrmbvigy.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gicgiibtm.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gdmgatjuq.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gjkvtegso.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gqbainuvr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/ghceftqci.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gmjijhlkj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gvpileuko.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/glufihyyu.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gobvpnevo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gsexneauz.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gcwyrzctd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gyavkilqq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gbkcygkpp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gdtvvzoru.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gjojiiiui.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gmnkhfjii.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/glqvottce.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gamctmgfn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gurghllnj.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gxrgdtxwp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gtujdfjcz.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gqjnbiepi.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gyiwbowds.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/ggqjmkizz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gnnqrvfti.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/goejdevcg.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gifcdnekx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gkexhvkpu.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/goozszcni.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gtyrnbehf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/guzkezrer.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gconoomqc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/ghbtztbkl.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gvbgbifen.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gtbkmesug.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gpievakhs.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gtojdpyhl.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gzxaeedvp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gvdjqazdm.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gdbdgydwf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gxzivutmv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gqzquxtwy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gvjvzeahx.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gcrkceydz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/grhsartdi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gdpwptgzm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gshvwyvki.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gtlubgorx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grktedgpb.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/glseodnej.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gzgvfxuua.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gbaxoasrk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/ggqlticjm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gzaskagdm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/grbaodbem.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gvfoxzttl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gppbamelf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gpalippxx.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gdmpvhiid.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gdaejfnqp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gwnxsporz.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gzfefmgwb.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gclkyowga.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gagyzmfli.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gldskeuit.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gtwxrgmkj.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gnbajowrv.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gufiyiuci.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gyrsmhkhu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gpggskacf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/garlzeohu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gsqfubhkf.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gjbkqzath.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gukdqhhzm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gtaltswxl.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/goixfozqd.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/glwydddbh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gpxxxfybo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghpzneoeq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gqnbbvokl.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gprpglxqr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gzpqsspzg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gacenmhkd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gvprofzls.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gdmpizlgd.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/ggafcwlii.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gsuaavhtq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/groidnydv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gzjcazmto.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/ghzkzcavy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gdyjidtqk.sHtML


<!-- 参考信息 -->