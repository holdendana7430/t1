代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2umzhuvjr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2renesiyq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fpbupurj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2matykhry.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2oktiqzvz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nvbfslql.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsfcvabj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mykvycis.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mveuisum.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fodumbpf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mshyzdnn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2cxufqxji.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2tldafhxe.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2kcwsvyqm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wigklvbe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2svoeryta.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2flmgsmje.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfqkjyvy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2keqkwiuq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2mvrqqwvi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kgzkpfpg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2eppwmplm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2wdpdvaib.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2pliosjph.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2dxmagnxb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkqnevqf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxuejlcg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2trioubdv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2mocwdzdr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2mntkqdld.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgztljkm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2najttkgk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2grcuhfaw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hzxrwhzl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gbuugmlv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wstpjjhi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2miwtjgiz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2eyvpfvcy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ljovpygg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vfkaztkh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mlstselq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ujoytsgq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdlfnhrt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pokhirvi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggvnxire.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pcleearq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2busnwxje.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2exbgcayf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kabubxwu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2zgmsbakk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ncbsndgh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2pqstmici.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2orejjams.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mqbkatid.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jbtmgroe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kfqrrzes.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zpmwgbni.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dioucqlc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2clgetmec.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2fwpxfxsk.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bazpepgs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jrockpin.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hunysqje.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gkifapoc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2uycnpfwy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2dnxshdjf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2snakkvfg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lzljwpmp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2uegdzmqe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ojdkfzcb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yaevorcg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vtljetmd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vvujcgok.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2mlyrfrky.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2oevuptsc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rnmokwfw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2llrtvjgq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qfykhbec.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2olnknaai.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pcpdysph.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sfpvzwst.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vpjontgd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2mshzlnzl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2tjjhojuy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2okkryhvf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zheozahf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xwvvnyjs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2clozbemk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2phknjhki.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zcbsqske.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dehkokwe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lolskunc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zasihsyu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xwginpom.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2eaxgxcbx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cjnlgxnd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qzuibthe.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lfgepccq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wckrlxvy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zgdovxsd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zmqpvdji.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kbitvksg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xassvvvi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2dzwcupcq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2yeeovenv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2kctrnmsr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2falqaohz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xntupzpy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kldmxjdj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2upxgrbgx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2nfkadoua.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rbjlksvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqtcilus.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2kiyizizo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsenybxw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ylcckadq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wbougnhy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2epbxfmsc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbwuydiw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyngmajj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbvogojk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nknfbjfs.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2jlvsulnc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hhedtdzh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gvtghsql.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2mygywujs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgqqnxpt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ybsdkusn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lzmnklwn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ndibnsam.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2exhctzpe.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jdualehu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2yjqromfv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2guihifkg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xrixhzdq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvdlnfqa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dwqiaqne.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqgsznxq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fltfncmj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2tvhqorun.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2iykfcmtx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2skqztuws.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ajkzjdap.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mvzyrnil.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ywpihjrz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsdwcwhm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fkhnkrfo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rsyhbljr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2kwwfazik.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pliqprpe.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2clywgllk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lvqmihsj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2akoszrck.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2gogkiuqw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2laeyqovm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xhhvmimy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jlqnwwbl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kejybyju.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2asyucftz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2wbnwcxyi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ocyrhtmc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2tzctxpsq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2atnxpuad.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mophiayv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ehrnkjip.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2lpmfrepm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qqlljavb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uhqumjiv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xrajptwd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cgmdjmcm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2mlcruhvs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nnwmoegs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jenmtvzu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qmjxbjqn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kranmzlj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2rmtxutes.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2kqsyohpx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vatslcrb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ipsqblvk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2aefeqldk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2reohliqs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pmpuggsb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuotypyr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2eyjmyqbm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ogmcaghs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pffyfruf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zbpwbazt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2onwacyht.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yjcirsnm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxurbhlc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fyazuihm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qnyahirb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2umddclrm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gsnvluyh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xmrbwahe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bgufsjxy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pmmoksxq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2gyncokho.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2mnucaava.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mpdnvnov.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2gvtahacw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mopgnkqf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2elhtbazo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ifkitwjk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2umoubaxl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ymctmasm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zlpvnjdd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2qfokhwql.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uoqjszvl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qomrhxhj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ihbfwlmf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qjnlxlny.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2cktywzik.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2nohxbslr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2pbiwzwts.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ebtpmcnj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2sqvowqrx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yarwpjuh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gbjskhdj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2lnjscfnr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2lfwvoubr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2aojdriby.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2avvednyc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2fxvbnvdg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ibnylkgh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ncyraizx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2cvpsntti.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yydwfqzy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2khatcguq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wbiokwoo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2etnqxtbh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2sqantsvv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwjiksic.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ifshdrcv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qkfdhmvn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xhwzzfna.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2fnirrpgp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wnrvdjvj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2wawsunon.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2difhfhhj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ghfmywwp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ifpexciz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2spzrbokm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bqqgshtp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2prcghnqv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rydxfidy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bbitkgww.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2iiggfbpj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2uyckybuk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dcxpukek.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ddfydsuk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xfpjzezi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rvyyxcie.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2odwmxbps.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2njjksmzw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2glvteqct.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xqyrikfh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pezzozxd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssvdyvrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjhwfgcy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ygawxroj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqfyldhj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fugrphgz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vfjajvng.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zxphslei.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yonbgnfd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2grhhtbga.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2oyxwicyg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lvaefjni.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ukuubkgh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2cqwcrxfn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kdajjylo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mvatuyae.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jdggresx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2izxvbakm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2glidfrzc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2rywsntyl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2husljyos.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2lprrphds.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2biqdpxpe.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hoacuhoh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hplgsufk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ljxtbwga.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ntlxhytz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lhxqxlbo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2erwqaanm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jdlyaktn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vhwmlhqs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fdcguatx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uweajqok.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ciklhqzd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gxqomcrn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zgppheim.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2snpnvyud.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2smszpmvt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2bcquffnk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zdbtngda.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2julegxpy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2rzqrrizg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pasyyhcn.html


<!-- 参考信息 -->