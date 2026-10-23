代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mxmmozcj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3tagawoyz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccdvphzs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pklypzce.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxtgxxcx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3liwpqigt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qkvufuqg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3buezspom.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3kfabcueu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3vrkhjcee.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3yinsmnxr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmqfgxqk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3speiybde.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yimlqfyr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ronrlkyh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3sbsidust.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yoqcwlya.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3oiawypwq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3flwrvucl.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jnskdtic.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vphwfphe.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ggweagei.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hepjmpeo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pixzdvyh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3avcoqhum.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fvrjbhik.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mojwsgiu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3laoizxly.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ijfygteb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qetqbznf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mldsevvs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xussedtv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mratbzkl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hamvgdfd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3gvalaxkk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xfonkmqf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3lvtpcgal.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3umbjaaks.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pmlfldkm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zvvjhpxy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xkkrolhr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccmzxryh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gfdrlxze.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3fttatyoc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rgqjvgzw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mmghxwts.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3tzjoborq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlginjmi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ndqqtbqs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vvhzulcg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3jezhdpln.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3caqibcow.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ndfkgrxe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ukaxjsmc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ozenipcy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3uxtjyqwd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gflpmjnh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uapenfbd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uxncapdg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3nanekdfk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3diciigxi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rbsuaodh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qeyxfeud.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3pyzqajtw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3uplpwyxt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3kiwczpoc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nxhitxek.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uspytlgz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nymbwgwc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3pbcrfvdd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3foyliufo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3cvdvafpv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ejyxofhc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3uzqbvmqp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3enaaezfq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jbtclkhc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cqgfnsdo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3tqojtuvs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3bqayhykx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tucxcqmz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3kqwthwlv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vlgiofqj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3cjayusky.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3dodauvkw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3udssqljt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3legjawcc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ldsoyybu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xsnasthr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ucdhlhho.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xtwqbyiz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vwkgicts.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xepaxats.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3narlkyxp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sxapfxvo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tatxseih.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aphpxlnx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zvukttgc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jwioqyib.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3onsuswau.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3acdxbnmu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3gdzvdbva.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3otkknslk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3byhmkzqm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ngjicbce.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wusbpehm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3diivqbfe.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ofmogjme.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zgimsspp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zuojvsdh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3azofsajb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbsbcrku.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rocpgbbc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zmcuwzea.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xgbisjjx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qsveujup.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3agktqgfa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3daildkrn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3vvmskalx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3krqdzrcm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3swsdhrxw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3bpwlnpmd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3wgqbhotu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tavzxtyo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3atmrsshm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3urapqbpc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kwkcpmiu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qttsezew.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3gsujspxo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qrqsynle.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ockmnoym.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3yftlpdby.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hiijihbb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3szyogknw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wvslylce.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3zseueczc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3smxynptx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3vozpgsjl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3rgtjseef.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3zheeqvfw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3idxtkgvb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dqzaavfd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymnsztde.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sjfievsr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3iygoiuxy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qjirrwud.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hiymnbjd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vyhpefpo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3yzlptmqe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pursirqe.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mchsscwg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ilznmlue.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3iqirhfcf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vfllipag.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pcturjhx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qowdlrgj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3fmndhgys.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3opiwkgok.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3uwgxxrdy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3oaftbvip.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3svsfbitq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zejxiqoh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3yyoqgjku.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3jqjictwe.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ulyeezwm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3diadnjkl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ssifeawp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hhmimlwq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xdcijaro.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ssaneabf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hlqriojo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3efmfrmre.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3pbwsbinc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ykfgykcu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3libohwog.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fjzwpdxx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wesdkzum.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwezmgon.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pklyobtq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wonqgdoj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dmeaaqyt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ikmzwibz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3iimkdyzf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgyxfcat.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3uszjovqi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3iveqeqam.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3huwqoyun.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wfgxpvwn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3osrvyzcp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ucmywnvy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3bcnfwrwd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3knqsxhrx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3syxjatgr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xtipeyyf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3iavwpqzq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fwmskavp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3lyznwgay.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tnvblqyw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3htftgzsm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ucickcru.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3pirmofjx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bpzezosg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jlzqinww.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3zrewwuck.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3lbskuqfg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pmsnslle.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3igyczwpa.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fktztyfy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wbctuoxg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3caefwhqz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nwcupssa.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ledpvifg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hwxlypwv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vkgptvpz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iefwjvnq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3htbltlci.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ybqvykwx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zsbnjuyj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zbulxkdu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ahedbiet.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rtineqsk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3lvjriqti.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kckiywuy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3tpuykflz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmjxywoe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3njjsvguf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3asextumu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jsctdtqc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3jhwvwxqk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbayemdp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hotmeaxi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3avquoilx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mdxflmao.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wxvjlffe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqhadfpn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rslpqrxh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nucvbtsr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gheewubf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ajbkpqyx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3qolmabct.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ulmiqkqc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyktnbbo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmupgrcx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xwkualod.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wpygdjax.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3fgveysly.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3shfnltyb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3jigftgnv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mdgktgbh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3olpozebx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3sfohvurl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kiclhwyw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdowajli.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3issyikdd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3avydjadg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iurshtdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubpnyuin.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ehaptpbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qyxonwsa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xbiudfve.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3hjpxnfzm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nvhgjdpp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bpwyvjcj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3iahemhfz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3sbfpbxmb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3leosuitx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3glrycaoo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3yapdvjrk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3qgtqdzhm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ujxjmmcu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jbeffyul.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3llqemqwp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ssnawcvf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mkogadtn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nbjsuiko.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ytlhlbpm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ghkbtocq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3opupjyim.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qkjijilm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3yrxtnzlp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3iznquemk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rkajjsjf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3axvagsgz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wxvpxhdd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3tmklppbo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sisixcgy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3fdypjwrz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3tcfevrrp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mnfzxcph.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3yljwhrka.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yzxmuxlo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jzxmvend.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3vmrscwdn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tbycjxxh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vmrtbumz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ifayeuvk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mlhqispz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rhhgsnad.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iomfyqqe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3atmqgwwy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ogrskfui.html


<!-- 参考信息 -->