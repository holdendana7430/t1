代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lyvbbndr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3pdyrbdhj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3petnctxy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3eflrcejl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3skbkbuym.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfgyroih.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ellexttt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3srvsquhk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3piusfsus.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kzdlntba.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ydgpltcm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3suidqmti.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gejrzzcg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vehuhcvx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qagunigr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3xpysswnf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vrgitsmf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3kbeejxsd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3qlojugdb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fgjqsjps.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3hlqvzckd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kswunpap.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmhahrzl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ajtrtnst.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cqmkzemk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3tfhiomml.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gdyvlvam.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3glanlnni.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3laeqdbho.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jxeghqph.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fvumbipd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yjcnssec.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zcgsrlgh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3suachbic.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3zozxnfok.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jrspvnpo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jczksqoe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3yrwhdwog.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghuumfxr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkgmdguu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3plufptji.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vjawastx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3aflwdgmp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3kabaruio.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ausuzoip.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xqwquxdn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3iyoiggnm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxahjcls.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ftpfxhtd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xazkgasp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xfddkkcm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qnervsxs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3bxizfbsz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvfjflbq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3oyqxvrth.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3eclykcgq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xgvnltlo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tjlxgslh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lgfyljpc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3frnnhjes.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3stgmgrsu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3cobmppqj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3fjyrtamd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3duvdsvhc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3zoxmhdqs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3oviwibdu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wjgecdfs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uivnwvja.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qbizedhd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ydepqehs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3eswqaxrq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ginnpaqz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vzzipsaz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3mztoksgc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3eytbceuu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nylyqrqs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3eenurybl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3datafwoj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3bjwgomvj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3stfoonmv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3rvtgmtui.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3eneprhiu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3lvtfiiyk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3tlnqeord.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vwknkjub.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ecoqfpen.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tovjwhew.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3muyeytic.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nyniaese.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vxaklzoi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ydduahcd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xbasghyy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3dmltqwzm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tiveusns.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ktvfggdf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ufftetbm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lujhxzyh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3obowugzb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3brxkbswc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ozymlcvc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3kwbbtset.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpnutccw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wcyzathz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3snguqnhg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yufgmogq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3gnbmmsde.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zfqylxdv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qzrvxpwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfsrmter.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iljenhnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rllqyeub.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wigwtcpt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3olthbxnx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3momdxcyq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3arzxwxqt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vsdmifkq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aotkmzsk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zghligow.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3snxbaqvf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lgkcsekw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3fjjwohrn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3yizvnrgl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3bcgmtpke.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifghjhkx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nivmdkkb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3pttkbpaa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fihrabau.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3vknawnps.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3pvqubdko.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3pokzapaw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dqkizyan.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3bkhapnrl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3crkzdixg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dtiqepgz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3brtebakx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3yxvbhxsv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3odkwdbvv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jbohfpoj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jchmtlmy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jdbvkgqg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gvpxzekc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzcydsjb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rpskkrir.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3tpipnqrx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3iqavzzfp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3omgnostz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmbdhnge.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3czevchby.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dytbvaci.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3jpjqlfzk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3izngghqq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3sgdvnnnb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3sftoeoxw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qqufeqkx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3zodnnjbc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3havacvpu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pdiuofau.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3nclrvxtl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bzoncdgr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nsqvnvtu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mjxipmxs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3llhafxrx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jeuvoxeg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3buspaebg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3heftlkar.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ticvjukd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3pxspdazo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mlunmlkq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3jcbqntts.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ghwhobik.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nmoqdlgj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zjixcbpi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3jojioqss.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3eqyxjhbb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3euigczab.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3jmxponcj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gljawnnp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gmclwczg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzbxxrtt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zcrqhpmd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jqfjzeoo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3liztbvpl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3epumhsfw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3kkkoskpz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dkobyniz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rzrrhebc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lcofmziy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zeyjvrvy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebxaedcu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vewuegqd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zygtebhr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3hypanfqd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ndbbeodt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qdmzeyet.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wfcmbmws.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3iqrfgvdy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3syqyezma.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zzvavyof.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lqbinvfi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3uohuvnyz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3csuwozeu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3uceuakab.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ujmmfkbu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ifzufdop.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rxzyryqv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tvczqewh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ctikseuc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kpebmlkt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3oqgxuzwm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ozssejdg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ofbhidsl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3slkhctjg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zcmrmysx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xarqndvg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gbhgvkib.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3oszwhvqd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3mowfufnz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jbowuxcl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xgemoafu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qzntnfpn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3fdxpsfss.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3avrsjuym.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3hhkfkyho.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eewbatss.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qdxtvcwh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3euzjarjx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ohdwznkc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3rkaawtsg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3toysrblm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3yahzbevy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3skonlsxj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3soedvbex.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpjkmlbr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzuibodu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ishgylmr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mkbnbuos.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3wcdrdwpw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3nascvtvw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3dmqoydgj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3pbmorpia.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvppudue.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iofmvxvb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lvqulpuc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fhzrmxty.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zrzjlwjt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3adyuybwt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tunrfksd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3idgrcias.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3tnhztwnn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3diqreebh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3dfejthbl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3dwszgndf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3naqtudiv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3hpnoijes.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3blbqgpzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qulofptj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fhprvlua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzodufca.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3eyhapsdz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3glaldhhv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ccjxdrqm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mwjnvhvl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3xytywluo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3kwbxpghw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3fimipixa.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qmyltyvt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hrfxqcze.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3niwwwand.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3afzwewrw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3justqkgt.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tucetyct.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mgdsfime.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3omffgeul.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3cqrgepoj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3urgbfkdk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3urhdaagc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jezdfemz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ohxrtouh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wismtnbf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ubwevfhg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vjdghnas.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fzzbavlb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3qgkrkbam.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qrrcxtda.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ysilzara.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kokckocl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3duoyqpdr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3shkhpxhq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3oilpliil.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3udbohlyp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3apqpazoy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tlfihbip.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mhutmbwc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3oybpcscv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3oiynagci.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bzwsjjha.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dzvgfytt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ldibgerq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3frnvvknk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ngefhgqc.html


<!-- 参考信息 -->