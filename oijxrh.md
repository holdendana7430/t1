代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rzlrzwco.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jmayqkwr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wjskxoty.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2zdljwcke.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymwmqnkb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwfikodx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzgxahdb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2oupdzbwm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2vqfugqpn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2froogebd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2zwkgfbkz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2nwdyrcpe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fipeujvw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcsvmwzd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ccvhlagl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ezelzdji.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jcmumzak.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2tpdyebbh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dzziyivj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2xkihtldo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2aetgxhpf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rklmcexq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wozxvwxq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lsmldiem.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xddrorxq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dbxaeyfx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2hijlaflx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yquduted.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ymsiakgb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2rkfrdijg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lmlsatjy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2akrbghtx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gegywqiv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ergudwsg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bfrrgwio.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ngyfqvml.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ryofpnlq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2wpirlqnj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vncoqxbe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezomshjh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yngycxiw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vaiqibrg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mlfldirz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2glkurywt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2litkcbxd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xmkbwpzs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2qprxmolz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2fkraxiyu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2nnwtfjsw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wkmyfqqi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sibylozc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lgaisvrk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ffwykhdr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2fmynoogi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aqrytpzr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vqlghicg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2djptzyfi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zsaymlea.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oiqayhbn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2oawsuaip.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iiximvjm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2yldpfrlf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2msvaxunb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2adiaegmg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2cgpfwdva.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xbqvrxnd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2euvtlaos.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cvsgbbhe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2buqwbyxw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2yfvqqmag.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wcksglqz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2zuwrwylj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2cygxcffb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tncbnunt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2oiwktpni.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2fwoqaaff.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxsozpsu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tcsbpaok.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2acbovfee.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2iacgbqqw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2efiotwve.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ebkzqvod.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2kugnogsk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ihzothsh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ezlhzteo.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bhosuxhb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2umowjvgy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uwpwqudx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2swtibsnl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bxaaaeen.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xnjmpihg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lymhgwuy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zedpqvao.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqmsythk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yngqghpw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jlbpfbqh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wqsarpkx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wpiwkoim.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qitlepau.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2eywvmgaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqxdfgpn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wexzyqyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxbwjkfp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wtnqgvtj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mwdexcmk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jofjmqpa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xctpyxqn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2axaebxua.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2reslnrwm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jolrpanl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2idlnoixh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwdgfhni.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hzdxuzxy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2gucqjjqm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwhalxah.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjzmoswu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbhmxjir.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2cpejopyh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2laudeuvn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2gzxnwxfr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2tvetvitm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wflcqlcg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2wzsyfubk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2knpcpncu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2canjrdrl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jarcpwwi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2docpnujq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2diktglfm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xtcsfrno.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2irhachym.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mogkwmyi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2csccyqjk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jwopfvbg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fupbubjh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ahacxuer.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qrsoevyy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2zuklyssf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bpryyouy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvsbwivy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jtkwdgba.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ikjknzde.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2saemvtud.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fslfxgro.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qouirxwf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2rxbpapbp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ihpftpgo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nekgnfdt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2dkxshwgp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ewgqehvx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2umeeotyb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2vlokkeae.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hfiimziu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zdpetnag.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wmanxesm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2pbsqigyz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2gwpkyprg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ulmdjxng.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ywfxptyj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hwnlizes.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ftghyhjg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2uzqovlak.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2xjmrxyvm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2qolgkmoq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xfimzasb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ljtwgkeg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qfqiniyc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qzerjjyc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2tgdkfugn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdruptmo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tjqzetgl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vuipulqx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ypqjjtjo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2rysceavo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rwbumdkp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqdlqqyl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2dtutwbro.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqvujqhg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iusijksc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tcfsrsue.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2shptjint.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zctzgdop.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2dqzvydfp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wydfffbp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2fugcuqaq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vxyqdcna.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ftfhjkrv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ypteymwd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xhveewzh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2egieyubq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yegovbhm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2clajmtsu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2mldotuxp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xahjorus.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2rxfwopmz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ugvinkxs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ghkcawho.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qpebkngu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vhknwxdp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wdweyjgs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2aurhuxse.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qjrotton.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vaevymhz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2tixmadvo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2frjhvgix.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mhfwwwlq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rmmblalw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xelmestr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2gfncsdlz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zimwluzb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rhxqxuhg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zsbawaxe.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2gsdckjgz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2nrgcuown.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qukgmmgn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bzrxtgis.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zcyvjwfe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dqhlmupq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2veigzcia.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2yqndlkfc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2euxusyam.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvrpgudi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2zkvwohxv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nyrjzyfk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pywbdglm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2odviollv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2recxcplw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2trldyifx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vpjgxwco.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2cffkifqc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2iqdjxooa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mrqunnnk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2coegfyjx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2paydlhlm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2agzwsnhe.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2whcktwib.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dbreymwh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rcvvvnwh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tqrduxfn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2fjtazsuh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2naqeuwkm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2izqxtofm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2etdaibys.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wavhrjlp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2asbgugxj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2seyyfpnp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vyzesdmq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2uazcqtga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmpnswfr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2fhhexgew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2karuhrhc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rjypbboh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2dpfohfwm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jpvkzdoz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jabcxdik.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vgpuupyr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2zueeygsi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2lgodprdh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2uhdgzigg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ycnntjzx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2efkebsvt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2iellmcvn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xemsklfi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2myficusr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wrpvjikj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2mqskhfgl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2qbaccfdm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2mckrieiy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rcxigczr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2tcjjwvjs.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ylgvdldo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2gejnlxhp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wbhfotif.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qzpzpwuu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2iglmljlr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mrycgkhw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2upwqehbv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pqromale.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2klnmidpg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ygrrxqbm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmcqvdwx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2wirtsjmc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ditkyffn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2rtqitpgd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wsilwpzj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vmidxxqv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zogbakrp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dpajyrlc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2npdvrlqi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dgeaujdb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2argfitmg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xvasosao.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2cgnwwcvt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fmizlent.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xflbbfiu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jeuxigem.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2isoigzjr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zbqcivcn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2htsqjchk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tnwtiegx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gtkbmnxn.html


<!-- 参考信息 -->