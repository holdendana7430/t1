代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nsbdqwzs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3enctmrln.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ucqjqrwd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fdyxppru.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ovfqdbdt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ptylkhry.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpjjurjz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmpgkoho.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fcyjaddk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3uogbaylb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3yvmtodti.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uuaosrug.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hfndvoda.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rhthffhu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3aainsswh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxbkwtlx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dorrpsba.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hnvjdaim.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bxefetsu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3yozlgrfz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhxeggyz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3iovtunmy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rbeubbuy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3xlsjirhe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnppvenz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vzdgdyei.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsvnvnpk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3juowxdjj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3htcmwhag.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3pbihfjei.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gebwirfu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ftgejamj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3luotglfx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3agnikulq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnsybilt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gbjgonfa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3nnrmqoxn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3yngmcrwq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ejhzhjjp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qpksxewr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3vyknfgoy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rdfuxved.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kqbtwiif.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fldodpeh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qunpdhjw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vpuqufrm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3iygvjrao.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gpczyykl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3tnrbxxji.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3emrkragw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdfjyrrp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3meggpicm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqyfzrhi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kmzxovxv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gjekhgck.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zzeoewhz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fqqevjqa.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3izmeiaku.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3txmignag.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3wbyfecvx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dywvjvhe.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3chrzbheb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3apebgwum.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3woujjuvs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mtrkmhnj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3juirmlaj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3viwktxup.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qfoqsdbt.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3bhlzrrka.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tbwcttzj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ghrauqwd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vlguxlzg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3pwyrtzwg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3enolvjbf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3dzzywrow.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3brbqjxqk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rjpyceeo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3liodqdjy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qzizteoo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xxdxchyl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bjifunfs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3kqybmlck.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3intmxrts.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vqjdxklz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3qwmqzzzj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3xgarhaaj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3oleuqwib.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgfkhmhp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cqjbqfxr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kodkhtje.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ogwmopdx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3rykgtkej.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ezfezxsl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3frxlngzp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3mwzhhjbn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3hteokqzb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dkloqfwg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3empacpjm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qbdrbmim.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdyxhkmy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3foyhwkad.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rrnnvupy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3bisunbms.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3oarcbmzn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3aufdgkdo.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nvnowkvb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ivpamkrv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uldoswbw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pppvcjaj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oijzydot.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dzxwfutq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3sdrsjstb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vuywwcpy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3gwxdfrtf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3suwubedn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fqbythvf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3piknznqt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3qajkdxap.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3uwuoavnw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kvrpohkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcmfthbb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pqarprtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ualqwpkg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbmqbvod.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jziefumz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzqddjzx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqsrnzrc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckafzpdk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruktecgy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jielsulk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xgwxfqay.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sidqfzfq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mqdiwzyb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3idbqdxvw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sudyntdr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zurrsyni.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xagcdxgp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3craenssk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pawgnawz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3boympkoy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wgrooyjl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fpvvhxrm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3oruijdvz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tqkeuhzp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtziivom.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nuehfyph.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlziqdyg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3wvmxwglw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3hbomifjc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lwztumtw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jtcvbmev.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3iaortllq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dgygkzdu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fjzicgjx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3oqqdjcwp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3geuogcbw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3nttlcbtm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cyskjegt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tkpvxhny.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3jdihusdd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3aihekmgs.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yuygfpyc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cptsyppu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fymksaeo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3qiwmzhgx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3aiqcbhjy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3hktvowba.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3fqdrfryv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wxsswkpi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rdnoaylw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bxvvmrgx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nznekpqj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yggtgstu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jjmcuktq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3syecedhc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zcjmijnu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zvjxgknk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3kofmtmcc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3njuczdzp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hnciutoj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ekuchypg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3sidbaenp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ijiuwjdi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3rhidixjv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3gxtbzwmb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ciejjglm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3rbvcbqlk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3irghxdmh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3pdbowwcx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nmliwweo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hpunemdv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xyohgxen.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3kqmxltjq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xhvfyzwf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldoyrbxg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3optduvnf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nshyabaa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3svylinsc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bkkwvtfp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jhhakwyj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3imdvbbnk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3harenoar.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pitjnlvb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qbhmvxfq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3nozcveqm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wsyqpgua.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vsduorth.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3zwlzadfb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ktrczdrz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kdpmmneo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uabqtlko.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3muoqpznf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nnobdkgr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3gjtbjuke.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xkmqgktm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3uorfhvld.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fgaydajx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wodwpbas.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3muhrrbsy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3kavdtbio.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3yqwpfpxd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3zjuvdrhy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3umytnftm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fwijwswr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3aucqfjim.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hbwyshja.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3blknpxkd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3yaugatbt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vdtrofjg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3lvleeqfu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3roylirnn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3msxehhno.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3nkfbxxta.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3whmhzaty.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bzlaovoa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xfhrpkoj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gefsooug.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3itabphmt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lgzndtlk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3zfpkluwb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3mpctujux.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3dklproul.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3knqbymhj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zzfspfav.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3oullqnyk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3syfqqwip.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ilhicoyj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ppfbfifg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3omqxjicl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3sccviudk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3dhbkgmpf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mcpotxvm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aepiipzz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3sgnaghar.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cbseglhx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zizinwmo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3opouqawp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3urbluqwj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qdzxtggf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bhtxfhfv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3knnryuag.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ojikjixs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3fpotezxe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3bnsqnalp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3oecmshpn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3rtleenoa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwdbyaaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znisbmid.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3afuyrvtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvvalyya.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bewwyyli.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3nrsbhkmp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3elwmdyvw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fexramve.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3mhdpcwhu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3gnlwazyh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qwjjpeej.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wgsahtzb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3gknwcsww.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3gazahyfa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ldsqnaiw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3iqzqupke.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bgvlflki.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3srywhwzt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3epmwbcsf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rnndjiup.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3uuzlvqak.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3cyiyyetm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3nfykhedq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3drvfjsen.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3cbbdnvpz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3esgaxsvb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ouoboetc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3papdwajy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ojopmshh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xswzvlhm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zltijipr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3euiviphr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3muvekvts.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwpiknue.html


<!-- 参考信息 -->