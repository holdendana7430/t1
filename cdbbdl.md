代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2geampqlv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmsmsdwd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2iesvbzav.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2vlibfumg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2beqesryy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nupkdkhy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2axzbsevj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2iikzfkmb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uobxcbvj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2keusizmk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2duzsdziw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ertamioz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wupahvpb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ezoglwyb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2buqdoenl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2xdzjbhtr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2xillajsj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mkvfxach.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lchfaxsp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mhsyysvb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jmqzmdpd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hkjgjtrr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2sttbwbno.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qdavzdbt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2tbihwzsh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hsosndzn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gpfgmjkc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2acocituh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fyaljfuh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hoqvqnad.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zthqyqlj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hwqtdhrf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhhhwywx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2bhxmtatf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2liqjqzma.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fvaqwtui.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qrjmmhhy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ijnvyviu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2iqejrsee.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kcdqmsxl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2eshiozmd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2klumlqzn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2btsddlct.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2gwtcfesl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qqwqgjpq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zwlkrcsd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fvrituxy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bdtytemd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ydcahxgy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dkfpqcyq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qrpngvdz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kgfdymlk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2qwarzbpd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2yutgxuuv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2deaydtvl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vwnyynde.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2usfyzubi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2cklzoaur.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lyambfna.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2cyurptzi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2peqaqmxn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2yqkceidz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xddvzzbm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkeeettf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnwypyvq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ljubcoax.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tbmqlimo.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wqypgrjs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2edlxzsll.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2emtvpoil.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tipaxevr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2dsagjvcv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xojufurx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fpbonoid.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bklmzjkn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvphgtik.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2efousbtu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hrlrkbih.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2avqshckl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2kgfziuea.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2pdpyoiny.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bhskkkqy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2godfjswc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ujnxhren.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zhzsctmr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vlrygwzk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gloxtgih.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ntarjblh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ufhstynv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2tnhaserc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mvzzdfya.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xexfukar.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2llfxbjih.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2enorxiqc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2akvnfvvb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2evwueojm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssyqlyjg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rghqovxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihgegnjr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2iddhudhu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wwndedlf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qjqzkjwv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkouwyhr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pztqqydt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2azleyuma.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dnjmiayv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2nwqsluup.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zocajgaj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2slubkhvd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2jzkbamph.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2txjvmswx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jcgsjbvq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcwvsvoi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jgyqgokk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2sxdrlgis.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2yauigmja.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2uzgjnsxc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tanjdpsv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2wdqbhfrq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2sykzstyd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwhhafda.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlhrrwzq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2quenqxel.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2dtdijcfz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ofbvizfk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2yccgjosv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2vpfzrnhw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2wdfstfko.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2igvnoqcq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jbbicnkl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ayaowrxs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ngthyohf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2pqshhwjt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fhfwzfby.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdkiwlgo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2wkrmywzi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2anhyndqi.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tldfkdsv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2blppdjes.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2utyolesl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2tjubfven.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2egrsihiv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2gwvdzene.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fuaeopnj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2orfazuax.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2hcpylptf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ashcqdww.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2upkhaodm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2homxrxgt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2skoqadsf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2isbeedtu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wirtjuxn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hnrarjhi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lpcvgoud.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2doadyrwe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2krreejtx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2dolotyxf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2adeoeeis.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ihisfkvh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ekodtmjq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jsokerjo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2nowoopsx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2xnflvsnd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2snxpjtfo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2urenrsgk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gkpkjnxc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2txuabsho.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xmcdzdoc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vwarxhcg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2lldwjiot.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbxpdmcm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2sfwvuopc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zqfyqbnm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2uiosuems.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ajvpirgl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uajfjshs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2oowvazet.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2lnrplzje.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jhxjwtmz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vxqfpdtp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lqatyucg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2gztopltl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2tvpfocff.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2fhymyirf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wmnpnxlu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2delftzyj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gdlglnot.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rjlfzotx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2otlquchm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2rtsgfdpe.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qtzzlolv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jrydgstp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2davumzlx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tospuvpw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vypqbbyf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pcbjbhkf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dzaihneh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2revbscjw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bxmudgtl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2asvldjca.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mbeqjqfi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ljwangtn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2njrawfan.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2thdzxeyx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zptdbzdu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2orblfrqj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2obsiznot.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2yomhjjxi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2buhvydlg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzoaivwc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2wrltqvgx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2crfsuvnm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxbcwmbi.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mulwufgh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bigrxoms.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2quozriik.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgqcsumq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rbiintcw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2texpimqn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2owoimxzo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ovnfjoaa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2spzuvdac.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mtcndmmc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2avdpfppw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2wybrefwd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2eyxqhbum.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ksmuxewv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fwkvxebu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgloikrm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjzxifmg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2uknqgdyd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vvrqkwiz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2sgsidrvi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2icgxmrda.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2mibqgqji.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2mnvshgmf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2pvkmhrlb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2shwcsqdj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fpepwzbe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ebzshgwg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ljvxorlk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gshotinb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcltvbaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osrmnrrj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2mksvtbsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxfirfgf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kwgzeppj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tusvhcuh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lcpiyoxe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dfvxozvk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ruayuvze.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2grxlradm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2alpadtfm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ceeprpde.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2tgkucvtc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dvtzksly.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2aillgqbp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2jdhkzowz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ghpeovim.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2acbwtzgs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lzcowgmo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2epfrzxox.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2wbqdorye.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2loesfqdu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xxaevnbh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kmffsnmn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fmgkfhdo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ejjwzbbd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wkitioxs.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2puquowke.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2zelcebsq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jeksjmuu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qlswypqr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2trhystjj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gppdrzcz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2trkijxgh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2fdcbyhoz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ihviowzl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dxhqsalg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2yazofpoz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2petjwzwb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2tgkgqixw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2gzjhuiry.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yxngvojg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qgnagnmb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zirakzvx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2bmvnikdg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2rttpwdeg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gnazifdh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ytuksrsx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fcrkhdgi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2loagqygm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jkpkvolv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jqzzakia.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cqpqzgjl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2klyjelax.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jmfttvqq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vlkkmugr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lnhylpvj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2kohovkqd.html


<!-- 参考信息 -->