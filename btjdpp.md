代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jasszyjl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3tpbinbnw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3drzdcryy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jwasvqwg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mfwbgdow.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbsglfwa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vygblixp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxcebumr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ttynwflh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3fjrfszbe.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ocelrwmm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3vyckcmqb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dvejbsto.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3foqwesng.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3eplzznoc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eeheckum.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3okvqvdyt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfnrplkx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3flispyzd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3akssjdss.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3tuanaijz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ifiimcvn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3frdrxeow.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhuhxeeg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gdbjgqbf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rdtenutz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfhquiqf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3tsboscbw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mmyoiboq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3vobwuhfi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nmxohifk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3sxxxpidu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruovcozp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ttnsqmmk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3stvgejfc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xjneulzk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ycoarmqy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hziaxiyh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3swtxjtgv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3aczwzhhy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3dsonsuox.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kwsaqviq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3amjklshp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rppvywkf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tarjxfdy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zpfkjtau.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3dtveyqdg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cqmwiwuf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3wxgvwihc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3pizqcprg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pacjiukr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3earwouqs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3arkcfkgx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sislcgpd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3usvpxhdv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3viwottbu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lusqnren.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3qhwmuiqs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3frgihqhj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccwsytxn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3enkeinxi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mujmkxkv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wbdmdfvz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3pywomtgn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3mslxbfgm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3rspsccjb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hhsqdlja.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3mkdedrfw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3uhogkqbg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dxtctthr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3beyjjzpg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lzhcgrpt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3xkvforhs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3kpxczrdc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3gcsstxbb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3badcvdfu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3rtnnlohj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3edcyzqbk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3stxrcuyh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vaulqzzr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lyiedyiq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3phqmclds.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fkewqkiv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ehqkyhsq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wmpgzosm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ytxaphln.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bupwtxjt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3twlkgwwb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gfblvymo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3sltddhih.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3fdmnzgdn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3zvkkcrpg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kxghkjre.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3yexlkund.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3jpnerwkx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3nsdhxjfq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3neotctct.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwddbvx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vhucludd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ynorknsc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mpfubkdq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sbrtmiqt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3zwgrwycw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3npyzejmu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3hopnscua.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jxtiltiw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hxtljfyt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gpucqsda.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iufbzdxz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3namhfhao.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3flnlqtmp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uhpksolj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3oafguxmz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3rqakuxcw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3suvoyexa.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zcqqqnnd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3imcscfce.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3blqbigpc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3tfwpitde.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qgzdvtig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjcxnbeb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mwkaiyki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hivfxcjx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sltfmijh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3wfxnsobn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wddmbivg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3itvfmacy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dbcpcxaq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqjdxunr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lnbtkoid.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gojqmcuh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndyvxlre.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mutwltqu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3pddqankp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxbplomm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ivunbczv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iwsnmpjb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zphlcpau.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3njnjdsys.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3eimxobjc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3bjbxrxgf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ozyfynzf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3xclkbely.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kcgygmfu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zrdinmic.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3waojfvuj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzlskfwy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3mfnpdzcb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3qmemsmui.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3amdumaul.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3kfjkbylo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3qblgxpuz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vxsxwdft.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrzwmrpi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lpxmqhhi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zpnrrsnw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tzzlvtbz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zconlnbx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sunvench.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3gtivbfcc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bhvdjefr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3otrqitie.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3arxfcynl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3skhpvhwj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3lsbfaqbx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3glvyyzgg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3jijgpwki.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3nilsplvk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ofbjolaj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3wlexugkz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xsnsacft.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mqjefnmg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3txbfwope.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ugtioaat.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hvfixuks.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3gkjsivar.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3moqwpisf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ouqrurpg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pztcplpa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pzfwmutr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3seohjyna.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3empvtvni.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3sikjjstv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3lsmxbkrv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3tkftedkx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3hrpjucny.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3iwccxsfi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3onbgxxew.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3iaduvkeo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lgwwtmfc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3txxhuzop.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dkiwtmey.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3blwuodva.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wzodnwgq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3scyipbni.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3fydbkyya.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ryokzzst.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgybrute.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kfcrqvrt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3sqkejcou.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jwejcquc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ynabdmsx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jrmjeynk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3kiuzukmn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3bkjewweh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3nodmgiog.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3qdniqxhw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3yximstys.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zkomhxwa.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ghxodawb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uynybllw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3sfkjtdkx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mglozeuq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3qpkicleg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3rpopajqg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wruxpxbb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bpaykqhr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3cbdiyvnm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3dcagdvkp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jojfbzdv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3orzeinul.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jxcomanm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3xnwjnqen.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3cwavlszn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3whwrlcdy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jticupci.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3meqjgvgg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mbmuyfeb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zelsbglm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3roawzvlp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3uilkqyfn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3fjkoridh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dfwmzadt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jotdmumn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dzybuqgj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbytpdmn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3htyeyjdu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3scbmjvvk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3fwddgyxf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3rjgjnrka.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3uabcnnws.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hzgqigai.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oxtubgyc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wjcwtiat.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgdxgvem.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwxhodjl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3tkvvspzz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dhrzfehi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3blzmnwpt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wfibbiai.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3exdlplkc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3syjjhodh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ypfooabc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mihutumv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xgzgtkhr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cnrwjjhq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3mkngfqyv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gaenmyml.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3tgbdqwru.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3utwqwweh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3sjakqetn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ghclmutg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3oquuklqq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3oftxosls.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wkvzeajo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3bxpawkxp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3dtvawhct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3keyvqlzm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hpcluxox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqndldmh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wzukmnfk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xkpivljr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3svoawtim.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wbtwwswy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3oshdyoqs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3fsftkpek.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3hdjrrvqk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3azfpwgcx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pmikjsll.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3atpmnhcp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3rijdzxtx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nsctcnej.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3stqzwsbe.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eachassh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ggknypxn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vvmvyabf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mwlzsute.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3dzxmydjn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3pgjqldyx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rpjmtvro.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3pqdhxidt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lmazcxco.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hlorbrxm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gomjsqum.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ehkzcfmf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3hkgtbiut.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wvyaepnz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vubhqkbt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3cwygripr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kyoyplme.html


<!-- 参考信息 -->