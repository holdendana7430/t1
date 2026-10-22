代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2gbiplbfx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jepmvjgg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rdadskhj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzuohigc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2csxdkxvf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2haoqkuaj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cafishqk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2emqyfalc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zpgtqthg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pqxawpoi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2brdtguba.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fnaomarh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zqbwwtks.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cnojlyym.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ihncfmdj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2onphdxmd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2cggctbsw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2oakwjgjr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uspaavkd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uypnnqwp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zewhxjed.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tiqcivjb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jpiybigl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2mlcfljey.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2namlsida.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2gthoanzi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2eagamsin.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2vshphysz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mpudnfnz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ltgizxkw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxxtoula.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ydipwams.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2aooflyce.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2nmkzexbd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2mkodywjx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2voqpkvzo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dcvrnorf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dgkazhmz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fawbhwgt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2tdkbfeld.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2qyxkzkpb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mnreeiba.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2chzclssv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2afchltcm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ezuwkcfi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ylbyfsxm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fufrfumj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tgboieve.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2finvngfm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ouqiiagj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2virxosmn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2qlukiqfv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ozhftqnt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2nmoqwxok.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2iakgynka.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2epnrlxci.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nekefozi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2njkrdcxd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2gvqkrcle.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bjleomnv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2wdqdfjli.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2bwxolnyg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2myhhlyje.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ndhbgqta.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vtxglimk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yerdcdoi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pilceook.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2tqsncdlo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2okxlazun.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xcpobakm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2pdfjfaur.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2fswyzwml.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ylmrtdog.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qohpiqol.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mnfcwxpe.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xeglggao.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zijvypgg.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uoxfgmcw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bobdhjer.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2zthqimul.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2luhdwmmn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsrzxute.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vpxkhgvf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ozhtxopp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pqcvlqiz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cnijlxyv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2yvnsmeri.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xuhffzbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhkpoeoh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gyxdczwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnfxtcqq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2velubzxj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nthweqjl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pktapwas.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzrheiqb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gmpgvlqr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnvmydwn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mgyjthyh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2awfxmnqd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qdexqjlz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gcidtbbx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2kxumxgtp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjgctqxg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2utorzvdr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2glqdrbpg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2mbprzicg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2apdnagmy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xyaltnco.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fuyiatff.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xvywiwui.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mfimfofi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrxuwuuo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ohxomabr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yfsnytdy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2sfmlmnhq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2gmcqnvdw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ccunttfg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2kxvopeui.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2epzrnomx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2zvohnloj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wwpzvhmb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jwtuszmk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gdaibfjm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jtayfeim.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2rloaeelb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2itbjfmxk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdajgel.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ffsotsrf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tdqbshht.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2qtykukju.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vumzzdec.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wmykkmoc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2lfkxomil.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mxjvagpz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2crygfroq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2uvbnirtp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2rugemeyx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2fycsdjjn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2fpsohejp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2euqaqwdf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tripfzpf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2brxryflh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2htwbrrff.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2oxxwzmjy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pyfrqapz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2serxpdds.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xezrfmkl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2amvpuroa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2hagkyhbh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ykeyhnnj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2zegpvmrc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bqlobvvo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tpcvmayi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ysrbmpni.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ekjqyhnz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2epoeziot.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2jllmqsiv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ydwdlxlw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kbtxpxip.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2tilkqztl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2khgupmcn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mkdzfrjs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pqqfvxzy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qvvxxhtb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqmpyqgb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qfoxwyzk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cscveazc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2onizshxl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytifdvjh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lrllnwtd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2idsdsnmi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2eitdfdhx.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2slczkcjc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2duwwdqcl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2geftzumr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2jpowmzuw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2axlzmvbb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2njgltdno.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nvcahhhs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2jmwoavon.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vfnhkccw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2rqsohpza.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2whcawuga.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wsxmirws.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2oshvtods.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ojxxsbbg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2fvjiooyh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2aiwcxbzc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ngsrflrg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2nzdewigi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2cwbckrcu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2baetdqyu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2pxnrkpvq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zjdcjwhc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rzurciom.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2huxatfmh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ecgarxlb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2dabbiwph.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2kbmlupfr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jlntquxg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ixrkemcn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuuouizg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2oysetrar.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2crcxtxcc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2itpgenwk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2pjygzqiz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2qmmomgxs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2atkbsbte.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2covugjzn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2galdoiks.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fysnrgsu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jdzcztog.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ofjpyeoe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgtndldw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ciswmtxt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zgaqrcdj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2xvwaotst.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2eerknytf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2cjhbmuwg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qdulcylx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmyabdxp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpvylhpd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zkqhyovd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nccoqjji.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2radtkhwc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2grdvcizt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2qprqdlqy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wlywbtcn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ayoevrif.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2xwfgbpza.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jrbeyvvj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2inagbgvk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kfmpqvhp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2plnjkxgn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qlddihlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mphawrki.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zolpxfbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2getyxzkt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wfzhoaol.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zptiskwd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ecfpxfwm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2msoewerb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2humdpcil.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2fogilcaq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2uwwvlspo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ngvvrnyn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2fxnsjgvz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2fjkpkhtm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2idwsximn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hqytdcpo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ebpscylb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wrtzfnhp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2noauzzkj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2xupvjapa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ifbwgtvy.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2izkwjpqw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2vqyrypai.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gotlskbk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2awphndlb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2orbbioun.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hsnfspnj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jjahzjaa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wuzerrwq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ehbancog.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fyckleny.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kkctfdsm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2oeqbaxuz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xuvtgoco.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bdcxfbih.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hejfptrg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hnemttkq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ohsxnstl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2chpqxuru.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lrsowpkb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wbtpixbt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2farchhdn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mbbxtdxw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jlzgvykg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2mlrqmliz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qhqegjoy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xbvgsnkr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jtlpioxi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dbwozope.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cpqsuezl.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kotdzaci.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ysrrufxr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kpspamxe.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zdkybloy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2emwrnxat.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hvqkmjfq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2frutdecr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jumigtvb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2yhmhxlxw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hwnyvvnm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kvttultu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2atjoxuyb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yobrvvrw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xmnhydqi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2oumpmytc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2wfyglkvq.html


<!-- 参考信息 -->