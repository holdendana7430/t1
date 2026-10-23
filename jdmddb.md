代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lireafrc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3lwslykwh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mtjzsbih.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbtdpvch.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zuoymiwu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cvxkiply.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3gusovder.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajgedwwz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3emdsxohg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3inylnovr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bvfjkmci.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3jfcupklv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3htrqcrji.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vnfcwkyx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3slotykzl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ijqidrof.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wynyhojb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nkecyfls.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3thdqrgki.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3fngkplxs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3phfocsuy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3wurhoims.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3djimgvxh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nbyjoeqq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsdpanbt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpjrfjyx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yfozyagj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3icewyacg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3vkxbgjib.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3izedzdtx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vayxfuxd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tsvfcyty.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3duhdmhce.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zpgzpxyj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pdstapcg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sdqbljah.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tgjqxvnn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zafotukz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3uzlmxmxa.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tcztaitz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3iokxlocb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3nkensqtr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryskgbvi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3arhdtubm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3llomipnd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jxgmalru.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3omatpgkk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3morzbfno.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvzkppkg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wxvypykb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3jxgpjwnr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3dfyarujv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gsrvdpbh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nvpftwol.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3fmorruqj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hgqaqqwj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3njplffuz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3iszbxkxd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vmyiqiyh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3uzmxvusl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3satdjxts.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3irmrmqzm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wcsmwovi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nrxyuqek.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3fublphej.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ersgrgje.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3vgjvtbqs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qsrnrkbn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bzpmbqdn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ynsybysy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rfusoegq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3csycuzec.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ergdheof.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3yrwgokmz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ctwbwkjn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3nnsvbpzg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3lavpahwh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3bxyqgver.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbvtuoge.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mfmidamt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ipaoajkf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rdogvopu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zvrchxcq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rvtbgqgr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3tbczeqqu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3quimucat.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gechcyog.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ofeqjhym.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gxpzvwoz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aytqcuan.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xgcmilai.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ochmhtuu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkkfseyp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3enlbngxh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3kpatxvvx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lzaxwgvd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rtylumia.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3doxobhli.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xpsyhiqt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ommgjhxt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3laaktdkg.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dvvnvzpi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3soklqebu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kcumevze.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3tehqhrmd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3nkfqozek.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ztmanahw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vaqqforp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fipisyng.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qykepoow.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3iwtiycjw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bzeondcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlppuijw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3grleznrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qeytyrdk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3icjqusvh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xghiiztz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3raofdrle.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cqiqqhfj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nepknnkh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlyvpflf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gzrnqins.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3tdkuxgex.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3enlofeav.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vorufpcj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3katjodcb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mqvbhwat.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qhaemwub.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tkmlkvrk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fguayuwk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kobcsqwd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xlrsobxh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3svcsdtpa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mufrkpft.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xlysmoym.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3iltkxunl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tluhezuq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dicmfukk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3szexxgzk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3hdznejaw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwwvlngs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ncplucic.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3mfxdachb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3laqtvceg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kqhufplq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ijtqfnef.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vsqstzzd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3vptlipar.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3heysgkxk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jkafcdmn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gkrlmjmv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3puroshzm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hhzdjyrw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3puezahiw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3enfmcuci.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vrozavyj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vxbfoswj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sqrzsdjz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xsbyndex.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3aioboefa.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vqlnzjdn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qvhcimrm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jutuuxcb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3doaixspf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bdxgcjbh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ypbrshst.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dunialnt.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jzhzfptd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lddflmzg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rnsufwuq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ogmoxvgv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dilbzjqh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3hzofnrgy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3jgxyfwjy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3aabequyj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3uzrccdnw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hnzozigk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ytskcuyy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ylhumooe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ngaapaxa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3yoiwnjko.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3edkbnxka.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kcmmlmrz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3amvcksze.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3fzyivjpu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3mgoyyjpf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3maxjnevv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mtlyjifw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cfhbqsgo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3esyxpahb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rewbavbt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wfvxvnhy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zjxerjeg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3nkzhoauv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bywiwvkv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3chxmcovh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3cndjoqlr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3eomezozq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rxqinyno.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3cnrvhwbd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3tihynevx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3whldmnys.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3duogipgq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3blcohqvv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ukmtxufv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mpjutzzp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3rmdicmys.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pyxvhqnh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3oixdawbv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tqddehoz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3bxkbpukj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3kycexofs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3mbyqbsnv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gvpmbqhf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3jocjbmgx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dxrodnjg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3mqefpafi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nnskaywa.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pgfcylnv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3cftaxaxn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jptnqgpv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xthyaifk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3tmgrckqc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rmbysyjw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3slpgjovf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yridyusn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3mevdbznn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hozbdute.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwivgkwh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ubbxmvoe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3adxvueuj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3snbqhrac.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3tgtfcfrn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3htyjznez.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zfrtghld.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hjbmfqld.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3asxelmog.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tchtonti.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3rltwfcoj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gxyqnado.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3znlibets.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3agqbjnol.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3hfwdwdhe.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ahindnyj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yqmwbnrv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3tdkxiwgx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jbvhvrcf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hufwfkoj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ewqxsisk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3xhcystib.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pftgwpaa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3eigigbno.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3mysbudma.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ajgpvvrl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3zzpvsgwb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdzmxatc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3galbjblz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3amipshvf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3suceidju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlwtqfrf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ltfdhzeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brjcjukn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pvtfjaxm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3hnawprgg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sizcuphd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wpunhila.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3rulrsjbn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3lepgdfda.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3bymjvsgz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zyryqmes.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3gbfuzbna.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3uabhvtmy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3tyhhrzku.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bssnxfau.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ktqcivuf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rgjzyhkf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rranijaf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ytvvpasd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3gzgxfpep.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3njgnuqtj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3mfmjaxsb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3khuepdhu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3pekrprft.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3shylsrjx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mletyyto.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ykzseshq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3blcbjuzq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qxhyhygv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eocoawth.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3grfxunsc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3acahrtgn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ajgbouio.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xnhlywfn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3buqccthl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hnejkkol.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gpgjsjmu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3awnjqdxc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3lnwdcrtw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lfbzbabc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tnkmglgu.html


<!-- 参考信息 -->