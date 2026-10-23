代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zpdsfptu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3pllsszlt.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3barsvtqt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3riqeieij.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jwkjpwxf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fxijefzd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3uefxocqc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hmohqmwf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xllzwppw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzzwvjtj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3caiddrfg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wizrsxqc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3zzajppws.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3cspndjdl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3sqjkcpeo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3xybqtdpo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lghexxde.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibthfset.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fiuvbzby.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3jvpaaohm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rvwpfujq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgorjutw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kpgnxoii.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3egznntxh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3fxfsnsxu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gguuqint.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oczhboja.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nnwmnsru.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cuhofwkl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kegzynfy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqovtrad.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ukvhvbhw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3cflqspos.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3snpaclyh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bpatfpqz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vqazoccy.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mwukumyp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3owrpndia.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bagffjqm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mlfvzfjj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ivdcdzov.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3lhypuflu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyhoujni.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3minigxjl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3umgmkfly.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bvgazzvm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tythvaay.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3olhbmwni.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rnepqohb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3jkdfmwvc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3biyxwhnn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3mlxgltnb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3irgxyczu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3afwolrie.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3zvbeskhh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jwpjumrp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3brpeshvn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqibvwsl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pzfxqsdw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ntzyxmdv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pjpicmub.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yoteerrq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wpccsxhj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vysbcify.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3opidervp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gjqnuetx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3bkhlzmkh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xtqhhlps.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bllqlrbk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3mtpsqwyf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vyvrgzib.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vunhrbtj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3glqrbist.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3awxuoavl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3enfimmqi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zmzzqaxw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3udkyoyed.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3fcpuyovm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3suymcfvk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lnstrish.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ptqemjew.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bcysovkl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3laiifibx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3vnywjtqr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rnlmmnzl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ngumqmuo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xnaknqyv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3pqxchbqf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpnohbhc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3boduasei.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3loslcazm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ngciezac.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rwwjlxod.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3impeuijk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wpkhneeu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3padtbryt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3czwjdfhv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ojaoganj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fhradaru.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zlhcaqwq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dpjypngc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dcmdfcew.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eodvlrrs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3cpwkiczq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3sjfmijag.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fmwwacvy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3sggozmvc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dmxezkzc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uaoddrxk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3rcuajkqk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3cogdzylh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ewrsmjcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xigashve.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3cbabflvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlfiocax.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hnzypjhk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3gxytqnff.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtgqxzws.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lijfdjvv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kblfqztd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdxjlmhl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3rfvhlbhs.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3texieuxn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycasnonb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vpysvtak.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3lklambve.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hmkvrbus.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3koiiwioc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cfwvtukl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3achgsikp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ajysfsfl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pgiyseil.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3usevjcfz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3imokgaqp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3vqbnuver.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xzauvuom.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fhwyxbab.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ztihgeyx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqvdkyui.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zujsdzsw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3szsbzwwm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3oakwjwjr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3frvijyhi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ltbjqdci.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yzsuqkha.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3odvyowzc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qfttcvox.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3twexdcoh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ubdbbpxs.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbdjbewr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mjvxwpto.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3wqvyanab.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mrfqbhrm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nxifvssc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3grnvqrka.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qgnqdkou.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nvxlqlmc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qqdkccno.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3llzrdvax.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3mdbfumyw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3unfsyivy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3yebmxtkb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3lbroogje.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vezhhzga.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3iaqceohb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gvdmsdsg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3cxomlalt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ieeksyxf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ovemfhit.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3krfolnuo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3zojmldgt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3upsvdkhs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zkxjxsiy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rplamwbi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cwboxhom.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xvsemcfg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hxsjeuxs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3hunejadw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3bgpqfgoc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dacrakdv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzvmonbz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3feqkgxxq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjfoafua.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ckibblwl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lttmygfl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ngsrvqcc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbyrjzdp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3rrluyxkg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzfeojnu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehlnqxzb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ppheicht.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gszatcnl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrvsacjc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ehgaemgo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixdgkimx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pwufyzhj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3umxbyweo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3bopikbud.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bkjvwzhm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xwwdqklr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3grexcbtt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ezpphphk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ufrdbczc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zfmboslb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qwtkivef.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3nnaaeisl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3zfpwychm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3soudroqv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3szazgtjz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3pulwkcui.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3nwyjwqru.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wafnhvma.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3gbawpxhr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jvimhjsg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3izenuorp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3onnmgnta.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zbvwvbon.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mofpanal.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ukmeyfgl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ervihowv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3puvjxhlx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gbscrpje.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ndkqasme.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3lybcybuj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3cjexnzsz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jpiuxozg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3vsvgcdjh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dxucsfub.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tigvvhdr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3dhgpeqjj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3gfbsyucr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3zfmwgsbd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3cjzyvjat.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3bwrsrper.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lbvdxwvq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tpuzside.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3enrjseek.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3tzcbdgaz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3bcspywej.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wmluzatm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ncchgtbo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3yqnlpked.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kpxvaxdm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3suuivmwf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btznrmrp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3guhuanws.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tqzeezuo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hpbxkqqw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tiizwris.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3esrsedrn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rvzmayxe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mqllihty.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3efxlzctl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3bopzrdil.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3dhhiegha.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kdmutqmi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zmkjhtdn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ulkcsgbh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkmqklxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zybtxmer.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3czwejnja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kktktnln.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bzztyslz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3vqgsegvw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sevyhlsz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3oflkqvla.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3hrwllprl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3mbggthzc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bzgqelpy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bgbicnrx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ujbnxycu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zielkdss.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3fbfglrqw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3rqbrvykr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xrtckrbn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mbclpebk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kfzesjii.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ixidwtpi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3fimzwuya.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ikalesse.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ebrhrvod.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3awknjdjt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3kwiprxxk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3cqmwdfaj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3laeuoldd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kbxcuafc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3elpvwmis.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jdqwdcqj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cablvvyp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3rboavhmm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pwtmmwdz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tzrhwtep.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3aoimmyqx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tydplcjm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3offdlxoh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3jixpefbz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iarunogf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pmvdzlbj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3gyppvsnd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lvhsylmk.html


<!-- 参考信息 -->