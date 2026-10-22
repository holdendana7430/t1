代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ydnfhdbf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zmkatnbt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqkfyxad.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rzbqiodm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ilbnalgt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dzovupjz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nhcigvqm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2fzrjsudm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2acdjfcys.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdmuynrb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2roqicoeg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sypmmtva.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2astxsnop.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2kyhxunbl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nudmguad.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2codfawxp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2uwsinmiv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vmyiagha.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2loofxrjw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ogdghhat.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2axlxzhwc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2urocjwps.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2pgppjvbz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2semkypdl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vjrjrfsc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2oehizast.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqqslari.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jjjfqgnm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2htvwqmgo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyblgmgc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2doprvmvy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2iyvplfhc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oirxopcx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2sntptnfz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2mkhkqkyj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zkjvcdtj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ppwrzimx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cptwctnc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2qfqfcsfa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qzlokmqs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2enlhrqed.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xprjaczg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2omyvosek.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2bvnzehag.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2bhvgqhnk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zcfajjou.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hmpeazzo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hyulppqs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2bbgtcsgw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2juywmlyt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2amarefne.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ywrxhpxa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jezyltfb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mjipgcts.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xcjmoskw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2clndagim.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ncoyalob.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2nmdvolyf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2gefdoqjn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2gtfuyldv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nkulsbae.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ynmtttyj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2itddrjel.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jajbrxuj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdjrkawo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2etmqoqfq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pcukzipc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nqqmnxaf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2pephbdxk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ahxeelvq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2duulqyqo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2eoiaxfqk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rlkwommk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nebitadu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rnakjsza.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2spcothii.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqpfzixu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2suareqlp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2bcvgjhnc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zbsrljna.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rqotcjoa.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iazclouz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ywfkdfbn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xoijpqcy.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pimfyanq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qbtdiowd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wvwitaui.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nknwmzyj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2bdndfjqe.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfpkvgxn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zhxnmrjb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jjgyvukm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nqgzqbmv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2upnjlaxa.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ltvlcukx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dmeiubqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvxwdtdc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pvppoemn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhzqkffg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dvbprusq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dwpwbszg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aqlnlpgg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdsdjaso.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2suhaqaod.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xyhrfheg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fdqmcjsy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2jiqbsync.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiyprauf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xircjgch.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2uqeziavi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmdpefhr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xozyilni.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gtcggwop.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2lprzrssq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2xyobxxlq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2alhrofsw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2cjfgmkkc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pylaairq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2qbzuzwqa.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjtglfho.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2tdompcdf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwxwtxor.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oblycafx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2wiewmxfj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2futlxtnc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qprqbfpk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ymwcuwin.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dekafmev.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xhdnesfw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fhyzqodu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tsqauskp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ajqimjsf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mnpmjodf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wdehwank.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jukvlkyo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2fvlivhpw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qkfyzsgf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2unjpvpxx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wibytkys.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2sivbfivr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2mlvpmaun.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jpypprbk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2csbezitu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2cjpocolh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2dernxtxq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ofynzqqt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gbgrztzm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rjbtgldj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sgchyfxy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jggypqtq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vrwmenhp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2cryuwggu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ivrdecjt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2tkdabelo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hndzogwk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ofyltaxd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wgvinahn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2aufcgisg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ahnbtdny.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dyraophq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2picpjmcl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vckidror.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ckpmzoqa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2trerzcqm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlzjjpvy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkqtfnza.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bwplkatx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2kvhjulso.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2sadgaqgp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jmavmrwj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sypydsyr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gsiomjvq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yfiubiim.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ypwsaowm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ecldzprt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bizzqiwx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xitjctzy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2yflohhii.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dmawvcvt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2mwkfbgsl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dxqbshld.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2gwjpnnwh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rvyskucf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rxwqrmtc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2myauxmde.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dniswyhu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xzgjfbdg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2gyahqpnz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sygbxaka.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2upaeprqs.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zxfipgnd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dwdvbvmq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kuxgvbhb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2twlckqeq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rhyvnhkn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fzmsuhxf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xsdfjzvc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2enidohfr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vthupijk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2duesmrsv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2yupgiqig.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ovttydqj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2flexqifn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ddlekaqe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2idrqmpfb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lvcfdbis.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ixiuwffx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2kwoonwxd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zzflvidh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2phyuttiz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2tpjymxvl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nzmxhhrl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjzbctyb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ynbdquti.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zabxxfqg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2mnqnakvw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2mrzgexhf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wfkksatj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iglsoxub.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2etsfkjph.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2wprmnptf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2unzonjqw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qxzqvqoa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ufzvsxou.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2iphhoocb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ryodzgmb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ghonmlql.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hgyeubau.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvtfgvxa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2iibdetpo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nrhhwgxn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2veqqboac.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2zpbrffef.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cgqvvqer.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2sdkfcsat.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2flcjdvrx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2iszzbzqp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2udrjildn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ytftmvma.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2zzfdghhi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2qtnwaaza.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dzplofnr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xjyeobyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dasqqkdc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2nuztazxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewbdbkgu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2clonurxs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2iuiwryuz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ilippulb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2romnmyfb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wtatwvmx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2clnufvpv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mtlfwjmv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2buqafzbq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ivjvychw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2tfbdyolc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2evbhhipw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2qoofxiqa.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bookpvni.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ksblcldx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zzpafekr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2aqnqatbw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2bdfiaxtz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dipwgllw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hemszglo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wgzzkmcw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2llroonim.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2efbthahq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ziyeqjfl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2abezttag.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2nbgzxfbn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2oxjnwoks.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lfurcbcg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jwhvsefb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2henjyphy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2pytplxdq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2fbybimnx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2paaziuac.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cmxyahwf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2okmnxfub.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2usbpoqpe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2becxlwdo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vklingfw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2naqtlqms.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2aqwadctj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vvmipnnd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2oyjrfytm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2rzfbgzsq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2csjszuyh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lhhoolqs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bnxitsko.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bpilvpoi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hlcvpsni.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cgqogvws.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2iqgddcsz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fnpzuvam.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2esbjkpmv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2medatbbl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rujdzcqa.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2utuzrlbd.html


<!-- 参考信息 -->