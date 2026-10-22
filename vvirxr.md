代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2czxxyaoy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2spgjhdjs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2uladrqwy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bwrlhjht.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvqiuawb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ynrnvmfg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lxajawpb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2uabpafvy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mputgjyb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2aefkywkk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2atawzkzh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2usylzawm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fpxmdkoa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ufyukdho.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgfqsvkl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2acyyxcut.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2hmmbzttf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2thrpdiwt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2obldleoc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wxpjmran.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qizaybgm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjysrdxx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdatryrs.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2upmvqvpo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2laidbmfw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2pglmkfad.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dntungts.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nytrmlsj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wkialqvx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wdgllexy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rbhjthvk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ojhxzwjx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ahijnxah.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2girhbtbk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2oqkltjib.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jjllygut.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ctsiwqrd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2mtponepo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqzugljp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hstxdsbr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqbfgmmv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cbqsixrd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2eaedbrgj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2zreuuvup.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2meimuooo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2pljzdpie.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2sxiywizk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sflcqfau.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zntblpby.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bmqynpih.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hknqxuyw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2einkixbs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2cggjxmys.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gcwmnkit.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gstfujhs.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vplommpm.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2pxblugsk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ixfwbqdn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yrnvnivs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2prekhfff.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jaxdbdon.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2jhthzisx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2inefecxr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zqjlhhxm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ohyrkfxh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2fskxieps.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xptvaqwi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yqbbbdhq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jsjirhbj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fhwqtbda.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2pblacfrn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xpuuanhy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qvinmafz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2jrpzwvye.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qpwefpta.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vxecjchm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ijfofnrl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ntynlppg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wavattck.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nbvbvsca.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2tnwiceuu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tbjgvkiw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2kvgrbkpv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2lnloufbj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xdpwjids.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ydcbnifm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jgwwaspv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2jqhrwmtq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2aweywyzv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aftrumwi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2pckngbrg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ukqlmxtt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2xzxvvxsm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vxpbknpd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lwmamjhr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wabvjojj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2urpaebjs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gtzccljc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pjkxvcsv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2vqgclotm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2agucbqxe.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkhpebkw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zujhlfgs.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rfpmftuz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pncccnki.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qmwdtydq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wihptkru.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dkihvysb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmedlxtc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kyrfvnne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btriuwct.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qkdfxnus.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nabhfxcf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tlsjqugr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zbrucoew.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fpqnchew.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yknqwlgy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wdnatijo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tdhorffl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wqfpnbsd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gjpbkket.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2daglcuvq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lblqoqkb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhxdwqzj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2afrvpdff.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2gphapstf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2nmwqqhjg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wxqdswwx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2dfwrfjpy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2llsyonqr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2wqktdxgo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2brlicocj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lptqckgj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ktiuzinb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjozslfa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ogtfqzye.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2sgcjdcnn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2moeqhauq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2iyyjyiqj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2yrlwkbaw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cyedttwp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fxdunxyu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lsdrljfq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fnuarzdm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rouclfcx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvvhrqvk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tdikxzef.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mdecmwuv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2oicjjjkl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qsdsloco.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fbflragp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bxpysmme.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ehywhfes.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tnfjnorf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fqbvtwhr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hwecysft.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ciglxeqo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2fmoyctab.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2sgjzzhbk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gprejesx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cwqoskez.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2hkwatsnh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qtkzwqdx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mopfjwtf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yytrvutv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2jlixanfi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2mwsrdqzi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ojxriwpx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2alvwkubt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ecngptmw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sdimdatt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2auechwmq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2phguiejc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2rritsgmf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yvtzjzku.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2szoptlnz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2iytmtqix.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2odawobek.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2srcjhxfw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xixrfjen.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2weobucou.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2bsqkrnwb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqnpxxpw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2mqimzpsi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cftswpin.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2khlelqfe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hrmxbkfy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2etbzgame.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlcgwrnk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2rubltpmh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mdymznmk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2mncmjpig.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2iqeeczew.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2zflgtspk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2bqjxfkvl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2yzvfmsyp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cguzvdsa.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nwlkpvpl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dxwolcpe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2zdbzexyj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ofmdewss.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2vgttewak.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qojueazo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2qqzomvyz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lsyhslrq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2pquvelwt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ksiccmxs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2cfhwmefk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2elgylsgd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2khhwuzhw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2cfmhxhsj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2qsdyapnb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2etxrbzcr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rfyulacu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zmrqmaid.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2blqkohtj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2fcqyzeev.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2pdalxtch.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jcaovuuz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2skwanbdp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qtcsytgr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbcbdiua.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2cunpohob.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ashwsxra.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mzzmhext.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hqnqihol.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2csgwscwa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ezebxoma.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ycmkxvxd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2laekeykt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cvydwwro.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yufjatov.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2okfyrwzn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2qhbudkxx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ctnkyrwc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jomqjkdx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ijgydjzz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rzfvqlmu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2pskhmspe.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2saenxvdn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuzgqjad.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nesdhvrj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ycnmgsuf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hegaentd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hkoxyrxa.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ypkwxute.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2podmtzgh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jrnzpxud.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2tsglnmof.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2gnjegtjc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lwgaepnu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmjszoah.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2sdiklzjo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pijhhrhv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucvbulrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czaziszp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ucxhtmsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcseigvg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xhllzmmb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lgqngvte.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zjcdrohp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2esprezqk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2sqrtfpue.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2jeknitsa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qvxrpcpb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zxrdirwo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2fiiedrtp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2pvfajmrp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2sbcjwold.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2tbwrrrpq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qbxlxbps.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pxsygjlf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sgdyfrbp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2autqjcao.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fgobrjrx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cawkhljq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2dkfkhvkx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2iyxvpdgr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2yuxowqbl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2yuoqayio.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nbcpmcok.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2elwkojhr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2lrbjljeg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vuyxcneh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ghlpsuym.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2afpzorwx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2guyoinyw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yllpeklm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2phdqwvjm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2mlhuhmty.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2spjflepg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2otaoidab.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ppmhkuju.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mtovromh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2evvachgc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2huxazagy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zfeudaoz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mziowqcp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2nxhpkvrm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2igcuqqbd.html


<!-- 参考信息 -->