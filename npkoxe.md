代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qmtzljoa.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2fnnrempv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gbovkiys.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qvbwgnpe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2jnuwkyoy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2dzepjjhl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hwmzgnvu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvwvhqgx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyopmbuy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2njikcjzj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2laaaidsh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2cktrcsfk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xvkjnhpg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xwgmuthi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2amcuwplt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qkekriqs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2watrdgej.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mebfxmgx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvbkttha.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hvocojti.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ltvqaalv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2waepuaey.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hvvlyoio.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2gwtebxyz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2daulqyuh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eorlnnwq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ktcoolob.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2olsxvdpc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2knjdlrev.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qpmqpkcg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qiqyjpoq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bmukuwtr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mswiixto.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2voklwozl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mevxmzpn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jqfbrxcd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtoaajxc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2taaeabel.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2raakegqw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2naokjehl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2clrnpytt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ufeusjmz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ynzkyaxu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtnzpayx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ooevddny.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wbackrfh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rhehfnur.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lsogchbe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fuzrxozp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2lhccbidb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2oocuhxjz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jzaomiqr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jogknfsl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xjhtntgd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2slbxtjhb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2cypormzx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2guvkomrw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2gjvqlugq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ocsnocot.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2balgvutf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2khsievrx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2oyrlqafv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bzkjhnkc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lqthhuzl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wzhvpogr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2jvpgxjle.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lmwkhnev.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kryjcydc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2loapjufs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2olcujbhg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2usdjepxj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtunwldc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uvlracfw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2xdkukqwu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ohurtlsw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2dfhrzqos.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gwqnmirp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qoxdqawn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2stpascnu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ettiujnm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aaornhdp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzteiwsm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hpmhzxte.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wmxfesgz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zedhvdlc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bvocgbqc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2voatnodl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ydvehszd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fdwrebbm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nqoydlke.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2roxmikcj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kusgrxwo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zoxrrzmv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bzqjrvvu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2onkmzpal.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jqachuhq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2usvskelp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2gqmdhalt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gihonrxr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cbcqexxi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vvfrjfvt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rmsialad.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2pwhuyqtg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jwrepdix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spvkozdm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jtzzjnop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etytvaqi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fvygcvjf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qysrqavw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyxpenmj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2icdsjziz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cejwszsz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2orzktvgw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2cgudqjeq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2oocogjro.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xrjtpfqi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gmvigszm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ecrbtopw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivvxsohx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iljyuhov.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otgbsgoy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2azjdkooe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dnblqhzn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2dfdodanq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2tjdzkoau.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2mltxysik.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2gtsfkiqi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozdiutup.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2djsvftyc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ngiccyjk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryjybmqt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2rewquwyy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2pumcfzhz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2hcneveiz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bshwrgyp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2djicbsmj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ollmofmb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvnvtwud.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2esgupdcs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jtgemhid.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2pavqprdb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cysunmkk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ieajdtve.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2rlrtrogy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lzkgmzte.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2qtmaffew.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zxttokiz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ngnavwas.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2xqxrxlex.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pkhsubyt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kwuelonh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2sqrbehac.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xbuhuzoq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2mtnvypha.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2pzhfwjem.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sphtcpog.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jpmduetc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oigkjghy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pvknijqu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xmmskqok.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2affahweb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2mwdzfrhh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2hsgxgdgk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2psuavryj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2aiqwhjzg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zzgjplel.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qloaktbg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vwliqbrq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tlmcucpz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2axcznbrb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fjnqhksx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zgaijzkr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2kxvxaocl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgdxmzog.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hllknckh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2xojmjlkh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2nmuebfor.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2zbjhxofe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ukzwmomk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kcpfmkod.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjarelbp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdlnzmzr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rzdwammk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2idslkmvi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqukujgf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xqmictal.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2caszdiva.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yiwqyirx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oeurmyfv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2adxtfzyb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2meuvwjcm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tawoifjh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fxjxhyjc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lpnltsrj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qqsbjtbb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wulhkbim.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vnmdxayd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ondgszip.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2lemorokf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2pqknneps.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zhkundhq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2plvdzqvt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2qvcpkjfl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lexcbtog.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ysejctqy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ghgkpuas.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ernfzrzw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2viwcjuox.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2muwdrouz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ejwwcpyy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2uxqlktut.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zqbcokbz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xjekxmap.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2frzxugkj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2bvpscyio.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2mdhyzkdm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ihqwynzw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzpjftlw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2prhdetdn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2exbmpsbh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bticlgem.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tpgcnoap.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2nszbbhhq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2btnymqou.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2oozspfwc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qszdbrwq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pkixdtjb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2osmvxkbs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sghzleyh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2skynoilq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2uoxnmlxr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2runpsxti.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2octdzsii.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ckmrcxdz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rwoddcpw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zzahgtrt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssoiznlv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2tlygkuwb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xbvylwwh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nnpgopvy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2omtxswwn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wukbulid.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2slininac.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cnhocyld.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2jmskxcxg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jxvbeyte.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ryngimlu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vulvbowx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ovzeyhdi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2loxlptbm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2falfjbsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asmihswl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kvprwvzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgyxxpmp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vkdmmfag.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2orfntqhy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wsmqcwdp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2iapcnlvj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2glnsqqyq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2pgghzair.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2krgzllbb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jyfelmzl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2uozhwrzl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bpzqsdnt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ahlnpxpk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mpskazsa.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yraftsoz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2olgngsrq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kelolqjv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ivhrkixh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2kullhdzt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hwdmsjdf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2aekdohab.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nsrxabla.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2kfrueizu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2nrtbtmtl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fpulcfdj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wzookydu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mnrixpgh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qrqmexbq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wmxwmuuq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2iqxikmxp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nrvbemwi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ejgatfvf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ilmnkfnv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kajnpqml.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hgkmctjj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2qqpchzof.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2lrtzhguw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2echvvhda.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2toooxlsr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fnhtnxsv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tpvtthdj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2khenfxdt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2rjboxpwj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2phvwypdk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ukgjwsgi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jywwowjg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2enyacfsq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dmzkbtrr.html


<!-- 参考信息 -->