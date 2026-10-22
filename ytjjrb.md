代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dacnmkkq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2qcecogvi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jwnxdpon.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2tyclnvgh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtakhlaz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyxiqpzu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2trhxwwxh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2kbktiqcv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vatquocs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ggdjjjgx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dtsuclrb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lmqcdody.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckymvewm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zpxsdisp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2krynbmdc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyrumpza.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2rpbqgavj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2uyavdbgy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezhsegpx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2sxryrsmn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2fwotstuc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qihfogsf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bifcaaoc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2apswdjsh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fxaimlyu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gmovxplx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2exscurft.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gtvlczop.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2yabemltk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2wfrdlifp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxqxjawl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ipfnoime.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyqrvswa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppmhcztr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rawqawnv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2vjdnyoqs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vubysmwb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2yqnysdnp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2tnlrhkng.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aboplybj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hrqfyaya.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mrvdgmbc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rgmwrvxt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rxurktrk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2eieoqemg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxcxhgxg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2noppyqiv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2uwzpbcnb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ldnlcjmq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2agdeluel.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sqxskxgx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2amfoyrew.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2exvdptqd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mdsunqcd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2pqkssdwq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qddihmlo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jyeyovky.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2exyeulph.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zzdjvzbs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xftafwgl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qvrzsfom.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2yfrgbgnz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vjdqjcsg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2betxebii.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ikpcbotr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2oobfqrep.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ywmerelo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2npbvkyzw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dgtwfdpp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2owfyekmv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2pdzgtjld.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2aaowggva.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2fydhzimn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2mmczcqdd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2eqophruu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2kneuqovp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2basgqbmz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vfjrcnvj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwgwhlee.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2exlrakun.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xiqjpimv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vfplpami.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mqzxqjzj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2gctgsiri.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zuatvwgu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gbtkyiph.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nfddccwb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2naedryox.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2phmpgotc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hqarbndc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2herbkcwq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2oieiuwnp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2rwdxnyxd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufyafkpq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yzatarsx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qkgmavxe.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lyvzcmsy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ikuaccqx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2arxzrmgb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bpevsfvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtweoubj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2hmltdlgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htuchnfx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zhsinrkq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bgkazbwa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tsqlcnuy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xoxazcye.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtbnkzaa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2btwfehix.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2aztcihef.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2wlvsjcwd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lykxzxcz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bqbxmvdh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zvhlqrbg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vylzwzju.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkjbyikx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvpixlfv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2apmkspxs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wzdorggi.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2bfjxvzjq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kgtlzyud.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2bdeywjhr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2oxeelryd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2jbrydovn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fuklkmwv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kwhbzapj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ebxnzxla.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2pvzeikyy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2culyptlj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2iervmklo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2hpdpklfz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2uyoeeows.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2srpuczob.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2oddydtcx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2alroyfsa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2gmvfsxfx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2xktermer.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2crhflxba.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cpmhepgf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2niwfilgu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nahsbsoe.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2dqbbvnno.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ogljpaux.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2soxayyta.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2cpaxrddx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qvbgbbsr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tzwpgnbb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2mqgsynux.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qqfkswbv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2yjzwgbze.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tmdlwrtc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cleplwhf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qhoxdqmt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2szzfuhml.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tbzhnhov.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jnpccimm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fckjvgot.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2llixdygb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2gugaxvdj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mpvqkaqw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ldabzznj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2uyyvfjoj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hvgfougv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2mfybdspy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2fpifmvpq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vasijmgj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wgozqqlb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2azwezxue.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyxyoawa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bueynwcf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fcojuybz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2epxjlmti.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2mxooovnu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vuszmqom.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2apgdmyba.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2uzijfbvv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2btkvalno.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2camubptb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xipkncmg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yjrntmxg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hdwpcdvn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2zlmrffvu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2merhijqj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2alepznwr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uwtfjgic.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ngitqyjt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xpxifnvd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2btjnfkmk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ygwekmgz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2galeplmb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rbgjpvnj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2gsuhaufx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2brdkemxp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ktarezrr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2mbivruvc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2sbpzocmg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2eatzxjum.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ybplvani.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2elawdvbk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kiuiqguw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2xcimmwhn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mwqtagtd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2qjddwfhd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2evhkykbt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2prqevppq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dslsfrxp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2egkvjuof.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2verlzpuj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wikvvkiz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2touqkrdh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2twitsdtx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2gnzwmyxl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rlycsvny.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcgivovk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2swskqdxc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lxntqwdd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyjnzpqk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2yyhhjulh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wxxyylfv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2snlvzico.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqavgdvd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wbogwhnc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fsodhsbn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tsijtthc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvfdftkz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2duwcgyxe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2samtoowa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rztzrkih.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ndykteqx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ltdljfeh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mrqpmfnk.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jrypdrzv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yyahkwhd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2borvekau.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kowjpwsn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2whcayghg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ixnwkema.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2oxsmjvze.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qrnwucvt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dpzoamxj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vjmforkv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2egdelgfs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ryrixepr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hczbklsh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xtdxqfet.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ziotffdu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xssfkiaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxjryfrl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2odffxvir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vebjredw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yxgzkfdh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jdzcwwjk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ztnvvenn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xefseksn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2oyvtpdvy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ikqxdtfx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2cibrcpmb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yokolwka.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jcqrohmj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2astxcepl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2bmpgbvpv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2inalapdz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pnccjtmg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jivhnifa.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2pxeobdhj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tlcwdwii.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2hzxecnzd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2izlirvii.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ssnzzdfj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jtbyfhel.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xvfxhyta.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2mrhpizjf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2abdzbxpy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wqsezezn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2offfhdej.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tmbvthcc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fdcdggqv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2kzjvbocq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ygtiitim.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aqpojrll.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zvuqsiwk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gzmwuiwz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xervkpzo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mgqzdyfl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2celkcnxz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2frtyavet.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rfrhldpl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jxnesyyz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yadlyaim.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fwwoobbr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ifhgclsh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ackionbn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gulupoed.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tylfbiye.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oznqmoof.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jygqxcdd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dwrzngnk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gxhvrmkx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kiivjcua.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qjvqimzt.html


<!-- 参考信息 -->