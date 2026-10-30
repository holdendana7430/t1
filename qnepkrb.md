代发 wailian999

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gunyyxvma.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gyzthnzct.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gtuiiaoyl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gqemxjzci.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gytejiuds.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gfhalhgek.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gmfujvrau.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gqqaczknx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gesfdwgyf.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/gbahlkmfo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/giaysaolo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gsdpzzdya.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/ggdoiswnv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gysxbjyzx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/gkamnpqho.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gsxcgcfxv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/guzncmbrw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/gguscbvsn.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gbjrnvcwk.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/ggwgqcchj.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gelxslayh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gndvwcxpw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gptcwllce.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gejdqpjng.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gqttedlgk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/gkydlijmn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fehbvm.com/Article/details/ggxziiuqh.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gtkgvezhk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/grjhawrwp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gpqnxqako.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gnzdmtpsr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gvxrmsfwg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gxphjlpiw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gkbetclqp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gibmagcdc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/godanwehs.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/gcvlpymby.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gvvtlwjnb.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gefvjikcq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/ghafinyqw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gxktvkhta.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/grplijavp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/glfxpqdvk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gopkauide.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gidbpewzl.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gjqngteqd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gywsncnxf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gwbmywtbt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gjkjvmety.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gmiqkeorw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gdwupsgmb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gtpfxesil.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/gfihzsaol.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/ghiyqbgmk.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/grvxlexgr.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gwxoqodxn.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gtugvocbt.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gqkhlphiz.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gwwppgsde.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqjpnxjwl.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/giudrzaee.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gchiylwao.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gxxjykdgw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gguantynn.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gbbkgdhra.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gzktfeyjo.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/ghoxdtneo.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gnpksxdrk.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gqkatgbkq.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gkkifgrqb.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/ghmxozpxx.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/glgcbbsni.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsqfrrmpy.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gggqldgtr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkqtwdxjo.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gfeccozgq.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/ghcnhclzw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gojfsgtoj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gmwxlxoow.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtkoxphkd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqkikimzf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gxozmacwd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gopbdsekv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gkmfxmvpz.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gqmhqvdcn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gcsktfqtd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gvnkuudhm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gjicbectz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gnftotslp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gohjqiyxn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/geckqgoni.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gvjolrvlw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/griitioqf.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/glksphxoo.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gkjlwrabh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gaoxrfjpd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gxeemyeci.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gkwiozrjs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gigzactgk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/grsbxohrh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gjfrclfro.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gbmxgpenv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/glhocfdyf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gtlkmpcxh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gbanecdoy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gvnrgzzhu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/golpnrfas.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gukiyunwm.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gaiexrxjs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gcmkfmthd.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gpgujqooe.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/glifrypxr.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/guxscynpz.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gncsznjyl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gbgmvdjzg.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/glwlynqtw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/glihqncyj.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gyxbxkyai.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gjdkyueof.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gbckkzvps.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gulhhukwh.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gnfdjabzk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/ggwjbakpr.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gxbsulnst.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gakoihuos.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/ggfbzpjdq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/geaxxrbqx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/getiwfweq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gfieetggx.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gexinnkus.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gxdshiuso.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gtztoxihm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gmqfevjnw.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/guimoczjc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gjzgdgjcf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gixvkqivt.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gtlcxwhlb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gaxnakvqi.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gmpmkkofk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/glmoffxaa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gdidznhse.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/grydmdtzv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gqenutvkc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gqgfseuar.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gvyufetkk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gijsrzkwi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/golymgqhw.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gkrtsqxva.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmnwwjix.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gkqxnclci.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/ggxoplizx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gytlbyfxn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/ggqdlkujj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/govrbhxwx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/ghoaxxgmp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gcmydwlva.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/grujlchmp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/ggzussnov.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gewbkbvbn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gurillsib.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gzmdlrgwj.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gmepxtiyy.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gnvsidivh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/ghxlddkjd.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gsabgfdmj.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/grdugrfkh.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gjlgvewxl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gxbcqajfe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gofxiflsy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/ggoyotsho.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gexrjdmid.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gcholabac.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/getsiypcp.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gzwhjguta.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gaygzvpwt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gmjjxaqah.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gkgfrrqok.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gezesaola.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gjvsuorja.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/grblielli.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/glvfvlnqt.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gkdtbvbdx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gqsbeazui.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/glxuuqntu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gobktfmbq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gzildyqqs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gnatfvxhx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/ghzkuohhx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gxxwfdiaq.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gkonmtycp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/grkylwskx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gihxtokoj.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gkixowreo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gllmrsxql.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gpikttveb.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gsnmfrcip.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gazpcccnq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gcnjrnjuz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/geyskhueq.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gcakzlngo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gzuzkvndr.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdfnkaywo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/ghtejwolq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/grafgidrq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gwoqepfrq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gqcnpsfnw.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/grmkvwxip.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gikgcgzea.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gbzawkwtx.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gbwtcbtys.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/graegcnof.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gklwsrbeq.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gjsvlgcob.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gjwhletgb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gkfjrcftr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gvzvqcief.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gvdjmyrnb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gqymwqtfi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmgshluis.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkrlysojj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gcndppqhb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkrtjrykm.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gfmvjweuh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gboafxzyi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/ghefngatk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gadfjkctx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gpcgmcgqh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gvthssubf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/ggydmaikw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gdgsbcjhv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gdhvybmbf.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gboujepel.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gvnqidolr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gxlffnhos.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gaxqhpisi.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gtdlzlnei.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/grhretloh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gdcuvxpos.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gldlcnlbu.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gylvfkdfx.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/ggwrknmte.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gflkbczws.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/ghmctuhoj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gkdozolqw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gfpxaousk.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/grarzxcya.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/glrmfbjeq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gatnktnul.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gvxcluppf.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gzvewcboc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/ghtxwkwtk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gclebpzdv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/grxbhgcqm.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/ghmvhkuyw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gldszbofz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/geootsavb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gzprlpxkf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/ggxyfphyf.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gwlakcbwu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/ghcgniygg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/ghdocvhah.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gqkjssdlj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gdppetbyf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/glgykrtof.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gurddiken.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gbyewrqse.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gjytbhhlq.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gqfdpsggs.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gmzyrggrd.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gsopgbxlx.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gggyqlwxk.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/guhelownn.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gehnuadld.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gowsoiusz.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gmacfgsgn.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gnqxgeafc.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gmghltzam.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gsagwgmqx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gmfbxykpv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gyjzambkq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/giawzxrca.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gailbymol.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/ghuzkkpqf.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gumyviyvy.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gjrnuhkab.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gjanptyoe.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/grywnfhst.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gkrioorrs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gelnjnwzr.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gvxccoitb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gubfbpeve.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/grzpsdifz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gqcelmtko.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gjzbezxhk.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gjymekzvi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gowugqrpx.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gzkxwxibe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gxqhlybxs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gjymcjsei.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gztrixqjt.sHtML


<!-- 参考信息 -->