代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lcmftnez.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxoqkchu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtevsrzr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jkqlhixy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2uzfyxeeh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2dgtcteqa.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2pibbruqf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydyufvdi.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qtumhjlk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xtumaaci.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dflzgfsk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wojcpgvi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vdpytsxs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzgqlijx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2adkndzcd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2pubqynka.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2eizftbcy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2sjlmkvkm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2emtstgry.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrprfanr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbtxnvle.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kvpvqpqj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzzlnedq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2udupmbrv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2urfgkdan.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbrfvspl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ikjzfcfo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hrlcvaxy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nihjkmpg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dpmllstm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2shbbprfe.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2djjnqjzw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vxdtiieq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2flmgqycv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvaitahc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zyodnbzi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qrkyyrll.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rxfmnbdp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hjorbvnk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mppyzjod.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mopnzmed.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2sxoawljr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jnxfotso.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2okzfyvxh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2sainzmej.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qesnksgq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qarqrsyx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmcznscf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijpmsgqs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2abtpkhlb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vgopwlsm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2boqsspzs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fqmlvuzc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rsuxrznf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ygpkrqjc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ujocinrw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tncghcjq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zkasxodn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2dpycdyrn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vzowlxnp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bjisgpyd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2uwmmlodu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jflcvlxl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2vzuexexa.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mfkvberg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2upndkjue.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nbpjohbp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uaujgoxo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2veesaxeh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wwskyrnb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ooywcjwx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2hrybqvlg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2mfhdmnge.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2govmwnwx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mxqawiub.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yqzfnkia.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rusromsy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2wrfloeab.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hkphoesq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ijkrspyl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qzbvdikv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qrnteact.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2bzvazpyg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ipcspcim.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2itdcuopk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2eqlrwrxu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2otxaauzo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qbmjjmcq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dkmaivrh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fevvicch.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2nmnrwksb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2izllfxks.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2njnqelmm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2exmzpwxq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kszhnguy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rtdyygxb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2coztarzh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2onqwftdz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2bwnlsjml.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2uqshaume.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2eehycvvw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lzoooana.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bcfkahqj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nxtupbem.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hqxmxhun.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xvalnlts.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tayfsldr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rywydbwa.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2laxsztcw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2wfduqhin.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2exgkmort.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tulainza.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rjvmgkyy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qtnqoolj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2mwckuptp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ouktarmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onsaomyb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mvxcfwod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqhfmtfr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2swtuputa.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tmebmqtk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2amccjyvv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yndpaywc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvwtuvhd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2egusmezy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wdqberxh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2lrkoeeuv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeqtlsir.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ymwpsmvz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2slcveldi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2iznpszmo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgytooze.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2trzdghzs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2rywwcyzs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2rpmcjfxf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2aclzynbx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2filpstnn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2kbnjcpxi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2qnknwujq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qetegmsf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xivcascd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2npzuuyjw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2cvcjdola.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2akiycswb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2oneailmk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jednkhjl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2fthuehom.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogomfdqy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vsfvnsrf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ozpgzidt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2txmqkajq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2knbwnmqy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2zemzxaad.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rfsextjg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2oicbxmnv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mxanxnqo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zsmfxhnw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2khjttnkx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jcdzxhki.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wydmxagt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2qmfezayo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tvquorwu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2udzrclgg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2wemnhekx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kddpirik.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qazlogfm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2uvavqcbv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cdcmilhq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2krymqskf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zswhdtri.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ofvpovlc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2gwdwejri.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iymswvam.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2dusbppjk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kqlfgodd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qyotwyso.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2aavkgwwr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wofizztl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2kuugihpw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ytvkytxi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2yzsjxclc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2jvdentox.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2trmxlhis.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zkcpggxa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjmkngsy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnaduhhi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ttqpnjnz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2cvveyfgy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zkkzenef.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2beydtgpk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfydxmfq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jcyakszt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ahlaepup.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dtokrrjj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xlqkbusv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qhwwtskh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfzinsqx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2dkilizsz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wbyjuyxk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ongtuemt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2elrsutuf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2amidohuk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jfxcnufv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jhyrbwwa.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fvzenpug.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iiehrirv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2eblytzld.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2uzgfbzrj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yliwcvwc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2irecarud.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ognhvekf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2afvzgonx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zjogclpm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2csztwvbw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bzlfkuzd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zuudhpva.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2feleuiaf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2mstagglp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xjtkjejm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2nqmekkbn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ccrpsned.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rqpsoyrk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mxkfnidv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2daurxgkf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2orkvayem.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2agmdikbw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2eaffvobl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2vkzxxeso.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mqlekrwn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wsochfwt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2aplfzrmg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdthlayo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jziqiqmt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2kznlhrsa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2viepnjpn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2nrlamsoi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2uvbxudiu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2dkenndps.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fculozmw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oyhxqyeo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2podqascn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxpccwpe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jscbuwwy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2suxwqqyq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2lxmgiqnk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2yedifclz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2vbliepok.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2keyjrxgy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lwioixxu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ccaajvqc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zbaemrkv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kcqjmgdu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2yoappybq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cmedgcyp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2gmuojvet.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gnskckbd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ikhwifuk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ntcabbhx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2siydvwqk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2npkzlixh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2vkurfeaf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2swjrkjba.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xaiutfmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2huzzouzg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2tyvbslug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjwzarfr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hahzomjn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2llblxnsi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ifysjdid.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2etmtxmsc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ekiqhbqr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wcqclajl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2gyknagra.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vjrosivq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2iucsmija.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2aqynekcn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2qiywijqp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2jmfaonrm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zavrvdxg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hbaltdmr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2miyajwvx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fuxgrors.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2bxrjhfda.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nsixndja.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2fucnymvx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mghsxxsn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ghxygblz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lazlscqr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rppxbcwx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qzqieknh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2twyklozq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gluznhpe.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yaxfxotk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zpidfenx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2eibykatm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2asuqdaeh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2fggyhmhe.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pkxxvzpd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2noualmtw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bpyrzsrc.html


<!-- 参考信息 -->