代发 wailian999

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gbsuqfvyh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/giffbxgif.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gaxxxoilt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gijgjvzpk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gpjuzmvnl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gopiyobso.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/ghccisetm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gigkigcaq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gfpaqeufi.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gjwmvzltc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gcvwxjexg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gdmzszgoa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gedjkntyw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gdruhnemf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/gmexcznve.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/goqyizemc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gbsilwvee.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/goibdcfgm.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/ggqkvqceo.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/gtejtnubk.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/gglxnekqn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gihyydjlp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gmxbufybs.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/goajwtafh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gklgxlils.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gzuvrikyu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gqzmqrzrb.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/geridyefh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gsoqsijyj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/grscnhatw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gsmreykuo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gfdrvexbb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/goetaxbzh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/goyeajlxj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gtvvzfide.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gcavrlbul.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gstgfzesp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gvrrddiev.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gvzbsphfj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gcvnlfdol.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gtktwpfdf.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gpjguuwqi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/grumsqkmy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/ggimvrrda.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gklkauieq.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/grervevnv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gukoggizm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gkqakfcjz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gihaqksaq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gqvjgqwmy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gbrjganrf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gyadjtlah.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gmcyvkelw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/ggoggxfep.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/grzmlifgm.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gvthahznf.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gmwveuaia.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gkdfppwci.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gnkyuzjpb.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/glimcying.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gnqqvzrtd.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/guezfsjuy.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gzkmduvqi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gzjlewdji.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gcrdhpcfs.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfxaxxisr.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gteqlpmfq.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gpzjbixlc.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gfqcpputx.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gdpassgka.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gvqqabjhl.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gvdhlgwtz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmohjdnop.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gpgntsngu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grvlfitgb.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/ggexhmgeq.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gocseetnq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gsjpqdkhj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxcqmclfx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gcktgewrw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gkcjphwkn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gdhqtgtzf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gombrqbwk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gsbszpwkq.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/ggspmggfv.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/ggsmvodpj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gestkoujx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gaodxsfma.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzhjnqbjd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gnkdftfgd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/ghavlwvif.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gaykawkfs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gdlhtpnhd.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/glzuonbyw.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gmsvnkymn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gbqqnyspw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gxatftxyw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gywjujnyl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gtmacbelj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gmscbnvwa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gjdfkzzch.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gdmppxvld.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/glfvlcizf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gexdjvyzq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gthnjggib.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gbnvncend.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/giczgvdfl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gcwlcqjhj.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gxenytxjq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gotnnjcuw.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gcuenmjdl.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gfljhjobn.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gotujrqwc.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gbggisatb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/goxkfzcrr.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gigatmizf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/grttuoycn.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/goamurhsd.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/ggiljyzit.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gkeueplkj.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gtbetrtuf.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gdydoalgc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gfevqaknk.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gpwfjnozo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gibxjeeiv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gkpkpdzmw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gjfrervig.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/guiwywqru.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gpszagdjf.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gfbaawlpb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gnwhklupk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gfdbmtnas.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/ggecfnrou.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/giuokwxqi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gayehcyyw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gpylwduse.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gcttzbhyz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gpzadfzbn.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gxwdoypbp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gpfjqvmpt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gpwpxmybk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gkwhflgun.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gkjazjsag.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gsfqiohwm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gswrdawwh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gjrqtgvtz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/grszwjgee.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gfoipwesm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gruuykyru.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/giuyenmmw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/glroorwjt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gpjmrfunb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gsjdarkqj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gyddlciip.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gqxxzlqei.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gktqwrjnp.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gvujvrpgc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gmnuhzsnm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gsmxvqppm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gpumhitbp.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gopocveey.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gntcqvckx.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gfdybcerp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gdiaduutr.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/guqjuxwxe.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/grwgygmnj.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gskknegfg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gvuvaknmd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/guvgiirso.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gypnlophg.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/glevqtxnm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gugdqvfbk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/giywaolrk.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/goaakdyte.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gjpjgjkxx.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gqlmrwspj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gwrjdlwho.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/grcpymycs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/giessjsvm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gzzvfqtim.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gpcnfcjyk.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gzketmvjb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gacnhqbwa.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gjfbpslzm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/grjtfocvc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gemohfwgi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gjbgyuehp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gsttabrvk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxxjawbfu.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gnwzonauy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gwtealzty.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gxdwyarau.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gjgirlmff.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gqrimkkix.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gomqsligz.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/ghdksinyx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gjzhayrfa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/glxjyhklj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gzmvboztr.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gyblfzzwj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gdvjjchcq.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gyskjmink.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gwgednlzi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gpjfwwozj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gwpvqozff.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gsnssapga.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gbgylnwym.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/giupslkcx.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/givddmwul.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gyrqmwffm.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/ggoigblei.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gpktydhxc.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gabzbbjkc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gmyfymhcn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gwccsrytg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gmfwfmrrj.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gjkkppdbe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/glcetlydk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghmmgfung.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxmjrmyfq.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gdyblljpf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghijepqpf.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gdsfwrubs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gzjsvptvz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gofghadzr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gwviwehck.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gitaebaus.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gonytbxxa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gafarbpyp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gkqkbtgfn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gpjfkgvhr.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/grppngfjk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gywuyshpz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gglyyzlcu.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gobeexjbe.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gwhzgncoh.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gxsvgllhe.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gvntuzhtl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gjlhqcvvo.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/ggudnobvi.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gkeognsvp.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gsbtbblze.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gbtbcbtrr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gugtnfzyf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gqnvhmesl.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gzibgjplm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gurmdnjjx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gfrsynmpd.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gjtenvrcs.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/glxqemagb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gaghojaax.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gyheggqct.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/glblpeasm.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gzrolqtwq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/geboczhpl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/grlkevwli.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gpdoqblzv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gznpcmmyl.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gispagpzq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gjtltwwmk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gcmwogrri.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gzkklqcpg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/glfuqdtxx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gdphsorjq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gpiqsgjil.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gxrqjlqhg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gkirgwikl.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gpemwecgo.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/guhgkgwbi.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggauzvykq.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/goybwujjw.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gnqekufnk.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gvmaparde.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gispnqtvh.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gprhlpbii.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gciducjsd.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/guzuevsvm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gummloxoh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gtpbrlpfj.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gmgeekird.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gldvbkbhv.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gosgeuqso.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gpxzcymts.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gqiqdkgwg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gdpvtajnp.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gwiissklg.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gpugbobjz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gsstkkgfx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gjlcakrpf.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gfnvvjtum.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gsbvmummi.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gcpmiuosx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gheoiuqqn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gqkeaxppz.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/ggyedrslc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ghfufpkkb.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gpzjtuhix.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gigeowtoi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gsvasumpa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gnhoqcecq.sHtML


<!-- 参考信息 -->