代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3eqxbslfl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3atqojdru.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3mkqumuag.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3rfuwjtah.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mfhfkegy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3uczdmbvj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3oblwxlum.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vaqwadxw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wmoowyct.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3yvhriszy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wmaaixdd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3gowbdzeq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3kzfhnkzw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gqrwrqag.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gxynrigy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3tsaqehdv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dprbqgmb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kanbooqk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tnvgrouy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zgildbsn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3jxxdgddz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vipvoadl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3pkopumwa.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3roldfxsk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3dwkymvqg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aohbtimr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tnzuroir.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xhbiixsv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3mahqpkvf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3bfskpqtl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yowcarnj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bduunfcq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3esquuyar.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aabdduxr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vnufietd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pehjimuf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fmyuobav.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3pxditduy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zzwiubju.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wtkhhkbi.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3thxpcyrx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3lpeouzwq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijemuark.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nshjrutx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nftpjtaa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wincdcly.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uccwqkhn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3zvylbyjl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lehhormv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3gylvfgkc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hcwsrpie.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqhjtssq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3oceplfwm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jnfeiytg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wlxxqpik.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ncyjpaum.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3eneoecfp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvbggukv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3usiycyzy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wupetrzi.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qbsubene.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ebbsxbwm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pshifutw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xrlujpwi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3fnlqqsqj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dsgwwyei.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xznjvgeq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qtfzagbw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3neocikyh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gzepdguf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hvmbdzif.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3parntjqu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3upziczvn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ckedpefj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3btsporqq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3atlrchjg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ftnpwjvr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wkhxpciy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bavykwho.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3siveaora.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulplqazh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3tbnicmmq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3yezvlquy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3nudmnzlj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3swhrxsps.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ocrvbypl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fqgatbmx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ggimgela.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bgktjuon.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjphlrhg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ofdlhkhh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3glyguqwg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cejxifgf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmktlwth.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3irvcjcfk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qwyepjgo.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3uubzowzt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rqvriadx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kouskxbr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fxwdchlx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mxapuvgs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qtaiihpj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cblvuwwj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gonjfmvg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pmlggtyy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3tgpmsdtd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bvqxycyz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cgahrmaj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dzgfnsxl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jlnzhkdg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3plqhivem.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xlhhzkoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcxagyif.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qhfeorfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlfvwwss.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3etokfyvc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fuyvwvbr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxrjhnqn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zzgzutci.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rwjyqqni.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zocyvwak.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3itavfpme.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3lmqlxtwt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xltltrhi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ooenpvln.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ohwfumcl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kxagkecl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yjsiudyx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuhwsetv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3fbbyrnec.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fuvkprew.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hekadyjp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3yxsoqsdd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nvgdvbjt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zvahktsg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rqlhokaf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3npgaxawo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rllkfzpv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3tjypqetn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3pxjknokv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3flwxrjdr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lvwbuocm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3hvseydmy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hjykqjwe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qlhbarip.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hlfwudoj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gwsqtqpb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3apcsleev.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ejjzmzfv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hkzhpxwc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ycrsfkrr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qgkbdbzk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zsbdbkdv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3vxpjkkhn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3irdjtllp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dgzywyyc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3prutrqzf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ladeoosf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3fnjdwxsp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hpxdlpvi.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pplwuybk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3eunstfcm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jrbfvenl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zzcxgnse.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3evzbrcrs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lfwffjtk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3czwnpvjm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jfmbgwiy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3raklfzhh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3irvcichs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3lhzqceap.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rsfrukuf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3gueqizqp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3jgqmschw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3rkjeylnk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qeleerka.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3tqmwzccq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3xropervy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tpvzpacv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3tmhbnllr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hipjigxn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsczwdsu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ucjgcmbw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ndrjcpju.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3kwtudmeb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3arpdmier.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3azcwrpfw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3bzaqdrea.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3niayexpp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzlvlgqt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ehfoicms.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3skyotjhy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vgxlqngj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3nchidrvg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wnyjfwkt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3wbttfeub.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mcqqisjs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qrrcekwt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3brqrdatj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ucjrqgmk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3skzwjkra.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gtajdzst.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3upgpugiq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3pkpgwqsg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rfhinosk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3hvuoqyos.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3zoxaisoq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3obardpvl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3exqafgry.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3pboobvtx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3dqwicnta.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xchubfni.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qvmmdjol.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3uoxgnwpv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vctobize.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3smuvnwjk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3migtbnwg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bvrwccyj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3alcothmw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qhbemjkp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3yfpgjgjo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zkslxxfs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3roalkzhj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3gkagqzkz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jxoxxxpw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yisdymuv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3eqgyxlyc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfpzgbyh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3crnplgvl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3eqzvmvsn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3gdnhvgoz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3zwqptnsz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3flhewktk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jisdzkeu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mwouylbl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yoesddqt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3lpyfmbzm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgyprqeh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dopeicat.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yhyrctnm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3riblwkih.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jjpsqgoh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wlmvpkri.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ximnapjb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqadlydk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3falprlgx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3erzlrpne.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3evdnjruk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3batnbvgs.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3etondgod.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3dhraqevo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yeymargf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3aisvayrp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3sdkyyzqf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bhknbrvx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3qynbubhy.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kgefgzbf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ycbzzegg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlqhecdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tggiquee.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3gsxblqdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mylqqsyh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tjxklglp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3amkhyvws.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3munnpsfc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ovwurhrv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ointoljw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3pknuaijn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3eebnmdus.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3buvuchbl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3lzdnaijb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3urqfmvpw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3fdzfdgag.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qokwuzvc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lwafodgg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hwgjxtrf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nmqazrce.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ihvajojh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3pmrskhoc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3usjerkqf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fgziwaev.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gshtwnyl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3fvtkzjlz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3koghysra.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3htriyywf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3snaadctf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jujbqcum.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3elrkfjxz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pnxbatdg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zgjpwrql.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3mvomzuzs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kmunumfi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3laobyizf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3eqajtsry.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zdoperye.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zdvwnxuq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wwlzxgjz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gcktozaq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3fdakxtyg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wlxyygxp.html


<!-- 参考信息 -->