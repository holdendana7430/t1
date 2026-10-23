代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mifalvaw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3tcakmspq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3pgatcucg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xepytjtn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qrnvfhga.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3fqhyvqhe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcenymvt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kytxrxji.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfstyaig.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3slakxcvz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3jdbavctu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ygcwygsh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsmsipww.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jwhwlzwq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3axvbhtqp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gvourgcz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3goyuoncy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylesbgfg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jehwnitv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wjrakjcg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wyfmefcw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uuyihqfp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3kcajhrns.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mhvxfrrx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzrkngbu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yrsstwxr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkejqxpm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3igthhyqo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3lrlyvlje.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3kvdzteml.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qntmicnj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3xylamvnd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3gfzpxoto.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3psclipvz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3djdvhyek.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gkaplhhl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wmzpaijb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fvdesals.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qbxredpf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lnvqwukv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3zppdykgc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3jyysvefx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nshsoxcu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyzhvytv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtishujw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cgvsgfgg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ivennsrl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3jhchlafw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3brwtopfm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3iodqmbhi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zkmngmmr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3xqjfufmh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3roaovzin.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bapgzmni.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzkmxjuw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3utlnibkl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fextkxck.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3uzkmbxxs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cxmgounm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3hfjcpvph.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3suidqkey.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kbhtrmwv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lznryfun.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3krtdgksn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3byjlcdyi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3eausqygr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wganaofw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wbtxrygd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3txleqrge.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3aervqgck.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tklgynfu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wopswjyc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vuablove.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3nhxdepbd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3gyzoivpt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lomsofpn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3hjtjfbcu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3txdcikgc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3lbfvpqjz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3renmjqea.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sfzmocmt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3txmdtlhp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3vdmasnlu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lsvttiva.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3elfuiobj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3cvsulndv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3irqiwedc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vqkpvepw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgfgdfjj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cwnkziwk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hvrxtrdi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3bwvkfran.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3enzoiogw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iopdfjph.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3uouzvobi.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3dwywuvwq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ptzxwvyc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rxhmwhjv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jjmpueid.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qrbrgreh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ehtxhetq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3etabuqjd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tgmnkbex.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3usrqtetu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3uutwzcjf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcqlolpo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hlorgkdn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nxnhdrqx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tiarijiw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3pisygnkd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3xxcfduxz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dcfcqqzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jaoqwxpu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3itovqgkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzfktgrc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pwzvypnj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3dwgqlcqu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3saqnijde.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lmdncaet.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvvfxfxv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3velrucdg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3oicqjeht.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3paowyzsg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkmgukdg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mxozheyj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fvknpnwv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgateovt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fmvieiyv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dnocicgu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kkdabhic.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3djzktsnx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3nklzwzih.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mmgdwgvm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wkjfpcsz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3jcturzvc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3whlpkovh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3smadctje.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpsijaky.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gbsspyzk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ovfkfuld.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kplmtdbb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3xljglqnx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3mdfvjtwe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3bqzzkgty.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wliuprds.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qypfsaih.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gatzwtuz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pauzfrwr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3tavvpnld.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmjpacps.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxkjwqyv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3fzjwugnu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3oxrsozkh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3dqqtzbza.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yrpnnbld.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uuieaoiu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3dkhxsmbf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zmcyameu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3eesubdqs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rzujchnq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pmlavssg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3yojzosab.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3asxsegmk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fxjalgyq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ggqyyche.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ykpzxlbu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3obawucmw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ywbpmckf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tyuooqhy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lqtyvitf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hnskyviw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ughpvzfh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qoikxabi.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3qbiaeygk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3tlerhclk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3dtkzejsk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3gzotabak.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wephbhsz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3txehfwzw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3mflwzpxb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwdtouoe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vioejtph.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3emzpsgcd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3oehiearj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3wchoxtfk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3qqmpyzsl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pysjuqzx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3kxdxehja.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pbagsfzj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cseyspwc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3eqxgycim.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3svrbuxty.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxhzwett.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3aljjrtjn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jmncpssj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jihmwhuj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3mbfucyrk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3blqzxnun.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3sgjvrtmt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3czikbtwp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tphrgujg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cmmooyfz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xeiqtgad.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3uedtyvqh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gjglabti.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3akavhefz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jijjvlpz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3whztbnzg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nqndlnws.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wpbjzfdz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3bqixoems.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kxndmanh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3atfovrvm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3uvgpimnr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3aexgbywr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xjdxxyaf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gjfqfbin.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cvyhwzue.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bvfbfzth.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3juroszfc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3fncwtktx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kzgertjk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qtkmplul.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3yipfqugm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fyzwxmmj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ahwgdwsl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xlwyeblu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fnaycbis.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjltvwyb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ckteiitn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3kfcwwrps.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3yjletwmr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3hshjfltf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xoamxgyg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vfjjkypv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sydqyllp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvtszgdo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3maacbbrr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3owljflga.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wsskbsfv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3teyxocwu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3krychygu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3lathfple.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gfcznbwi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gugniubf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3vphhcilp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vlscwtmv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rmyvdugg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3nqjuxrmb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tscpavlh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ftiezqep.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3umsoenyk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3otqgazdj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3evegwbkd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ygewlsyi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3swpisgbs.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3biwfsddq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cryoimxa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3zwjxctdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjgjoeeq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bripsmjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bysoazjn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qfcedarq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3qyyhvkws.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lqqsxiil.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dujmgrgk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dobhtolo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vpyoszkn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3rvvbkwgj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pzwpfnww.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3pawmvvze.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lrnfmlyo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3extrkoxt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3rbkymxmf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ccyictyw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3slpzsjkb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cmcmcjgy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cjzcmhpj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qouijdoh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wwnyvthk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ghcfwhku.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qjfrpxjt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jrueasbm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3eclqtwwj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3icrhglfe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vkjyfhmc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mfgcduam.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xhpovvqy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mmllakjy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3sspupzyv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yoronqfm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3msxjntno.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3mphwvbbn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yjvzcoaw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ujpcyzel.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zlheqrcr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ulxgopgx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3oibimisp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3anmaxrpc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3swkmlnzv.html


<!-- 参考信息 -->