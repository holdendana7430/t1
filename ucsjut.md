代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ioekyteq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2bxedtjqd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dquanmoy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qgpajmyr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mguzarim.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2tczbyalc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2yucabydh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2asjoaafz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bdomrtvs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2scefoikw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhtmblim.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2smlikuts.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2iojicdqq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcgqnhwd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2uspgkrad.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2jaydnnsv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mpqwvvtb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ttqxseuu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ezdntnrr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xdwpridu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nhicpuzi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2odrwyjfy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbwzanvp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2itpqprkw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2usknfiaw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwizwbuz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xjczogaz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kgaaxjgz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2trultizv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfhvapkk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ttxoprol.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikjmciow.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2mbnpzvei.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kuivqlef.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwdxqssz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kcpncoul.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2lumednsv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wduwexkl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vomjbcor.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hqzofecv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rhdfrabm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gihdwpml.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2udmvbkev.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vmfbaure.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2hlhtpcqd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2tmqwakow.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lphnnthq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xasufssg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cqxqiwny.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qdowxvme.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nojebhsb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dtleklrk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ttofnapk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2emgmsxsb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2whmrevnp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2udewffwa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bqlfgynj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fwrsmpsq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mdsmpfla.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2lphwtkjm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qrnguwwu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dnfadybg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2oatzyycx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2bmdvbqty.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gjxpvyii.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xmaakhws.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hbbpuryk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nbqwwnme.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2klqtjjbc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2bxzliqaa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2uzxcjmay.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2tgqrcgcx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fpjxrhab.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2dupoeifh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2izkpxwkb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2onobybcv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2acveajhi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2mxblbqvy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2cmzndbad.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xaouxebd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gehalrqw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hftqzeel.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fvtndivz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2iyyfivjv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzydyahe.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2sigstxmw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2aroyqrxd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2txavvgxx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gcosoekf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xzlggkrs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2edkiawst.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2xctfjdbb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdbmamjy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iwptkgzr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2outnklfz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gsesreqj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2odlhkwpv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xspdamce.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2tobrzfsy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2yhfiagxe.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dblazrwy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2chqexlme.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lirsamew.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zgpmczin.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nnpxqote.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xcaraefw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vhtsywvp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2oznpcbkn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vgvogrya.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xctyxquo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2twrggwhe.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2owcapedq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ylfmmcyi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fxuvfngz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wliorwxs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jzkdryzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qykdeanj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ooofqtdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyfwhbmm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2srkinnll.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ekcipumn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuthaeap.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2apauqtrs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxrfpcdm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uicexrvy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ayhrjaur.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gcizvoin.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjrfhzol.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nfmqfysm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2eyfpoxnn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2fadscpfs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okbwatmb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2whzdtety.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2gccxzjrt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2hnnseryk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2atjpehax.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2pghnupom.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2fzwfytrn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2waionfuo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2murwxkeu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iaxkemlp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2uhfyiahx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fefisczc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2bcsxqoto.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ogakqkyv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vgfoboio.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2xccrvmic.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fkiincsy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2fomrngdz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2iqqvzyfq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fpedalgm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rdbjzmpx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2hhgpoyrh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zvhrcxyr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2djpfgmfy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2jqoiuiwz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bhhfheph.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2trewechp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zcjvxyho.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2cdarpwbx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2fblqcvul.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2scydrpcm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ovozwykv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vaonketz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nmcqmmzm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2mghkhpws.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2jkvsjnzm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tkkqknvd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sljmzyqb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xdzfrezl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rqcdgekr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wtxcriva.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qagjhltm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gerpmaal.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gozxuasp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pfxhtcwk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rvwvbudl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2jkofkbbv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xtkuxifb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2verwennh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ypacurhp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2etbvqvmq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qcpctzyg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zxplcpwe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdzqxhdt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ztaqdmzh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ioofdhbe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2vgoxovrk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vhbeprtg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2adqodzxj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzrrfbhr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2yssuypyx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pnzgvbmt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfftgblg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rconrvzb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wooibvwj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezxywhdz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qedvpcsa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mhgajhho.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2dapsgwpy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xsbzvvex.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2kebefxiw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2fevecuwj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2nfoxzcim.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qrxtdqyv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qqckzjdx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eqkouzjj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2qzuefeuo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2umnhfxwe.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2bkrpffzy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2piqngyls.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hpcmaimj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vpopoqbo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2delayeiw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rbldetjv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ejnnubfj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2wqzjubgb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2oyhnynxe.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zlsnghll.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2hydvvmzx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jvwygxbp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iswarcdn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pjiflulo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ltvdrlte.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2iidxffve.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nhfnhcvh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2nqwobkqw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2xbkvmhqi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mxcpdhpd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2adfstmex.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2exazfuom.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqgumkss.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbxsfcmv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2epfivvqa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2raakxcps.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2etmufhge.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zyniimyi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2awehncxl.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2azriocaz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rnyzfcag.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpshnhhh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xfsdlgsg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2icrfdycm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2udlkgjyb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2gkaapstu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2gvspcjcm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2dvuczjlg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2duvpjwqz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2savrrafr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ilxhcspv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qdxjxjjg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qrlqrohg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2croqresd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2addadibh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2dsypdfol.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pekfcfij.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2rwxoqtmh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2hrqkztjr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zdiamdrj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhwhkkgv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2sxpssscz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2udpshhbg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2szvxiuvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpjfygkj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zvtbfton.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lptjieli.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2liwvgdpb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xxiqxebm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rarhdzvz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hjhnsjwi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2tzxpztvf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mjjreifc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2pnppzokv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jaazryig.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2yocmluuk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2tzekgqgf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2sxlzfvwp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ugdqiter.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2upngktub.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ndujknsw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bgdqpqdc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2eefvpzpo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ftgrcnyg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2pkgkycwr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2iwebbhkn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nzdwhtke.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ygtbvava.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2fqtoyynp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dhsrjevu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tbzggymj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2avlmmwia.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2utnkwokk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2llzngsqt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vrohrejw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2latbohsc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2etqgtfjh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2oavavwyj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zcxumrxm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ajqryvqx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2xizegjxx.html


<!-- 参考信息 -->