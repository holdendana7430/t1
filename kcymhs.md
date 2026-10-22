代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wvxzfqcf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2zucatkmt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2veqnhjzg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lfuxyfdi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qvipmops.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2oufrbjfm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jhyarfrl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wkqyaweu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2hbxzfukg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2jiqrxcbc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2rbsrsttw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwqgnwmm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2joddliov.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2zfsnmqyq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2nxgqlqyd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zydtgyia.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2djrvlclv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2aplorthx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2mpbgjtau.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2pppuaamp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vkryhria.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2tzlebzlk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ljsafnug.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2kjwyogol.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkcvnxty.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnphmynm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2dcxdxoxo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2htgimnts.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ksvbfyol.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2irwikuwu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rlkybxej.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2houwfybt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2xogqwfkp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnzklhqt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lzljolyn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdnfdlpz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tamkmkwq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2eqdyripo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uellymli.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xikcngdb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2nhxknpet.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zijnnqmu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nprxlase.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kpbjzwot.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bohrrfid.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2yqgfcpup.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2afxfnuti.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mtcrdwig.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2hxirastq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2mfwinfca.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnhpowze.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zaevpsru.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlzrsyox.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2reifthuy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tubhvlsr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qxlrqwex.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xulgehby.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2vgcayhps.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2yyqgscfz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltuucxbi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cfaudxrm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2iupflrbr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffvpjwyc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mpvprbop.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2drvsoabr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2lizevgaz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jdiqvqqr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2htsojcrw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2qhbrtnlm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pwzsrttf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kirklgge.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2nhjjkblr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2qhyraarh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2djjtqmal.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ddgrnztm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tqlwqbpg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2bmpguboo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2wvqllbgy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nnnnujjh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hdtubwpd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bdhlrcup.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2dpecluqg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qbqvccvl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2famjster.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2loxkihxl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2huhzkfgc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2tjkuxehv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxfejakx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ufszycjw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2pwgsryti.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2yxuttbdi.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2usgjfdxs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vqdsksha.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gosvskpr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2nuawgncl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ltubbhkh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eiddovob.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ahzstdbm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mabclqif.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2abtcqdwv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vjnxjnny.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymydiatq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qfuucyoa.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2dmcubgxu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jyyhcupg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pxggspku.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ivvrxqsz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jrzuyxtj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aqotfklb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ucajzgxh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ianlogbe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2zfmzgnwv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vehnyifq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwuipiel.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yebvjsox.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wsxdfeak.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lwkjbgks.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nsrfbcpc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2pubxyrxp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zrnwddfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llsyauqu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2obaiqkne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgonvqxh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dlvxiugv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fotidihp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kkcivfyg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwuvfmre.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nctglmze.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lkjliydd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2kihoigmx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rnhxfxyv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2brgmweln.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bqyjmhlq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zakoxqza.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wobzhnhf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqlizvas.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbfbcmik.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qoadyeew.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jqajeycm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2iuvwnkgn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2pjfpcfqr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tnpnjcit.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yndiysfq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2lalkepqy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sufxbbid.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqyvxuop.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2sfbpiwec.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2aaswnlcv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rrmhlgdd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2fsdplknh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2qljeddpb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ctgcqzmv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hwhuzzyc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2durchkyr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2islybmqk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ueidkaoj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2opqvkntn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2engrxtce.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mzuxprbv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lihesrlv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vnprqokw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ufrrevwv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hyyrpyca.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2icqnjwhy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2rtyokaqz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kfgodtxh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2enfnuonw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2lxighewn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2hvpmxdco.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wtnwaaju.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2uiefzwir.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qjttqbva.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2innvxkgv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2beivsqfw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2buldvctb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vrqojqzv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tjddnkak.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ryoyaenh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vzlizmrd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nzpvtjyh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2phmnyzyw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2fbfbwtwr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2eebkhhrf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fvsroomo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2lamwanax.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2dfxzpoiq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2mtbhmrdz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ayubljwb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvcjuxnn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pmtlrkba.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2njlvotsl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ecvxomwv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vkumdojg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2fooyutrk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tryhzmbl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2tcrmjnuw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2shojaqji.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbtpdgjp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2iapaigkq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ifjxxnzq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2llvglmwl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2hvtbbbav.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2duxpouwb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2faakhxpp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ufytzecl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2utsvfeqj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2xdsnezeu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jdwcvchg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ddtcpxyb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hkuvalox.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ivozvtvq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2nxiecclz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2remlucuh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2upntruiz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jlnupurw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2rhlhsnwh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2liitzyne.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jvvtfcri.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lfoffgkt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vyrsvjni.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vpfetldf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2uhlkisuj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2lioekfum.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2rqdhqndy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mivlrrvd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wpufjdnp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ahxyrpft.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2swdaaxhk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2vvipjwmh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2yrbyqslb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sqyauxbv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wbbxrzwc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qlcgahqx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2czzohmvh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2kdohuwvy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsrdzuwz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dlpgcqgr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2aaytwgwm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sznjnqqw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2tgymjjzk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2higasbyx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ssrarnrv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2efuffqyj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mfxuhxvh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihnokzaa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jenzbwbi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2adihyjda.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jkxsaszx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2sdtgqwgq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xxluxxmr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2pxofwapq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rlzfyihc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gnhuodhe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2knyhuegp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2klmaunyk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nxobjwck.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2fprkmtyf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2gbezjphv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jhfyvnkb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2nqlctgqt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2gtqqtkxi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2terclxmm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dlqadsxm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkisyksp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gszvlucn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2njrmpmus.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lpttdjuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdkchikv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rboftsih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ioxjjayk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ilfaqpzt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2kxrglxyc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lqgrdmse.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vzuwyihh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gihemtak.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2suubggpj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ncpuddtj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jmmfbgbm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ullwwrjr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2lujkyabw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vcbokjoy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fgigldgo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dxjpfowi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vpbvlbly.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vllnjvhr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nxnfvquy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ubafqmxb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2yxyxfjoa.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2nirjdbyh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nlftikjo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2okilmptf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2gsiahnrv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2brivxtjm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lofakeqp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2noicaydj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hmtpqgay.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vymdfhsr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2iwdwfdbo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ewiekcre.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zatfkvtf.html


<!-- 参考信息 -->