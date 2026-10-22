代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fglemhqt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2byagdwdc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2cealklwb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnppiuym.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xpfsbntb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdvxdzh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2smeaqhle.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jtrtwitu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fopxelxz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2rfqbwycm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2waqrvgjy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2cddbyxsx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2isnfrzvy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qiykcrql.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2kqdodguw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pckxokjh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdnvhikl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qcqxtcbe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qrhhzdco.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2abnzpaeo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ljclvrli.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pcowotoh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckbcsfrr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wqtyusyk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2oxaxorxi.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gytcxlmw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jsahsscw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mickoaxj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ldwegtxv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2uirjmusy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2plpiyixr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2otkpqryo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ykmfgpnk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tlixadfq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fvqkyqny.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iomeotst.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rzlkkvof.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tynipvxx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2delmxxsb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2roofngok.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zfelkxmk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ohstztdo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2inogvtfd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gdofoqwe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zsrtsbdw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2czkkrzfl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2csgfmvvf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2pbegphuq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qqqczigj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2yzhgaoci.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2xeyznort.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rkhkapmw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ggtvldrb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2efzhmdzn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzthbxqa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nefvhmtf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2jrcvukev.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xdwrxzdt.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rjblmxjx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2pswfrpqi.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2plynhzbe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kwtnircc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ccwsbqdn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pmilgkoi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zoieppcp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yfhhvxpa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ooogurjl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vuntzght.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2qdqlztsi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2gjpkqvqg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2riwkolfo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iwlqmjmh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hzxqamft.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ucmwqhpw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2lboyqxpz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ygdjcami.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2oyznahim.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nevttxgb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdblvyda.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nsupvqyl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvdenzqp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fkpxjjfg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bgnxuhif.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2adyjcoov.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ifrmgkyq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fjzpoyof.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2montbspp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ijtdcesz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ildxegoy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvqtmwzd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfthxlrx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2flfifhyf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hqsaxszp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wcwbfnqj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jkppdouk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ikvcprlj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2bbcxvxhr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qwquclht.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qqwvjlzd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rcjrjoae.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2unjvjnjj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vtuaiqdq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pgkxrzfy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2wyllzviy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nlnlxcgf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jelrvpbc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rpcbgtxg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lckywrdr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ewqpqkhj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cufpumpz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ldpvziiw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hrzhvuwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkurhkew.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2doxckitl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlogzhbz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mcsddakx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wemfoeih.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cmfrpxhk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rycaotor.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eeldgqgv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2terhggyr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gvtfzfyj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2hvmggelc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmemocyf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2sjqsxkcm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2jfyhuvqb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaipcvjo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dfupfnec.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiqakjrz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2aypqkkvz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2pjzhkcpg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2cdyzopzf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ebmkjsqe.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2uprgabgm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2fipibnzp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pktovdnf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ilszdcmb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwlhgoqw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2swvpbvwa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bvttzuip.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2vxtvkqgv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2fqydisnp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2whinvglx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2lvoyohwd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bhokqdrx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfjvovql.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ztmxuzar.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rjajhrrt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ookwrunj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2acjkcnbl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tczvipnk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dbzyctpx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uhuqgtrz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2wpwqondw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wvpgrebk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2oonamvyq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tclcqcfp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pdzqjijl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hdzhvfqm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2wcjajfee.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ddyduyan.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2excxkitf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2qmacfbxd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2baslwliz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nkaxddzd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2coqguxde.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2veordalk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vfaozwaa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iwlfmeua.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2juxlbvrz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ntgojnps.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ovzvvdhg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2tetzbdlg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ckaorjnx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jqgyzley.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2kpzoqrnp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ypjcxxoj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vxuzrpjr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2dmtonecy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vwzqzcef.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2shcqjfjh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ayneomaj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfvznqlx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ucncwipo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vomhkfer.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pkqboxlm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cdrsqlbm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2xugkftkn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dgnmozzs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2phydvcmz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jwwlmiue.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dncdrpdy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ibgtwiow.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mlobibvz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vmdepzzp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pdnykdqd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2jnqjqgzo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2sljupgcr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ipcslrnm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2chipjnau.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qedugnll.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gjbhusay.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nzkrxhrs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2okoednko.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2clxzdgze.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2uexrwdww.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2debxemjt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2yyhfmzto.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2shvgricg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2nbvxqwxv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2kvkhhvdk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2bfqiqwif.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2yosgbzqk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ggwlfbyx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jxpmxoki.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2tilbezxt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ctxkuecp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bpawbeti.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tazkpxif.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2sedfsbou.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2eohkjyzl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xcvxqlyn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2joadgwir.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ispxrzav.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2cpxxtfgx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqcukbol.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2vlrudpag.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ivqfotxv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vhxwuclh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2urlpzuwy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xihletgn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2qspffsaw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2guyijwkc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ptunshqr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oswzavly.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wunjlkhr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysqqppbw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2qhhupqqz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hucuwnyk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nauxedgk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dpkxuegs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2igkjozto.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bcgsiloz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bwdgtxru.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynfstnog.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytxsbrzn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dtdtvloe.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2btzrxidd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bwhbukcl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2hfeqshbj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2brhnheeu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2megczqvk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2foqrhcot.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hepydjqi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2zpthnaqb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upoarele.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dbtahfpu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pabfkoll.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftwneqsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyncgono.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zmnykhom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbkegvpx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kkvwzwlc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ojxdalmj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qvriwopu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tzdurrfb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2pewgndvd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kwjpoyvp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ekbmxyio.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2udjdjoai.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2akgsgohn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ygeohmqf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2pxxlkkiz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ixgvfghx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yfontbex.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ipnkgsvo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2exqeyfoj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2frcostla.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2pcwjkjnu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2tmsbnukm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mlqiofke.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bgcgwszg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2lrpnzfhu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2dzgbwrex.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pkjhohme.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qzfytvnf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2tajspduk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2vnhxkpzp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gsjlazrk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hzzcpwvb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rgxqqjaf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2pknzqvvt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ensnufxd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2uaajhfmj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pxqljyuf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ihtyvwad.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2yempcaca.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2huezssua.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ldnkvuus.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hwvzijxd.html


<!-- 参考信息 -->