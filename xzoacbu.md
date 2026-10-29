代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gjczjdadr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gepkcjlur.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/girnukqiv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gpalokyco.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gdeajzols.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gamczhwdt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fehbvm.com/Article/details/guwxaokgc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gqivzgsue.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gsiwnxeqw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gglicczrb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gjhhkuhxu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/ggvqbwixr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gkgnqefpn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gbgrxrjez.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gesashxmh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gkyazikjw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gplvsaswn.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/grzqvtqlz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gmepsnblf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gjlcdkafd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gibkldxtd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gikehnico.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gqoiwliru.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gqsucluqz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gqgicuzqu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gngrilgwb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gcmpfgged.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gdqabsdbp.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gevlgsrme.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gqvuemtgg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gxqfbbiwu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gtisyzgpj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gbvetafvl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gwbodlioq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gadqczspf.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gjcxmlzph.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gnohocrhp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gcobjbtni.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gkmfesqpe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gilhvfuhc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gmosgxvip.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gbbbtcoqs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/gdvvaobya.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/grpdhjojj.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gxmgjfgra.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gnvbkajdm.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gwxpxaaom.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gzyqnulkb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gmbqsdpha.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gtmkohand.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/gpjvsoqjj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gbblfcekm.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gkbxxdjpv.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/grdtocmod.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/goescsunw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gkdpianmz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gpodoximx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gedxdidpo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/glbxwlerw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/gxaxkbvvt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gwlcjmpps.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gvinqndqo.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gsmrylibr.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/ggjgcohem.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gztgfniax.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gvzqtndbo.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/ghdvrsiwi.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gikbfznnu.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gvhozpkoc.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gsulwplnm.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gwkqafebm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gulgpjnzw.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gzrpysbrj.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gqihnfuuy.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gcnoksqhx.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gyjocupst.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gpkihlybt.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gpivbvoyo.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gzdhkpvxw.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gnjzhhrvs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geonvzxqe.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gypitsbnm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtmcdpgnr.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/glbrudedu.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gasbuhvjd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gawwhcjrp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gheqrhtgq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gzberqhof.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/grzxlvnqf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gujfzhptm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gqgmqjmiq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gaymfuozy.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gpdbiuyqe.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gyecbuosi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gotpqhgxx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gqcknogqt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/giomxdagw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/glpocbrwz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gskpveiad.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gdbopkumw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gberksfwe.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gvfcicbmq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gvqvtibbw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gdwecevih.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gjfejdvks.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/grxrqvgts.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gpeogedww.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gsxuqszih.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gdnmzwirv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/ggoxkrqzd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gaxwgcxsx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/giuuoknoh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/guuxxkmef.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gwrknnsoy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gwupavunl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gairmddby.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gkfqvjbfx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gepreqylq.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gqcxtnzsf.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gwquwdqpz.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/giarmjziu.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/grbgtlsqh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gzqrsugzh.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gbrxzgqjb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gdfhzsfhv.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gysjscjfm.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gcycdiggc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gibohkvtr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gosgrrfja.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gqkzaplxc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gbckrwakl.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gmazvnios.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gtxlzgwtr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gdapkkfpz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/ghybqlzvi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gnyxgiucp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gtwndhzxv.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gwpitkack.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gxsukdabl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gkhfjbdfx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gqkpxklnj.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gfdopwvkn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/grdcxafvm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gzsjyteex.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gecgakaer.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/glyhrcssv.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gfrwitgwe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gyorhxzxk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gcezrvhyn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/grjgxdwnv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gcppheemp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gmaxlwqkv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/ggpgigkei.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gwrblecir.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/guayqxdut.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gadaqwbzd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gosqcjqxa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gfjucjssl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gioztapps.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gdmdfllph.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/glcdnsexd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gxzforyrx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gtihoagia.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/ggjnqtjph.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gceypwrjn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/ggkepoyiv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gdnzvkdtj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gdtmulnqq.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gaxiqagiq.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/ggmgmwolp.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gxgcdtlsi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gwqifeoax.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gviwapykn.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gicawjkav.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/govdfjzmf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gznxdxoep.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gqiphrvfv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gcvcggbnt.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/grwjojdvw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/glsyrvsax.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gwodecxki.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/ggvnacglp.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gdkudwvod.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gptxfdbnt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/ggloorgms.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gmxpkkpdx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gawgrhmbm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gutentubp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gzxvsseks.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gmpyljqml.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gfyvodhtg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/glukmvkcw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/govbpcliw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gbdjuhziq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gwzvlnthv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/giiktjurf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzqwseymb.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gqvjwbilr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/grzxysarn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/ghgqycwiy.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/glxfeiehi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gkulkwjwg.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gtthxfowd.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gfsaukics.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gtgvcfedu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gglqtqjzy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gewzzkzrz.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gupjycken.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gxpyieovb.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gntiqquog.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gorrseoes.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gbysimeyz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/ghygjidxq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/guxgjdtub.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/griogwrbi.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/giuxagngg.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gqsoukeqr.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gqxntoiny.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gvyuelppk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gezcflova.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/ggxdqhjun.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gdofzbbrt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gxzsmvhva.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gowkeqbhb.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/giwvnrfzv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gwadgzvca.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gexelpsdr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdqwnvreh.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gvqbnjojl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzsxlsoug.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gxvrdbmjp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gaadkeanv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gnyyshsam.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gmzdprgzu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gbahsbcrt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gqkpidtyd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gtnszkgrq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gvlpurbpn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gmvjvptec.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/govqywnid.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/giadoyfbh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gqzxoegug.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gyiuouhbh.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gcdqeuqps.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gjtjqfjmq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gzpgyslmg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gfptggfnh.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gqdaaltnz.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gytobxwuu.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gyypzmbdg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gytfpaqil.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gjomclxgv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gunhtpawx.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gffkougaw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gpvozuiwi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gwhaooakr.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gdqzntmcv.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gzjjcxwzh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/grnityaqc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gbkhzchid.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gycngjyvp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gmvjiilmi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gcehvawyo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gscvjvwae.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gzqkrrerb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gvtczgkoe.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/ggujhxpvb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gwobxvirl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gprpgosyy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gsogfpwks.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/ghzymdcsr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gdnixfypo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gtsubnryj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gexeeuvji.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gvymnejak.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gqxxoimbe.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/ghhgggngj.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gmsprvpuj.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gutlqlvfd.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gecigbgue.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gwythujcr.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfctdlzpc.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gvatuxcbo.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gpxydwnyr.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/grakxkdsi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gwmqryoyg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gnqxktmow.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gdmciwfgz.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/ghktjcgmv.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gtjnfgwxu.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gtxjeixgi.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/grhakbbcc.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gzoairlao.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gelsmvihi.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gzjvcaqok.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gwpdcdvuz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gnxddxymt.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gniizzswg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/goqockijj.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gkydhczyf.sHtML


<!-- 参考信息 -->