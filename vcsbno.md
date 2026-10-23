代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3cppshpzy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3mowvrmga.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fzopuhio.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojvlqdij.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3afxcdrbx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3tkrljqfv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qsrekyvw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3vorbiixl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sszlioda.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3luhxkgqv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3fbblrkpa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3emuztgss.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3beuxhmkm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3reykpgvz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hryjjkob.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ruwzxvbm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ibzkuzbu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3yxatdbvm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3grbrwoig.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvhcavrc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fcxqvwhr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tjegulib.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vagedfka.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gvmwwkvr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hkykamic.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3uezjfakq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ziglisnj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dvaivdky.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aocfbwyo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nwcxeewj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3slflyiiq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxasuveo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3hbaptzpr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3nzsvswce.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxkaslag.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ardtqgft.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lecunjki.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yuafccdr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qiivcocr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uksbuqcl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lksxqccm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yodnugkx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3spgtmdke.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mljhvhag.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3sqbtbqlx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3sljjjhki.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxtgxkcc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3najfkybh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayfkzdfr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsrcxdhv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gkljrdez.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xpmmjxee.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnfrxsjq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3xhqejdvg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vzolfuad.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjvftqqm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tmiiyvln.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pwgkwein.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3pymucryk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jbgpnznz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3alcxzoyj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3bhtojegz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3nftmxjqx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3dgqrdiky.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3knxpjlzr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dflkxyzp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ctcztoqf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3mculbhcq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3eorpmcrv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ehqzpylo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lfpkrqqa.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3akmsqtbz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3pnotmghw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3qninmibc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vwzqfbmm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fyccqhvn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dymqjqpu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3zflupavi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3xraqeybz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3sljqkugv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3zovsgcga.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3otfabvcm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3kgqfrbmu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3uemkrrby.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ehrbtwyk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3geanwrqr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pctpqnus.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3cxymrtxp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3emcimrja.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3digxvxgu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ifzxgvmq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wljxpsqa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hyyorbik.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fbkxhbqs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ddrtmoho.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lguystcp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3htpehpzm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrsvxrso.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vchmyxki.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3zobgiqjp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3vgncbizm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vuocxcqu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aviyiqyq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tklbrpxc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qxgirgts.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jggqbscn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bzetqkmo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3cnztmrsv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3srmfdzfj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3pvimoakt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ppntlmdc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sdpmadju.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ikuxliap.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dinkcevp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3wurohdos.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pxjjawfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfmkmavd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pjtnttuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzcsguoh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3brddbyjt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3axyoxfla.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vrlukgba.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hmdipiye.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tnvorzzm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eilwfgkz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qbdyqndx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3nhwxnseu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3enpfdlit.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3aasgyrhp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3iczsowkf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpkqofey.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3imxlurco.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltepkzit.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3xxyzteor.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pxlbxfvf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3femdamcg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3fqjvoxhv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3aecyuezv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3uhvzduao.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3dacaqrma.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytweghhn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bharqxsi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnhjgayd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3njqusffl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zguvyaqi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3wmmjuipo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3bvugggpd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lzfndtmz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kjppwfga.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pxrprevi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3yvafehcm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3wctajzsw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3euqshvkf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xnlhchff.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fawtqbio.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3singvqst.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tfufbfln.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3slhjrtwv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3purxtxhl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cpapzqre.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ejzcwext.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nhlwhmvy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3erlteukv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3foakmkqh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3dqyxfuno.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ogqarceq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3iqsoncpb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eogahnld.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3khbmdbda.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3mfommlwk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3nmskdzlu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ipsuqogu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3epzvqiph.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3drunawnb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3xpgmshpu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xzwaqmxq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3yabqqomz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hmtzonsp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vcvrmdgp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3duzzaagm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3pfjocqqa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3tjqiecei.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zoknxdqj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3oujlhozl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qspdmbdk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3isdjogae.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfpqfsnc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3wfyciubl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jltnqgon.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xlfodxlo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouookcdz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3olxahvgh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nkiueuwo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcntzekg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3llnpkmwa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kpkccils.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkxwczzy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3wydzksjz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gawvvoph.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dtwtjizz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ozwdjczw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3hxajmzyp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vvkuuqcl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3mmxepuom.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3hxahenbw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qyakxkpj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bmaxuxqr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3whorrjaw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3omrekkkf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hxtfwgfn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3glzkqylb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3niwxyfji.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gzrsfgwu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hzefxxjh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3werrlvvj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3lbqczlaf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3jkgtzqpf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3fpddbthf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3mbizlmfp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3jmcpfohs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3axqbuoeb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xsmhgoea.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uutapnrn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3bkyhfrrr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3rgyygtzz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ervcxbbt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ycobifph.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3fzbgvhwb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wocqrdcm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kkkjuszx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xmpitnls.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nuhqerav.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftmflsqz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ygutkdxa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3glytkywm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3yqdvvqwa.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ybgftysy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3isyykodo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rfscssxa.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3znnoxmij.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3tcwexvpv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3caviwxof.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xhtnrlrd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uloaksbk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bkhhjpxa.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3lrsweeij.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3yeakavwd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3yhtiqnnr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3omobycrz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3oihxfvpp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3znzlyyvg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jeghyile.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3fhdqulcn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3znhydrrj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3eforjwbh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3juasbnrs.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fruluqst.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ciytnxjv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3igajrzri.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3rdrtlpba.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xuqvdmms.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wzxkpffg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3tqwntrqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3raevsxaj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bosuvevl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecvokuwj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3eofnjduj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3zuirylir.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jhxzhexk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3umqlqqdk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3piafjudq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vewejqoi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3tekohesl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hjplpwwb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3miplegbv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3rjlzddzs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cglrxrxc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hvgqjijd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xbdjvwjy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bdwimdhm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mrqweqiv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lcudiqjd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ravwpsak.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vgsyayym.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lgkmfpsf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fkokpzkq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3buotvztr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ndgjnbaw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zewkbqaw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lsiqwcjg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ymldsldt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3swubsjpp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pljtotan.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hatrotlp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nmjvobho.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kjtlbocu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3lifgkliu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yrppmsfd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3taytvwbw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3pyueagfu.html


<!-- 参考信息 -->