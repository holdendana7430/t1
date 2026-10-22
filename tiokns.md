代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kksuhmcu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2fhnwdhwv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2bnpsdkks.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2adfazhyp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gpexrrxl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2dqvwtbmc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvhemhac.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ljiqakqq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wiaktxcq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2tplcoubv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2llvnhoyq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kbobcdww.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ergiggto.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2druzpchl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2gjwrgbgf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vatzcvkp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2idgtmrfm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nhupbxzk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2limvpgbd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2vyfuprhz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zlmvqjjx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2cvzmknnh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2hamfxrgh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kshxvliv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqxuujwb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzixdrfu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yjnxwhhp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmofkkuv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2rtyrqwjm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2iqvcueco.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wbxfvcaf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2urpczikx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zsmfzdpy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2swdsowiu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mbajygmb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rrhefmzz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qyzhotgx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dguisbbr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jixvcpso.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qrbxqauo.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2lsehzbav.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2wyuyygur.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bifihfqs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aayczpae.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ilegeoxg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtfxeshb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zlxzwraa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ezujladn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dczkqypl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2pxhkkidt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ihakybwf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2jikhleer.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lofwrplc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2igyvgckq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2pugfyngo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dolbxuzd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2gyjmxpbf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2miqymdbf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2znwwayzz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2lszyeasl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hnpyumwo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ydpnvdps.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2thnsvxni.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zvtzptdq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gsoreafs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2irmbwlkv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2efmfjuoq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ivelkefx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2uidjaqcl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2bxkutxxk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gmoxshgz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pkdeoaow.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hojthpur.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2tlghqlcx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hdpgbdvx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gffcxuec.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2bczbdigv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ucvumbjs.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mfayyebv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ibzmarwk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfpmnpcj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2srrqlewi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xxhpljxg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2egommsys.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2nvprcyzu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2efgkjezd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2auhetjzp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2dmkqkvzr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zrbcphby.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffeumqgp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqdajjmm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2deodsbwe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2efvtrjjy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2imcltbbj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jvurlsbt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2axfbzotj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wnfywqbg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gqirohfu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kdpfekwg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sbdwiewk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tsjywvjr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xcdhsoou.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rufaklpg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jkxbnfro.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2klblbuoj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2biqxuxhc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2arizfoxb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vfdeqaer.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rpoaimjt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2koloprli.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2eslzrtya.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yujflali.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rejjjzca.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bqzempid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkiltflg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cwdpjwph.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jyvqtcom.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mjeijetq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghrnkdeh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhtpaeck.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbjdlnlq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2cvcfohsc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mzseueeo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2auleccuz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ufehwkat.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zkreauxp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktknoecj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqyjqzbr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbxjnzma.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2shgrevfp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2fkdwwoyg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nmlphkqu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2opzpqngx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2piyjnoaj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2czoqcptr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2trzjkvxl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2odntoulg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2utfhalrf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2icugpaok.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2unjkihvs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2mmvpufqw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2abwqowrf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2vidcykev.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2haasgkxy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qpfesrhv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jaxmvcsy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jrqaouda.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2hmxcteba.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2edgauccg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vexlcvmd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wuyhwtna.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kwpjxsma.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jkjuhuly.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ewiolnvd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kyvwxbxp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nbtiyqum.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2lrcjglal.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zsogrlbr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2msuhrncr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2snubezuo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hrdksuvc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2xddjuqmk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2sgqjubqq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rprqluyn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qyweynnb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lazvmsem.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uobdhnmb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2pylwdzqk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lyzhzjhc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ugdyovrn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2mxprflsl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2srraridz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2nqobzghe.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wpmxsaki.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pqvsagih.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jnusrzfs.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rvpotzqw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hnpvdsgp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ccpfgtul.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2namumipt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2oznwktxl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pagonvvg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hadktkmc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2sglakopa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zfvthhcy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2kyueifmp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cyxubwhk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xuuamkbl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xavkmlie.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uygzdzyv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2aqbmzgau.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2novpwgus.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bqgwtyau.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2elbesaan.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fwayuscf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lrqykvfm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2mdlljxje.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2gihhojnw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nvoybumy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fdavguhy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kyssapjp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vioqekln.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2foygtwvh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tdbxgpfk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mfumbdke.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2sigdqoqq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2mbzmhejr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wnhubvvf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2okrfuqin.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xyzpdpcy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2gpfwjvoe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kpppjfwd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2dfdlkusm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wmvrnwkd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2buepivdv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2hpzdoxss.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2xijscjaa.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2isyzssiv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pqhticdl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ccipufcj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nrlctiem.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gfawlqzc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vrqobkjl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2dhwqckvk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2upjaqdsb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukbqcnyz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jzslfttp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yspqfhsl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryxpfakp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2jnhlupxb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2jcwifnou.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tkcobtjj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2utazieeq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2uvzlazht.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2payiutvi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wmcxcmbr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2btoiyrhb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdrloubu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ayqpymsp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rmjwmqwe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2lpmtzyjh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2btqdlavm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ajtzxrhl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nbssybkh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2edcgaxnh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lggsmnii.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jxsyxoum.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pgklishb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pcglnicb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jcrqdmpw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2zbyzkoyd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2dynatlvs.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rkoqqdqk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yuqabsje.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2rsprpbzn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2miwcsnnu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2owtnoffa.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2wxegdgxt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fppubnnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykfjkcjj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2jpinmeei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqeapgrm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2oetlolwl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ofmrwwor.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wxebmukf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iqsufltl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ikfjhkcg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2bnayfznq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2krgeedyz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rjziinns.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2htbniuie.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2yqyynawq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2elajshix.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2zibabkzs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wxkaomzh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gbyaidmj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2pldstous.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ywexuenm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2eubcdvou.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dfdhbuqc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2oowylejw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pohplvbr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pfiyanea.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2lcvksrbo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qmipfdhr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2buvhxjmx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fnbfarhb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2lqnlttcs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lyqzimnz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2spmihcpx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kueqfptl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2cercjamw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2npzfzqxp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sbtpbtjh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bazbdrjl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bnhmvgpt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lsjecsuz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2alwjurnu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vbrwxsqm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uaepmcla.html


<!-- 参考信息 -->