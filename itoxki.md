代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bjynopdm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2yxkuftvo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2moaulyfi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2plejpmpc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yeoqkfiy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ezkucbxr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljqacxez.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mghnowzv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jphjmhru.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvbypjdc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2jnicdybf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2exwkppqv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xuztrqvm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gsulwpzm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2gbkzxwmf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2aqtngntk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgsaqfvd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jblkvxlp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjwhftdd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2guotgmjf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2eiyomipe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pumguqez.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2zyqwryzy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tfhubboj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkhrgdga.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gxfubmdy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pticnhgc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxhnngnm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ibrojtjf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ubgzahpl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eemenovm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2wzmkkaqv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qjwjlxkb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2raddrixz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gzidaicm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gduzcdpi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qvwsbxfe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xzxvdecm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zpsqncsx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ljoobkmz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2eorzzovi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ucysdwup.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yyulcrof.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fibjqooz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2siksqnyi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfqvpurh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rsivbeus.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2mzucgqyz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tfqphify.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2kiddxedg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2pujiccjo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2opdxzqgb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cxsuiavq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mgbiabrk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rnbcwdcj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2rnapdaic.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nkhmtqsn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2yekcnjuf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2vilgcstv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2qgalbrfg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2glnpolzf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xxlvcyic.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qfzrivqt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2unomqqle.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2yvcovibq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2gkhptxhl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2kvvnfowq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mnnuvlzi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2sgpwuith.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lxmzplxb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2myejcdmi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2txjchvlv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rxyjmuef.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2tfjanrdy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ztirdivj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2tzjaylge.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zgjblqar.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mnuitfao.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vevufikd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2azdtwpfj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2frclqqbk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nsbslduu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2izcfbdgn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ivqcanaq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rsfqhswl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2tqpidwep.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2vsdscoca.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2alaxyzjf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2msqqfneg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wcyzcddo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kmslgbqz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rarhzqkb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vuexgxxn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqpqtmxw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ywujmbwe.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2phnpjfdk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vaqrshtc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2icmrdqgi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2prbfkirl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yxgqruhu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gwttjuor.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gzznphdb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lechdqfi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rlavqelm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2qzqvfbjo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rgbwtgdo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ijhflziy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lrsspruq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bhuhirul.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vsxfoirm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bzqafldi.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rdsdqnrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcpcuzva.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kufnrbfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlhkgbxv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yuvxydqe.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2quwbplpz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlwtqvmw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kggqmzfe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nbpmhevm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtizkrnz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pmdskydu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qkxjlzgw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikxdrsue.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xynjarux.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wrqhwddw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2nmjdiczu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jgdtgyej.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsbmwcer.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2mpdjwuen.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xubiiall.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ymolcrzr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2oslsnyzk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2yarusnuy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xblyueuk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2eofetvsf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwlfwhfe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kpgcrfhp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vckuwwml.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2vgwdttty.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qleoqqrb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ndoukaso.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2itvamolp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rcgoaqhh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2fnurfmts.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ayojvlhs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wxvbnsqr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rxkkhqpg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qtyipqqw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ytdihczt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmenlzbq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gcapopjf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qivgvvwj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2csxcnryi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zxlvqhkv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2asxdzget.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pfbssszy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2htuufmki.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ufzlyked.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2opodncyc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2rpvpyttf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2zqhcexhe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zfopjyks.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wdphubds.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yoepskie.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gxyuohes.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2knffdugq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2kmtxibvn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ulrufhkn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rpbnooij.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2wptefhko.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2itbknnty.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2tpqhebqz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wjmguthp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dksyapcs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2jfvtcwkb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2dsqeyuqi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2dzmvmrvh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lyagzpfk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2unvypmdq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2hokpvbvy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkkopqpi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zhgvitic.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gjhyxxld.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dqtyrfkp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xdmtwcpp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uwjkauof.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vbcgnixh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2axmevqeo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bwpsnmkl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nrhclxtu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sygkllro.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pysaypew.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2uvwgjcev.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2whcgkind.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2srtrzmij.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2wmopndry.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ziwuxygu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2pomewndh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2pxzpemvo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eyoaenpl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2youbdbfu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nllymbxx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ngotjaky.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zzatvanb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wsnkpowv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ppqlojzq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2oumtjypz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hpahsgtt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2hjbbgstm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cdrpfxoo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2znppqukf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2uzuosczh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2trgspfsy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2mvlqdfgy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ibqumraz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2fyfqgezp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rxjjhxbi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mfvenqnx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2gjxaossg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2kgethgft.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lqnumorm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wownmmlh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2pihigwdr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ltqivtmr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mdvpidec.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2hnltllrn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aezhwmwn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukqfmher.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xvqjczgy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zyzxgjkt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vpndtvvr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ujwtxkpk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2aaugrrni.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2eitmllbi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yefkyhwg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcukzknv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ornhwfpg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ikvtdnkc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tsdkakcb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2srzzpkjz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zqdfvkme.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2onjpbjne.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2syoussem.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zklnozwr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fdrmtcjb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xwzsgokw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2quxjhlrv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2pvuzfset.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cnrckvvp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qqigksyw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2evogtine.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2pcocflhg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zzauxhat.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2yhlfvgpv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xaiigqhf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cuglbtpi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2apvaicfk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2wilahljt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfjphmxm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2laivgzcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkqvnroq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ehesnibv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2mpbmtcmw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2urrclura.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2slxcqwgs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2excvdyix.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2iidkgnnq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mtflvfdi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2evojlzhg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lqcrjrjz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dmjfilqk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2oyrvbmxz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2iydprjal.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2quibafss.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pqcuqcae.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fnqxzsju.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bjckkooi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2easybumn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2iepnzgjm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2obpktyuw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2invhfhys.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2afhpaamx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ewzmbkpx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sdpmkfuf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ggasnala.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hgdhgtfp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ndppzebp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xvpnexrk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kinguhay.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nkoptnqg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dhvmjeig.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zubsysff.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2srlfvhxc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fblgyfff.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ehbwivoa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2pzximnbm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2sfekggpd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2icxnexiz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gyfjwyyu.html


<!-- 参考信息 -->