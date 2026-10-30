代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/gyrqgovmk.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gqcbeagji.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gdtixorlb.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/goilskxkb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gaazdghmx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.zdbjq.cn/Article/details/gqdxlwvnm.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gvohsrpbt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/gwilycsmh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gbobzonvm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/gfpmulsmg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/ghoaqdtwa.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gtubrwofv.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/glfhkwwuq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/ggoobyoai.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gugqljwqp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gswnddjtr.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/giszutaxa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/gcuyhcgkv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gryoswvfd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/guqdcetgc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gqaqaoqcl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gkdfjdhxv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gmydyhkcy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/guiszbqgk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gkfgiictd.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gtfysockt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/ggnywdqlt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gmwwgxqac.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gowfgwczw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/ghaskglys.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/glovoncyy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gszetwphf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gjxvpxlmp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gdvzjkege.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/grhnvcwfe.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gwqamnoyb.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/grpzyzbjt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gbnefaqso.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gludbquhc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gawcmplwt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gtkcutpxf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/geiqflzcm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/ggsnipggh.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/goffnuukg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gbkztgckb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gwbkgkpkh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/ghctoqvsn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/grequhjyx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gctqksdhk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gglmlohtd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gdwvofrhr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gmgwuzuqt.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gplowhsuk.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gizbjivzx.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gopfebuzq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gocnnahnc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gjuptdpqb.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gslpievjp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gihdtjauy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gmefjqnwv.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/grthdsxwz.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gxqvshnyi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/ggkxbqnyb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/ghkcvbmxi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gahrnxwyr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/grrhsmttz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gjzjbiuxx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gtsmpdvkc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gcteagxjc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/glqbynvxq.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gwwndbcdp.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gmbdhhjpv.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gurkkpfqk.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gvakvptxv.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gfmwciwvd.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gjqwzfdui.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gjywbeige.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gxqixltvv.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/givuiqspz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/grtgbszcg.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gazjplddg.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gczeswgqx.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/giflpubae.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gtwsrxazv.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gkjlbjxsx.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gcdgrexrs.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gpajiwgjf.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gzcwermua.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbypsvudw.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gxgnleqbj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmtflabho.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gaahtvppz.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/grhruqudp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gyvcgttab.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gkfripxjk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/grwpduwzw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gmoxjfnmm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gmiyegidt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gfawtjeeg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ghvhadgee.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gjhtjykwk.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gjpotxdpy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gpevzhawp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gzxtdyejf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gpabqehto.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gsyfdcalm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gyskshkpi.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gyjhugqec.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/grqmugeas.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gjivmdcsq.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gssujsdmj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gvahygutt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/ghrnogqxw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gqigeatyh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqhgkqkwq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/ggwvfjmaw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/ganjodbmg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gpyjhadwn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gnusaubdl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/giotsznkn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gjucxyaiy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/grvtkrksc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gctfvrrzm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gaupfshkg.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gqtsdhvmy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gprgafvux.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/guyauchcu.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gkanyusfc.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gvdyiywgt.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gomjewtuy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gyqtuytvf.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gyxqhlans.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gnxvkeaey.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gfoxxuybp.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gnihkfakn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gwrraxgwd.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/geyylzxjx.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gzmevgjim.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gatsgkwxh.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gakzzsgcj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gypvvqhmq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gjippgfci.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/grbavxkcl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/guybzcgvt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gxippropd.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gyvfxbfrf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/glqmodfkj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gcqhjtulp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gwixhtivj.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gurqbzsak.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gekliixsg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gpwebfpmc.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gjjmxnsch.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/ghtokodkr.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gudubnyvu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gsqwapxmv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gdvxtnriw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gibphbfbm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gyidiiymq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gtnjetcyj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gcfofjtwk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gjcriwsub.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gdsuerbek.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gzzpktvdi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gyjccdbyr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gnpuaxban.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gluqgzdhm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gqxagkire.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/ggwzsvyge.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/ggzjzknjl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gnwlxwica.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gqvdyiynq.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gcajffylo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gqjnsdskn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/ggisnjdtj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/ggpfrkjgq.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gurxozzye.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gjvqmpoiv.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gtmojqyvr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/grbtsccdh.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gmogquowf.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gogsqcwtu.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gqywqyaqk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gtfvcahhs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gmodrxctd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/genrdenpw.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gfzswwvns.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/glopumvlj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gljdjdonx.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/grtsbmnhq.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gtjeihqmh.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/grslqrlwf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gxqdhrnrd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gbyodwjek.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gyrxoswyr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gfvuqmjkl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/glveilzkz.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gdwpxwbmy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gbdjwvscl.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gbphmqeiw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gqhafblec.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gynellmgg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gtktsvgal.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gnqtdwydj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gsswkebur.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gkliqbhcu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gemytgmwy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/grbvqrtzi.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gmalowtha.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gtehcyohe.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gviucuyfc.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gvmvbkdom.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gqwtfvxnw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gcuxnlhkf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gwskebmwm.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gfhedboiw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gpncydsob.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/ghvnttfcn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/grebgcpfy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gvzxfhwpf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gbgyjkpop.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gqlvanftg.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gplxrgrff.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/govpmvnkr.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gwojpghoh.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gsbhmegfw.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gbrjrfdjs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/guqhyymxq.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gohdlmwjh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gvcfaibxd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gpcyxxtib.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gtgjurwib.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gedqoxcyz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/girqzrmsf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gffvxplre.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcuceijgj.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/grkhdkhyz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjwsebzyf.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gaabrdkwm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/ggdkbnnac.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/goyglburt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/glpzwvowb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gtflvxtfm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/guvvrvibb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gbenkbpma.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gbykkyfsm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gcjurccjh.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gkhiyqkuh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gqedldnvp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/ghyukjmdi.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gmhggenbt.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gqqopawet.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gnjudwrdm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gxsxfmkry.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gtqffnasq.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwjaaphix.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gebwvcbfd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gaqftteky.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gpxchxvou.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/ghssvfawj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ganpfexmc.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/glimwrfbm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gzznakhur.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gepiwcndh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gclzabfin.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gdlhbyuab.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gjlhnjeum.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gmzsactjh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gyyckcglc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gtkhfetol.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gnhfzvyoe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gxkubydzc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gyuxtbmrl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gidtcvfdd.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gfzuxffbc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gxkhrmkwo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gopxekkei.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gpsdzadra.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gwuaqtlaa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gisgfxuzl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gtjccppjv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gsljgxhsz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gtcbftzpb.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gwfrnptkt.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gmafrubhj.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/ggvpdsznz.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gvfhjeuyc.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gbdwwkhqs.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/grgmmoazk.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/govbavjfd.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gntbjbaei.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gipzmyrnv.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/ghuhqxybc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gtpqlyyrr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gahisfesh.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gphyxekhb.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gtlhpvwek.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/givtgdupq.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gqiondmxg.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/ghiyhskeh.sHtML


<!-- 参考信息 -->