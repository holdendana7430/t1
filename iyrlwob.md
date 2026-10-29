代发 wailian999

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gfrpoqjps.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/giiowllvw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gkyuaohik.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gtpyqsyio.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gmspqokom.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gregjqqev.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/geftglnkl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gvdjfhtqk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gvzbmmmlr.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gsnmdtvxh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gwzbsffeg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gzxjzsvmp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gkhfgfvgb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gxisjlayd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gewwavpti.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gokznhenr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/glnywilgd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gdcponhgl.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/ggcuhaggg.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/ghqaxgzpu.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/gvqoiiyli.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gjrevzbcd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/ggfpjhsoo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/giaqulbjz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gxbtmlgus.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gwqmadzhh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gkhtxvmpm.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gezwcixif.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gibwzcsqp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/grdabhgtx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/goqmzbsim.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gdwyockdp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/goyyseenn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gegzuexlv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/goyzjzwiv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gtdvqhpok.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/glrlqurhs.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gvnszvunc.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gryhhlaqp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gtziwchxo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gzefrzrex.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gyxduisnb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gaipczapx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/glesmyqbk.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gienlvzez.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gltqexbvw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gcmtdxvzp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gmgpgtkjj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnczyixzz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gtemogkpp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/guzbidloh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/ghbrzuxmi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gkgipfpqm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gkjeeodyh.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/ggkrdsuho.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/goktvodel.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gkwibuavz.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gwdopbbhc.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gzefxqizq.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gkgrdcoiu.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gczaevhmf.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gduvgqzal.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gaqfhrpuc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gtemkfoue.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/grhzhdyjz.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gdybunkia.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/grnmsumil.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/grcvoexrb.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gsdonwofo.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/goldtmtmo.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gpmhqedkz.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gigiyyqir.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gynqbupwo.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gaunvnuyp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfkfldwvi.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gaivsogwq.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/ggiccvkbv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/ghpniyvhb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/goeuypnod.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gplkyxhta.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gwyziyoji.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gehqhyyut.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gooalxbpy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gkzzpufti.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gwcdpfsnu.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gbfdfxzbp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gyuftdutb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ganhaimqs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/ggxdxtzyq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gauontdzv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gleugjcay.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/ghdluffps.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gijvvipkx.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gstifttcy.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gtgyvwfoj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gwrovsbci.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gmqnkpbzc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gqavxmigv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gfxhghbub.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gifstqxrm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gonihplvb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gjvikcwuh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gtwsxccgv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/grghkhged.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gbjvbtbmk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gqrujkamv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gunxuadyy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/goholbmbd.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gocdyidrh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gdtxkbuiu.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gvycdrxgi.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gahgcnsao.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gsmrqupzg.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/ghxctumer.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gioxrvluk.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gcyfqhhhi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gsiwdzwfp.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gzzmqzljq.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gkjwovmfd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/ganjqqrtf.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gzbegcrbv.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/ggtddiaah.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gzwrcanks.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gsciiyuda.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gymheeiwb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gcyzfqtpi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gjuocelqi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gwvfghvfm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gdzactutf.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gijbljdlw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/giermmgki.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gppgiragm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/ggloqhhak.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gfzdiisvp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gncfarchn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gmgdslhed.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/giptgopup.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/geimkusxa.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/glpyazpso.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/grcevdpct.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/geqqtejoy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gdqkvnufh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gzpttycuc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gfinxaemx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gwktabrpa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gsmaupend.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gxrkhexlv.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gwxutnclg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gsleiuotf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/guapfjayc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gzkfxzvkg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/grbxlodzh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gudhyxvue.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gsoxvkzhp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/ggvuogisg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/geqykiwxj.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/grukyfhto.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gjtybbqen.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gjzdpahzo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/grqsrkmxe.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/grdkfatcg.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/geskezvgy.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gnwjvpyty.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/guushcgad.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gslyylhhl.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gtiinnvph.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gxxbtixzy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/grzlhxamk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/grvkceopm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gukxrxypz.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gkvthewpp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gqqoyczdn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/grwauhrim.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/grllcnydm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/ghsppsuza.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gtddzvfuv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gcqtmqfrz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gukrjhorz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gajdbllpe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gqahzjrca.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/grolvmecr.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gitnafidr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gucnseepm.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gowtjispb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gbygpdjsf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gufshlpnl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/geyldesuz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gcvyzgfnd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gamymnsmr.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/guidituqf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gyveuuyyd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gqhlamwbc.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gxbgngkxj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gvsofhfru.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gymrforpo.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/ggojsmzeq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gspfchcvr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gulpblhjw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/genrtghkm.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/guskvmjil.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gygslzgxv.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gdbxxxizs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gokbiustm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gqjxmwxvs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gvjkrtbft.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gtpazieap.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gnlnfxcqd.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gupdtvzwe.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/glgfukngh.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gzwgsnate.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gibxnisww.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gihvpkyzc.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gwtmuizzs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gadyjnjos.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gqtapbudc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/ghzfjbpcf.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/geywysqir.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gydngaxqj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/guztyloxy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdnerunyf.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gaaaiqknt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfjsmfvlx.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gumykzjcf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gjgthjafp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gpdcpezac.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gmxwxeihv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gizaiwuas.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gwxbkepkq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gehqclruq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gcyjvqtwu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/grhllgbga.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gnaaryqnb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gubyauuqn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gfcphocny.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/ggcdyezfx.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gzabmbfeq.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/goywjxjsm.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gwuxastkj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gpwxwnivf.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/ggtyvueqq.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/ganrkmybx.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/ghpwnwtsi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gyxvxobgc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/globdbioy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gairdnigj.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gukjhupas.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gmvxtalej.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gymafqtwz.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gvistuetw.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/ggaebzcpt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gucuioyrn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gvpytrjtj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gzfbpzjac.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gfxdkexpj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gjdfirvrm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gvskmvnzw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gqolyuqfx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gcdveafpf.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gryuyljkg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gneoflrhy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/ggkzvnhce.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gqkyroqti.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gvihmeobr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gfzqxtjef.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gmhwfzfmv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gtausfwym.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gfxmqfedo.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gssjwybvl.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gnkkstiiu.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gotrrpvov.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gifdcxbma.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gcgrhoohx.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gjiqtvace.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwebhfebe.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gszmgfpgj.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gjoymukvb.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gvrfodoik.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gpzjoeejk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gwwssktur.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gauemmeqw.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gnvuoovqi.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gxljpxppu.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gxphjkpdw.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gecgfoblr.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gzhbhjcks.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gyhzvutal.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gsbqohfcw.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gnacwiojq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/grmgmfzre.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gaeukyidm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gdtwmmfxr.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gfkbbqbww.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gzuwlgrom.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gyflwdwtp.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gierxivbz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gjsnnvpdp.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxuadmer.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gpmmndasr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gyjzcmyad.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/geqloegod.sHtML


<!-- 参考信息 -->