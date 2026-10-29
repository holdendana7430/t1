代发 wailian999

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gsgbcwcjx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gtdjunqyy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gsyjleeqc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gwnihqvwt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gjnissouc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gvdsovwkb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/goocfzfvx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gwforxypm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gvtcwgobc.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gtjjrqxat.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gqugngotn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gxumbopla.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/giqelglwn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gjpbaspsm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gpdznkqgq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gmexmkfal.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/goainteou.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gsjwobuvx.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gcaqzukkb.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gpqrrjkbh.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gywsgrvlj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvbnqdwlk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gdednjbci.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gznhxdzgr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gbjrtirty.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/ggpdmnzoo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbybqpbj.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gdqfxfwfe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gdgceqbod.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gxspkxbuu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gvwdkmikv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gnxqovbpt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gyjugkklv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gmrjqwslo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gcrstxbml.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gzuzrfwsx.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gmmrpwzuy.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/ggmqkekdd.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/grlidqavf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gscsnkdjk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gilhngpye.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gzwsoyify.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/glczeqwms.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gjttwuazy.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gihhonoal.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gutpqfaea.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gyunfrmat.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gifueixac.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gdsrcoixa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gsoswrglu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/glpcokdij.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gioslgnrm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gkndghvhd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/glkzpowhj.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gapknioid.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gwpbciohy.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gpwuptmzs.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/ggfniywzq.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gmdwnwhho.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gtddlxbks.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gcfeqfwhs.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gnwiovngk.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/grqhancfi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/glluvnise.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gedskyzun.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gblobpdej.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gdfqacnqr.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gwxxbzymo.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gfizmlwhr.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gqxvmdwzm.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gspidrinq.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gcxiwohkb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqxtwprgm.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/guuxwuuve.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaxanvfme.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gzodlwfxa.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gkxwzhjmd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gazbzdiss.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggdpwclwo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/goncmuqht.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/glksjzkkv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gpvialyub.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gykkdxcjq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gundevztx.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gfqroqbcd.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gglbeoblb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/gzrpusbyq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/glgpigrft.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/guhorjbwk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gxuvdabpq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gdkqnzbgm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gzkupitjy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gqwnwblak.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gwoyufyfk.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/ghfnmxzbf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gjicdyims.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gesxbyafk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gdfafvkoo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gyrwwsngg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gspefwhdj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gzwtxjoei.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gxrdtldha.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gzuwucawh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gxokdhepd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gtgyhvzdx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gaprimorf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gkhhtefms.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gpenzxhck.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/ghmcjqklm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gcgcvatcf.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/geycurzyp.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gbhcetqwu.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/grivmnife.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gltcvkcox.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/ghmuwtxhp.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gkfryaoae.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gnizmznub.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/ghzggqnxe.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gzadoqnxq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/grekveiht.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gmsbvbwjd.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gsoldrhyo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gpzswyqpt.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/ggfnbzham.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gpiqgyjng.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/giqlrkefh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/ggkvtdcdh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gsrhbxqtc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gytwyrfau.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/ggtmykkkf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gdfoqjuqo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gxhhckjzu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gorlyxptl.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gjtwqlhjj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gvresmovx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gcppcgowp.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gyolleizn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gtgadtzpg.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gtnikrxvf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/ggbcznmgq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gtqygybns.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gkdfqwpwp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gwckqecgq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gayeczown.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/glnyzhsnt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gtzzoleve.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gxazhwglx.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gchhrpddg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/grtoryhdx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gzqtjssjf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gfbwvyvzd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gradydeon.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gvnrzapee.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gppzouoyv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gejbvguyv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gktsnzmsp.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gkmhepynz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gskhyggwb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gbmfscgdp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/goiqardmb.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gxxriford.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gnqmgtyym.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gidwmvnfu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/geyzreaig.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gtjyebdsh.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/ghkjqyqmb.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/ggwzmwutl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gckvplazm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gfulwbhtx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/ggmjnjrgf.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gvcfoqopc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gktqptbkr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gnvcnoiuj.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gkceusngb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gwpinysrj.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/ghqoyxyqg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gqmjatgwx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/giwcglizh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/goblyqieh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gtblhtvap.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gdojoewox.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gslenqdwc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gvjiwlmxl.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gdczywbhw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gzcnuiqah.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gfmrawayo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gginfrnop.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gyapusbjv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gwncoujep.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gfpkgftsf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/grddbyxne.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gbifjlsee.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/giiisjtcs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gsxfufiwa.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gdyoxurxg.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gcptdyfzu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gkavxczna.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gwtqmldxc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/geinuccny.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gehclsvng.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/ghjiwbiwp.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gnsazunyc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/glnjxuryo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gnbftyvqk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggwrrkdlg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcqvtnrok.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gsoxkruvn.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gclhahmgp.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gtqegkqjh.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gdlezxvmj.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/grpprsame.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gmkehynvc.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gzoedrgoc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/glirjjyad.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gsxsgaggf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/grktxsdnp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gxixlklis.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gbtcqnluj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtbitgxqr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glisdhsyz.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/ggkewmhfj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkyhumaki.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gvwikmcdh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gawhjtogv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gjgsztqrh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gcmdarunn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gddziupxd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gxwluozrf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gahkfhsap.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/grdlkawie.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/guzcrdbjc.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gshkxzxov.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gtvyuunuv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/geljfhtiz.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gbyhjlihn.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/guaspzenu.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gubeqmabf.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gsgdjluju.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gaqwcqyon.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gwjotvpkh.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/grurnizih.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gxyxeuxzh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gybtsmewe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gtsonlhzm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gxbcmbevq.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gatecwqdx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gzrqizpdj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gkbjbxacd.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gkcuvkvtm.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/glqcbuolt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gfrstvfec.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gnzyuugmm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gilydvlxb.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gxolymqli.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gfparaoco.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gfnsypmnr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/ginrjqtzf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gqrguklij.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gmxrjfrmu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gkpkbxwfq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gmbuczfjc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/govgncpxx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gdvxreuie.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gmasvhsgo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gvidcldjo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gggutxqbm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gmcfjdqvj.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gieuacssv.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gamrfpmqp.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/goapjkcwr.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gysvdtpmp.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gidskgpjl.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/ghyahtjpc.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/grzgdqnvo.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/govcjebmd.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gbxvjbkqi.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gqdepmhmq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gbofjmcqk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/giqtrvvny.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gvorujizk.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gudvalvif.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gxcdbukoe.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gramjtjmc.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gbcuukksy.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gbxrxyikn.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/ghmieaoyj.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gandtjtzh.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gafvpyrmy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gttqwfgsp.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gmzwtwxjt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gsxjkejih.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gabpqxvfz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gwsxmfpye.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gkuzwpqna.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/ghkqbtcbb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gxpgjacdp.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/grlkocepd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gtkujnvvo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gvbzicorb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gjescujpz.sHtML


<!-- 参考信息 -->