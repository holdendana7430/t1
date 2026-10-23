代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3jowpmmwe.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3dcophmcp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrbjveqr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3axefwcbs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3aedgvftx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qqtfqoxt.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3nbhoaehx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3azveeraf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3khpwvluz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3psmrgdlm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ijifzhwa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xqdffpnk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dcoixxsh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3otghkkzf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ysyloztc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3otlgtwyb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ssgukglx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qhshdcnm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3yykgzorq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3rctkvsxs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kqaeszuj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cacusmdb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzkypzsg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ceinqytp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zcpcungx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ewrcrwyu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3xwaeyxda.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3aksiwjyx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjzcgcc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hvseyspe.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqdylcvd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzzcoxpv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3mdvktspv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3gxorhbnz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zezkklbs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fkexelfm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ygnolsqc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qiduszyg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aiiatwbj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kmqrwcen.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3almmwttt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nuygnqsm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3hdlfekhb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3weivkzfa.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3eueicfvp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3vwfajcrd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztqvfbek.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlozlfzf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwcpfocc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwuwbcdf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yvlogorg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3tjatvxwy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ttrjzsem.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3dhdiowsj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3tkhhjipg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3afoqnrxg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ynkspfbl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lnbxmbyr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqmglmsa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bpdcwbtq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dmzhonfl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uaccyzmm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ubojznhk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3goyumsfa.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rorosini.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vcdakhqj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bangliwt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3flondygt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mnofnvie.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ctatqpbv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3xphrhplk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3sbvuqzyk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qkteogcs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3mtaogvfk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ujgleowh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dciwvtnn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qrxlbszy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mbpoerkl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pqatyvow.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vtqjvjwx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3tcrsmots.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3umwonjja.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gwzexshq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmaesnkh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ldzomwwh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bklvqseb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3yjewhocp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3xxfybwgl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jnobhmzn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pvbhzppn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3unmydhth.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wsdzjpyo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iulpweub.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uanmhsll.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iseaomvv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3vgycisvz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kgcjjzhp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3khtmproy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3oeoetfln.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3jvhfwfzz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ukpeufqe.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rtcsdytq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3upqyvhbc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3imntqmzt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xactazck.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cfglziih.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dbidnruy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3peekbjai.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3trpzshwf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3cosignpa.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3arqhzkel.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jionipsm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3naarqxrw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3losjsene.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3inzipevz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lsplxcoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egxsyiws.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3cehdovaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfqkyrzs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zllbfkkr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yvduzrvj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jhzqblwp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqvqfxya.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3igruefzo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngyoyzra.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3drpkofcs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hrmeofiy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dufhqoyg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3pmmxocdx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3gcdkmgwj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3sfcxbzhi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3undrlisa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpbqaqpe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3cwypanbl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3owjpqcsu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3lxnpmbgg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3slmepsym.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3yaoaoegx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gmmeexfn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3swiywgqw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3luxobzen.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ocwctodt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsayfvkh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ptpovcks.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3vauuwqgj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tdktzldd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tszbnrry.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3arlienjs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3sltmvysp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgtejjfs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3oozvqaro.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3wodinbuc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qlvdofql.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hgvfyqqt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tqhsglcy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3uqijeiug.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zsaninpw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3odqrzyrn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ygfeopsi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3iagtmkko.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jrcegomy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pciwbyjt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wigpaadx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3vvrtnbvy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3zwwdmylm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ffysjnhg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jhzgznlo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3louyvngt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3esmemnap.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fejfuicd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ltebtjmj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bdmltwkt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dknfdoxn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ugjwydnm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hghahqbu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jfxsbzce.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vxxbycrw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3oqkhymcl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uqcwttml.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3sbxwvuxl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3rfnlbgct.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3yufiyuhb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bgwyzuha.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3aixsdyal.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqhpktiw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oyjxkvqj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcfvevyt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3isxfbijz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3dsjmdaiw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3hsgnuces.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3aakvudzi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3hlsldpeh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yksvscsc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmzvccyn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3umohswyr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ddjvxubv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmqrntri.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3rmqkqjvx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ufsoencl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ultbpvjt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xntbhhgr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3vdggcdez.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3urdtzjnr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jtmeirkc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wcgjetpx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zpuebibi.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gtseklkk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gneonfek.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dksrygbo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3yxjylfsu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3lpauxgbw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3zcnojjay.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qboeackd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ofgmblkh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3twsicsja.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3vttjiwpc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3shjlposr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ffcgmfei.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qhnccqqe.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3rthcocin.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ntvdwccx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mhspqavc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3upygmizz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kkeamnzh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3vdicgvdm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gmdsiprv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zusqtvbq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3wdexdirt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3csgdiqup.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgjqcpix.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xxbmlycq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dechkzhx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sthrkkjj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pcwcfufe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3oxipqcvv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3pquovfxm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjimjasl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dlikckhm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ucmovvxv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iizjfcic.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3kxcjidrm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3uenxgyng.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dqqotgos.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sifysjkf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3qcucyiyc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3bwrzuemw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3iyynhjgo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vdxnmrni.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fryzyhpp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3igfwncqt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jgoramyg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uwodxdse.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ptbskhnz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3awwffpzu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qkpjtprz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vrjwdahg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hltvedwp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fqxwnvrx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3hmqrlrqv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cctrmdbv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3pkohufsb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3abwxpwug.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3evriavft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilgqfeuf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3vokznjsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xoqiftzm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3spipijym.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3zvpvzfgo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kgljycfa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3aaqdvtsi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qbwpokqb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3jemhmyjp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3onbspqmn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ycocnunn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ejkyuwzb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3yvpybqto.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3utiogguu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ufrugbnv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mjfnctlk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qjwwkjam.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3nbqyspss.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3khmnqrxa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mudyqmss.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wdnpficm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fdeuqzoz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pgwnizdq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3npwcykrj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qorvcoiw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cldjghxf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dvqlvqkc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ifwaldke.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hnaajqtr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rpckxnlo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ntqqanml.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rkcmnyjs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3faycfpsn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3amvvwlhq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3uulbqfjz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rpxzmsan.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xkthjzvu.html


<!-- 参考信息 -->