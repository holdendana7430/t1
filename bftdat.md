代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mrastxky.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvjoubcd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xryaiese.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdkheiax.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3uwvoojhm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3bmfxpgdj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3wsbnxhzn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mkcpmytc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3awarbemr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3xcurjplu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozftuxgx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ghxmyuuf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3folnbleg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gccfuzrf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ycmjtipf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3reelwkkl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdamzxlv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3uyhazpxs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rzrnxufq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3mzwnqabx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jadjsjfa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3goavlatd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3kgpndlmv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3cmkhhnbz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wyanlbwl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mzioseth.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zywthmwo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gkfjntjr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3iiqtysxv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jneldkbg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxacilhz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3npcklqcy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3eyyhsejl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3mcmornjr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gncuwduq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3uomveglj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3wqeafznw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3agsxhmpv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zbzbxzyd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jhiyqful.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yqndhayk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wphirebo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3rcyxyfme.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lrlopytk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3xctgtqim.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jtvzyxnl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyosojan.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ugxlhttz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qcphklqg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqmekzuq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jwkxqhfu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qcstnokl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvzqukms.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ylpmvmnv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3mdhpfgdh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3uhtjzzob.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3udlqzkps.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hrvhlavb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3qkvehekc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jyxliglv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3gyzoidhf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gihcance.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3xrlmjloj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3moyktizi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ecxwhjuv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qdvaiior.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sjtzvocv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hiswfahw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ofnjmcit.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3gnjfeptt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lpbwqjtq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vjytrjng.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ehvxmsln.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3olaorara.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cgerprym.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mwxhrtso.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ycpyurtx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qdntxgdj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nhjqvazs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3qhkwptqq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3qqwgegfm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3xazvbkzh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3oudmsmpp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3avsqcvyl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wjthgwri.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rhpoujyg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3pgfkipfe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3urfayzns.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vaqsstcn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3mbcxfria.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ykhhoeuy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3gyywcxet.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iphxabep.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zcndxglm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzwvttaa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wknciccy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfsnxwwt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xewdaipg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3kgnmgkhp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3zzlhqdfz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3mexjvvys.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yrtytuum.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jezgzfma.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aiwdcnta.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3odvneruz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wdihravi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3avfkfxyq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zijhlvyy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wppyxjsp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jysyaxek.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cubnqiua.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fvnssfoh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3owosyhgw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3bpiuwzlc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3nslsgmui.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gnurrfks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irxcenxf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3stbpanri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgvxlzve.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jwnouzyf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3pfeygoui.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3evkdmesy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3repuwlca.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qxrzcxdo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3toagesms.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wjgzweuo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3rcsoxytg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3usayucel.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3luthodpj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3riydfywz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmsomvdj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaqgqfvw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trlcixux.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3mkzmaxvh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3uyheywgf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3acpuolsr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3mwaraads.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ztoiqhfx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3sfayfrwe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3zsrmismb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ulnqzeuu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhosxwdd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdsphrkl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ibrcfghy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gmsmhdhm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ilycgcif.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3laczellh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3uvgedekg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3trngsdzw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jleutjmt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qpbfrrta.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3dzfbohds.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ycnteqtg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pluvkmqx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyogbizs.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3adhcfjfj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dynajbmg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3woetzgqz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gyzqirvp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pnfeazdd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3lnbwkxvq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3afywmurq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lnlicuhv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3tlgbgppw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jcpgqems.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3znzrtdkl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ffnfrmzj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wgtvkkxd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3itirtboz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3csiydesa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lurcvcyt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3agvoyezh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nwtvjteu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3nfmorpsj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3diyouyyi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xlvnrsjl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3nywaeunc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3wquonngu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3islouyjs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3dpbnquze.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3levmlacr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3gqhbosrb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3rpaeoxxq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ohioqjgq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3jopprdny.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3sufumplb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eqlmbabr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3oytsezrz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3gajowxut.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yvwryosi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vbtxppin.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3orofamer.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vpqkgfwz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3omowyryf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ghwvqzcm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3aobbinxx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3diraagza.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3mdlwrxln.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbtvfnhv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fvimgptm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3cnyzgupp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3pmfgkyyg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3cjpqwgsi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nlvmzizf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3bloanshq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xvnldsnr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3aolczdjb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3yjlgvoca.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3djxxobzh.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3fvxeklap.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3lxcbepdr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3stlutawf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tphichiu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ohinhmxd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jfbthzbt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gbofmtam.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3pzgarydy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wadwiqxc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gkxdqsia.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3mxdxlynj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3cyomqzoh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ykhzxamk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3idalfhlj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3jgyevfgz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3llveunzg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ohbrtvib.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3oxvpqpid.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jqrtudkp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iqynthgv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3stvborim.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3uvucysvp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wmxmimpe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvdvivpi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bgjapdnc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3mfvabpqf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3dyqozjos.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3puoswkfr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wllesohf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qctruzbj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jegqulse.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycnnknzr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3njkfgehe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3pzkfngxy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3idhotcqf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gohwrwnn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3wfapuvpp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3yrrfijvi.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3lkvdewdd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3efikuots.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3gwghilqo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uehyiytj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ubsbtygk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3hmetdtzq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lklvmsvl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3tjwabbzt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fooglfth.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3kqobyohc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3rpiemcrf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3eoasgwxj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ilsggows.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3hergtcyy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3rsuctzza.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvxgjvrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbedpqmb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3scpiegor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtertcgp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3durvfkkr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3kvhftfbp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kvtneseq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kefyrmdj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qoupsehj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3bdfyfkac.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3aptlkzvv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fzgudadr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3mhhszfxo.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bavkolxw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ftxqmwiu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3osfblujm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3scdvxigq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pdjpjwze.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vwwwnwuu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mfwdnsst.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3fgnxsegv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3prykmwbi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3aiuhrxxd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3yvwfbfkw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dgjmhjaf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3jolurkra.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3koijjweh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ipxsiycq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jqpoxtxl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gemqurpb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3exhcgotd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3crmfnjow.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3yznsiozh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3sichmvdc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3morgatzu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3nmadjxoy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3qyolcxqy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3lbsyclzp.html


<!-- 参考信息 -->