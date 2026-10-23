代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqehaiis.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3sofbteur.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3hmenwxxc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3shexlnkd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvypgmvf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnezvcxn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgsnptrc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3idbgpkdd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3hyzawvzk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3skzkepsc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zwdzsnph.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ylollyoe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3faoharwv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pkjvhmoi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3esqiyqhh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3taxnrcvr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3afrbzgke.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3evsudwqb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbohfied.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3tilfznwo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lnbtegcz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kubbsrch.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3iktvnzon.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3docuumvs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3llfxkvcs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yncctqqm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3reijqnkt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nsymarrg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ndaitogg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3fnzrlmlz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhxegryh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxqgdvhv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ukfdwhir.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aqgrdvgl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gavrmnem.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3nxhwyggd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpcbtyov.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3cycbskcs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3mrqpbfmv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3gaujybpn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3fgsaviph.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nimafsxd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3riwoelab.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3frbmgbnx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qdlzmvln.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3qhedaeyx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3rrpgcqef.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xelksmiy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rbxpsoid.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iherlurc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uqalpcro.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gutataoz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3xzssjkxz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3wzlktqkz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uqfvwaiw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bfghczlq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ypzdbjoz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3kyfwfcgh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ezxmujdm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mpsvvlgq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dbslwcfk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3syhbryue.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rtzzgwyq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3emqzkyqe.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3mgoeewjc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3zbmfezgw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3piihxija.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3amhzgola.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jdwhtrti.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wexibtep.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3myhjhned.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3fsaumnmb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3hzenboar.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3eyqaibmt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fekrfmwo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3caihkcmv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtaepypw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uoyoydst.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yibwwmda.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3izzcuxhb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cmejgqlo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3etufxyrb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3aqseqict.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3omdajpwc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kfzyfckd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cxvypebz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sbnhclpj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oxroyobi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ykoqgseh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3honcxdtc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eigicyfe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3wohpuhjp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ocyxhtaz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppbvwqis.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iknhmaxv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fjmctrut.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ezcxepac.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qiqhpenm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3lyvhhirl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3btbeigyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yozjanfk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ukgdlrhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlxreerl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vppgcwly.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3tqszlwlm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nrprbxng.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rduxrixe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpzyvoew.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zooivoip.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bqfxwvou.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3fyyzxica.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yunhnpkq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rzthrcpu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mrotiddy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3avagqrtq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fotupvim.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3teymagpl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3tcforidq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3nrguqjco.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3thqnncmv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ixlwequo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ikifiwpk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3cuwutzfo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3smpucycu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ovqrwyov.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsfjsdit.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nolhnvqy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3tejefroh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3doaucfzu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3aebojzhn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3kauzfdsf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3rsghchof.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3phjnmjwn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3thrhjggf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3yyukckow.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3itmrsvno.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3xujcpvrz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hvxgemhl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hlbvroqv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3uurdpmlr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yzvxqsav.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ctgzmzoj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vmmqrazs.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kjlxrbmt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nfrezudu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uebtkiag.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3hyvxbxnq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3mlddtstv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fgahzrqu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3uvbhzxkv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3pjgwnofp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rzndayut.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3thdykybm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rfttcmfl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3veudharc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wymbbenz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yitgzpns.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bomlmqeb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3lmyupdrt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rwmcrtgs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3kjwhyajk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gmhlqfxp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ulzxgaxx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3wmgqddyu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3wnoajirr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3twtltojw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qztvorih.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3kkleqirl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3zgahlcoy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qkihixfs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kysiuuai.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3chudthwb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lidtoudx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kocjibwm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cqzicskg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3uprsyljq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtnjwscs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrspdibg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3puplqfjf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zmbzxdzt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjrbrxzx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3rsbcrxog.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qzolecsb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ofbhvqvp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nzpqookf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ltylyatm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nggnrvnr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ivyegfxt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kzlajdrz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rlemxqdb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lxrowzgh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3tpcoyslm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cfcbawqi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3wkpkjioa.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3twtenpui.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3wohbnfbv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xidfzskk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3iphjwubd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3snoqztsd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mjoiylnl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3flikjdbj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3hwwcjrbm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3nvctcxxd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tijaxuxk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rhvmslzk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nfugjymx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vxgdqgtd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fjlfyfdi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xqnrdoyd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xkjaomnx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jxkifnwj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3bumamizf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3itvjzdeo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjbntwzg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qzjblczh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvtxsuac.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjkkzwge.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3qmegnxhe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ueyizsoc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nisazmek.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbseybwi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3fiudludn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ovihcvyw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xgcphkcw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3whptoaxa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmocewpk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3heoaherq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fcrkcctz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3okwobnft.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ykxptqat.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zzqykjov.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wmvmmjfx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkdtrcpo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3jeypvpjo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yjdrsyhn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vwjpfiic.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3yblyhyfg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hmlxeulw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3sqfrowae.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bltajgrq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3lwuyrldw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3rgfqshpg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ludqctrp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3xtlcyrbd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xuuqqrid.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3dqbblfdv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3bdrmpcld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crudvuxt.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3erjsarrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpzuwaty.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eplzgthw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3lfjirutq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vbigpuvt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fwbxywwf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qlzlrnkp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fkovvggl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jtqilkbg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3yvwzpurj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3fifrgjzb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3eufjjwvy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3whykvhyj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3eqxqrcgt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hmtxlbeh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xijumlsd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3hjfwhtll.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3njwkxjcx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3biikjipv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3adosbmwe.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3zrhqfqkj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3doghhqea.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dcjwltqu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ctpzrcdd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ixpsmuyc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3inmgjzmg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3fltphbqj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3focxfssa.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hsxoaxfs.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ccebcjbh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3izjxtgea.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ihmrwptx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3tmmuryqw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3edxdariu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rdeityux.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3aznoeuzl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zlpxpdbe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3nwpuborm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3gldyrtzg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gcsbknyd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kkmjyxxd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ctxmoncd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3hlcxdyiz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3aqzuypku.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bmpzupoq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3faewgqpd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3feanzdgw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bavzmkqh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vytmusmb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zzrntwzo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ejwyjoqq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uaejjmiz.html


<!-- 参考信息 -->