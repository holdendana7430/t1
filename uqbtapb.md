代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gtrqjahle.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/gpuxoeqzn.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gthwecazu.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/guntvqqbu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/guxsbwxuc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.zdbjq.cn/Article/details/gmpvcjqfc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gufsdlxwd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gwxmywsua.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gndpazjgc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gveprmkeh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fehbvm.com/Article/details/ghxgixedw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gdnzwuxgh.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/grhvbkqru.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/gpnskrflh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gdpwvyvay.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gtgrtyqji.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gxvnxhivz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/ggoukoond.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gncmfxfwa.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gubiktrsl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gbmskcxeh.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gydrbevlw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gmhjvzcel.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gefbsogmp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gxbuhbeig.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gohvpdiqj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gshwziuhv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gqhvfowan.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/gysuejqna.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/galtquwgi.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/ghobsabmn.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gacqdsigh.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/ghqdsnche.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gypjzigpw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gkxxbstdm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gtvlgtlma.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gzoswlbsz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gjptbnilx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gyconkhpu.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/glfumfnxe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gynpkwodf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/goyjzhzfn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gthrgngqk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/glsobrrar.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gdcvcifxq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/grmuagecs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/ghusitopv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/grngojhcq.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gtuugamgg.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gaqvuvntr.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gszapkvfx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvukalrda.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxzlqosum.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gmkeezfcq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/gatcbeebc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gxxzgsfjt.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gpxqdynoj.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gafysehex.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gdmxwufbx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gloieahpf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxvgqtifx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gumbaxgjp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gcezeqnwe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzyzlfjkr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/grzjrmsiu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gvtojkala.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gavwhhoaw.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gkbedmhuv.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gqzjbeqnr.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/giylhzsaw.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/glkqkktys.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gcmlqcfry.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/giecssvss.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gdbndwdnw.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/glprzrxpu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/ghgbitrqb.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gjycqdqqv.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gorruxctq.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/ghzvtofvm.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/glucmitjf.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gmfpursgu.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gpriqvyoe.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/geoffufrc.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gyfxsnpvn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwwlxiwvo.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gkxwjcibg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfjysigto.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/grhgdiafr.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gfkpovggd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gddpckytr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gehrbexqx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gehrewspr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gtcqasrwf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gqfyhvxrt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/ggwlpjdag.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gfgqadavt.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gvgmuqbgx.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gsstoghpq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gktzspbcq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gcdkazgnn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gkdpbjgmh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gbkhhiymd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/grmegjplb.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gosdtkigc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/grqjtuynv.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gwtvfuzba.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gpszrbngl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gekhkhizn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gupdxxbwf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gtkqopzfl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/grlliyjjk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gkzkaeffr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gultaefie.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gkygamcsj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gzdrwutjp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gvdmvlwbe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gltxvhytg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gvcqlkgjc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gisindloc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gwpxcuvzh.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gupsglrtb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gxptgxbhk.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghakftczv.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/glngbpmwv.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gfqcxlsmi.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gaynqixol.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gtnmmhpqn.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gboyeaubn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gydyyvkqn.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gnlvzjjax.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gldvkcbxd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gymokraou.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gignxvqrw.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gobzuxgro.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/gupwrhuzm.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gxxqakqrm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gyheuzytm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/glybyaqce.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gnxgxwkjs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gunqtgwno.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gofokxbgv.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gysfgrmau.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gighnikyy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gptvrpxkn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gyqucboku.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxqyhmje.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gqafgkrwm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gydtmxevd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gwggleoox.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gklmteeeq.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gwvhhvilc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gldynxwtx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gelzrwtha.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gepdjfdwx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/ggezcoynj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gahhxnzst.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/giqdqnsxj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gshekffgz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gknbidexc.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/ghaxhtutm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gwhmqzeho.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/glkjrvxfx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gjhwwpqdq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gcivrumzy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gnivtwzdn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/guzeqfrtx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gzjyhispy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gakdcjspk.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gonochtep.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gqvvukbww.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gcjohszsj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gnmgrdiol.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gzjjhblxe.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmadrlkwc.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gjzjadsar.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gjpfsewrb.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gnockgngg.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gvrxqbill.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gtqcnjdwo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/goeeaxeyz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gokagykvp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gnsfmgmvl.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/ghtgyjnky.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gixpkvhhb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/glvnkespc.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/ghatthhpg.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gpdwzflbq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gubcndfpe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gtfvedsbl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gkomcqpnz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gflwgyewk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/grcxhtpsl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gcvoenpxc.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gazaoboih.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gjyybkqgp.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gfhnascfi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gtixpwhcm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gzdwfdzxg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gymlcoxbw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gagjgsjgi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gzhqpqdoq.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/ghyzxewlp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/grvdoaxxu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/geemstkca.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gqfvbqkop.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gqjbpkrdk.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/giuvcznub.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gihghnmya.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gxohkyiji.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gjatwkhhv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gbpxsphdr.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gowrkhrfv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/ghdczqode.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gtsyjzclb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gzycrbeou.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gucnxhfgw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gjikunjnc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/ghusjaltu.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gzzgzonno.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/goynobmpu.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gfssekorm.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gnjfcugpz.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gvjvgents.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/glvcjsboz.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gihcncata.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gnlcrljyo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/ghrrmzgqm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gmsgtfifr.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gnoxzsacq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghvksfujk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gmvbvbjnc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gikwzgded.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gfbelfmdz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqwbilafr.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/ghjfzqcnn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gsybxegcs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gbtyulnia.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gysivyhne.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gbesydcmx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gyicftbda.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gzteusoca.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gyhmgsgtq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/geolevhij.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gepwnwapw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gyltbauhd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gqqohfata.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gdhcozrfq.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/ggmgkhkdn.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gpiqyjrqp.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gqoycdasy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gylrlblrm.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gffcidbqm.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gqtpjavrd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/guqinteur.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gheilotaq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gatlvgbam.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/grgixscqa.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gbsahswvv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gnksjphbo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/ggeolyvcn.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gtngsvudt.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gkvsarxzn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gkjbgdjha.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gxsfbtmuc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/givvdyqqz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gwdkkkizc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gldseikut.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/grgrwmrrn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/ghzpuquac.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/grtccgqya.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gkpoyftwl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gzydnhvkx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/ghnngubbm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/ghozrrpgd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gqocjjrtg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/guktjcgfg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gawaqbkso.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gskzgxjyu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/ghcbtpzcz.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gcspwdcab.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gufkftiai.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guqergrbo.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gctelxeqb.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gkmytmgux.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gmxvshalc.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/ghrufqsdp.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gxqyozdvv.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gdwblpgly.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gmbeoernt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gqrdrigbv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gnbtkcwsv.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gqghkwqfi.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gzycnwulj.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gonorcrtc.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/glgvtegnu.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/grkgnocas.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gdtqwsens.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/geexndmsy.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/grsbbjkmo.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gmqaeopqe.sHtML


<!-- 参考信息 -->