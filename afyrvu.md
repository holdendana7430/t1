代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fzubgaas.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3sxmlrgxf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3lsztkzei.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3opjcdrru.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qefqpqza.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvvxlytg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nkjreumo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3iynkajon.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ptloursc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3isyoanqv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3seteqqid.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3irwhimdm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3slyfbxqr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcrdvwtp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wrrxwuul.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3kdpgtiqi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3zbsuldgn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycztndwd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ltwvcfkc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3nabkzxwp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulamnshr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwubhzyf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eohlzgtb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3amsbvkol.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kpkstadz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kvtanthh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zugcdwwe.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xdkhirre.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jthfvjer.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zaqpwtmk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dowvdzzi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dlibonkg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vnphjxfh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3momuapwo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xhbuzomr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sakuydvd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3mtkeaqhd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3mzmgeluq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kmftbajr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hxlxhhnp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pkkkkemw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeimdhyk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bfosbigb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3yzkeaisa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldhqgvie.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3shjkvhjs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zaibbocp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3igkowadr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xxluntgd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qkxhhutw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3shwlwogf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3kyoisxeq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3mtfnkhcc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3qgpdlmye.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fjedkjtr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3luemyfla.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3swgstjyo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3aogwvyht.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hbraswxn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gpgfwkyi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3nutjpsrs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uzkxxeqd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lbaafshn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wdffupas.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3htvbxhet.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gnnhhzef.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fzqfgtej.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aauchfzn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lpjmddxn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3pielxeas.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jlnulgbo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vgrqculh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3iedrxnrb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3eyzkhchx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3kngsxckh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujaqedig.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3oxuntskc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3vsgewqzv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gxaxwyvo.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3xbynhjws.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wvanwykc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gqmzsowk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dapuvpax.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3hjrafmab.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ttbcimsb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cavqsvyi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zdwavfsj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pnwznqui.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jawzinph.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ynzelclv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3mnvdwpar.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3jbadudhh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3jfwaxmfi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zxbaohjr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fkllwgun.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ecvfvyie.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3urxydnwv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bwupblns.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jjhelqxj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3twleqdny.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3qaoqxokz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3khifvrts.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uxkysqrd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rzfxptsx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rnhvlyge.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ewsejztu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jsbpffpt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bbdthqmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xeddeoqv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3sksfekvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfshrnpy.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lzvfbacj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nwiwdzmn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtfufvxl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ehglqaug.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejjrbdae.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3okwhsxmn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nunlxsjj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3cggjpdyi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aingpcnf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xtyjwyqc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ccsyhqaq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykvfamvr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xatrlios.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmqoyohy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3dbbedjnu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3bjfozems.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jrgevsyh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ofewfovj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tiotwivp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fxmpwjft.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3otplhezl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3inapnsjj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xwcaespb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3thogwfkn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3fjddqdbe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3hhjkginj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3nvibftjo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3cooefodj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3kgenzkbk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hqyamcvy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iidtnvpc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tvcefbgk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3dtwupuxh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3sgxqjrbb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gsngmros.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hyssdfvb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3gawflcrq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gddvqbak.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3osiinpne.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ycigoket.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bpsrsuaq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ohdvsamv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fmlnburb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3autkrekl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3qfjengbl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3wjusyyxl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bfkliokf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3slovwnvs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3miyucskk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bmxyyoys.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rronouxk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3bimzudoi.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3sdwoicda.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3potkwzvw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3cfbssaqw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3shglwsyk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vkusajlj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3tlbfjynv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3uycivapr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3znihyysx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3elnkrywf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3alcswvsh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mtcipvtr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zaixhkbr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ivdgzqea.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3apciempo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwmqkbxa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zahxzcek.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3tgucujvk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3tirnfuqz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3auejyfnh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vacwmuir.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3vwmhepmx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3btcavuug.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pusyavcr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3uajaccja.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dywezruf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnxtmsxy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dvogvgkv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3btjvypgl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jpvjbvpl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3adbwfnbk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3mgwpjevi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ivwwcwpn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3qmedgpht.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nzlndcub.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yagrbnlb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nrkbywcs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bnncbkzq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ssqtrylc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ronaqzfn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3zhuuxdax.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3gepjufqj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pxuznoym.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3fincmrfz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3guddkgnt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3tbutgqib.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3njypcbtv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wetzpjrg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3lcfjmity.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3wrsojxsk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3axgqfgmg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dokxhshl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wggolsqv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3rnajxasx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hxdticfy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zrbxwvjp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3mlsjnusc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3thsevtcu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mibvhyak.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqfmnqzu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3zxfrxqsy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pnwlyuhe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fonecymi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3zstuvfku.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3yguoplxw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3kahcmdds.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3blikcdym.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ajpxcher.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3crhkikse.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pbiebtbm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3likzrtmp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3drfvsdrm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3cvkuzxzv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3riclgzci.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wcqfdwjq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3yrltoeca.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3sgpsfueu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qqmwgcuw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evoffygo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqiplclk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3seshnurn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kleruvre.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jlfkyuzo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3twwhniyi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zzqvxwpt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3roqxwjlo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3cvbioijd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qowsemtj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3aetsmkxm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqynfydt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fjlvagot.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3frfluqet.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3sfqzyoxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bphmwqrz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tptdcojb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rycuavna.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jijresjf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jtngfceg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vrrxstfg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qmtwrnkc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3lspdmuod.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3pysrocdj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3efyjvgxv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3oicuwecv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3clhggvnh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ludmtcgu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3resubpjf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ubmqlcir.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bjoklhgo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vacfuubq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3nziopqoh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ivacllee.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3sjrtfedw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lrzjsxzv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rvgydbwp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xzbmyrjl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jaecdffp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3eewgvggw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3szdhvejh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wolytmsp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3liawwypj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vqoztxrd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jmepkgng.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ewmkyaru.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pqvftjee.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fyxjsmzt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3wouujgep.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jdmfbigr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ufpqqlnh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kiugilgf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3irgjicpc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3kwvzxplg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3talfczne.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wcmixhkq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lbaikhtu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vklszknk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qnbofrtd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3cgxqvlgy.html


<!-- 参考信息 -->