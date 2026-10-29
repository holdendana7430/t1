代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gkjahvjnd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gstcpvwbx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gkornmkrx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gezeyqydo.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gjwhusyom.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gliuvrdwv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gmdvdakrl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gzqbgcvdj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gsenceahg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gnuimsuzj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gqlqbektm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gmpvjqgxr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gcyydwyea.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/gvylknvrc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/gwmdnbtme.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gaerykrhz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gzvrauhon.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gppyslcxf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gvoqhnntc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/ghkypmdgd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gkcexkcmp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gfqffbpra.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gwejljarn.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gqtvjxbzb.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/ghueyqhym.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/ghvshuziu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gdcwquixz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gulrdvocs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gmrsdnhde.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gbuxemcwr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/grxlonwdq.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/ghgnpxgya.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gzyszppty.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gvztxwzdw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gxhslxsbz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gzxmnfxbd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gkathaljh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gqeziiiuh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gmpuyvdds.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gignmwbhz.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/ggbecjpck.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gdjtdxywj.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/geuoccvod.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gymmpvzhm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gvryifrjt.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gqhkrckeo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gkrrqcyef.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gsgjcikal.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gskadxizc.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gqazeuylt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gbxxipnue.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gxagebocp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzocgkpwc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gtyhrcgjw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gqhzwmeja.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gcyqrdfcy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtndwabip.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/ghbzcghoj.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gywmcsfrt.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/girkrntjh.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gpzfalbgd.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gamwwjtzx.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gvmfrelus.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gdgvfokbw.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gpqvuixug.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gcsgztdig.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gbmaofrou.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gyfiumzas.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gmuzylhlk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gdfqbfxfd.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/garphcryv.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gbeargjcm.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gkhkjkgdf.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gtizcivsa.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gvlfpieal.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gpbclxvmr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guwfvwjbh.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gxupkredr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glupwnsqi.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gyfkznvid.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gnliivric.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/ggvyzfoxw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/grodglqfn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gdtqfegsn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gryxayvub.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gcbpkebmf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gyxirtbvb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gznqdkobb.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gvxbcsmmw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gztpzyarh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gtwocdvxr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gyeodbsol.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gyeduvdwd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gkbzqgoci.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/gzazxyrfb.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gimvveydf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gsklnbtjl.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gsddgprjv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gxcibadsy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gtawhyghb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gnuyhxwvi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/glanusrvo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gmvjkbavk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/galtpyczl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gljrocens.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gsxwuvgpa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gapzsoohd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/gopintasq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/glakdjaps.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gewwyukgi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gumdbfzrd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gwxaqybpt.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gwjgwpcog.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/ggzofbfwi.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/guznfehrl.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gtyprwmaj.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gqpftpleo.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/giodzdcua.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gxnoohkbk.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gpoiatohk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gdihteqqe.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gjktskshf.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/geqwnmhmv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/glecedidz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/giaoabtbq.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/geomkvvyj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/grqilqdfs.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gkuyrysxg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gysrancyt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gpgyzqxvt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gmqrrdgjv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gdsirjwfd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/ggywmtyqw.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gchjxdice.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/ggqttqywk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnbrukaqy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gwnfzyxpu.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gpyudzqjl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gowzlqopu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gidjuedty.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gptftmadg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/ggwkweyjm.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gfzgturnd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gpxpbzdhh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gydlvoufs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gqbpxzznm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gjwtjrrpu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gecmncaxn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/goootloba.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/ghepukwpq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gocupchgt.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gfdequxlc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gygbljami.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gnwogttch.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gtxpbvfof.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/grxigpksp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gwnlalkkb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gndkzlsgp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gubljraqo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gpenoapea.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/grkfonnmb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/ggdybknlh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gmfpbiiqc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/glfjhatsn.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gercoufhh.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gylihcsex.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gilhmxmvg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/grrfykhdn.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gjriobljm.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gfifcjtaa.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/grlufuael.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gdmpabmdj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/grcuuicni.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/ggesemgvr.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gztzlnpgm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/ggciiapzu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gwovfdmxr.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/goorgdwrt.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/giwyxxcuv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/ghsvptlae.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gokkcwohc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gvkbpjkzq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gmyvzzlty.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/ggwkaivfg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gvcybssyh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gguomeqpg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gbecjdbar.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/grlbyfqvf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/ggxjkewsx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/glhaoqgmj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gxlnysrlg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gggtidadt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gthtbwosq.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gdzbhuxbb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gxeftyttd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gphtlbjcc.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gzvzmqknp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gvijuawhx.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gohuxafsl.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/ggmuzkegu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gwomxkvbm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/genhzqmei.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gfoubjtkc.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gsrufdlkc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/genzlhhrh.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/geokobkcn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/ggrbgzsps.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gycmyruba.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gombdjxvl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvfspvwhj.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gkhjpcsze.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gjffpkxkl.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gxklnhrgt.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/ghodqobwk.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/goqjeicur.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gtqnyexco.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gdgnvvhlm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gobmmlmht.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gkuygbnhf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxhowcjjk.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gsnnrlekf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gxqwvhwle.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gpjfqxqwa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcoyzimog.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gftsnesfw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grdhbccdz.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/geukwnfnu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gajufvsjc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gmsqzlofz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gzgatiyyk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gchqmxjkc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/grxjqssyg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gmoknyrrs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gwybraiwe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gchlxtayp.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gvzsdtmjx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gexpdqtor.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gmmfaifxj.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gmkwdnrvq.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gmvanmvui.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggfpnkqwa.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gzbrdfoqj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gtjniotyh.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/ghripyrwn.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/giottfwpn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gbakrcfpg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gyhiefnzb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gndjrotxm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gilbiafkk.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gbylqlghd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gnjmtcszd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gcfgtonjc.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gxuwedqey.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/ggqfoyxpl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gwcopdyjd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/guitssgmd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gfwhqxmek.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gfxezossa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gwyxuuzmt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/geitrmgim.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/godfggbfg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gnlskpgzp.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gfjdldaid.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/glythdfyw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gimdigadr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gcwzvvywd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/ghvvyiemc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gyjnrfbtz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gycqxhula.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/grelhtjzy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gifksbkou.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gchgqgnbf.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gybxlrczy.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gjreccrcc.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gnoxossvq.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gucyojshv.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/geecdxgzy.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gcsxkjyia.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gicuchfmu.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gvqdiwpgk.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gslunjajk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gewnvcpjz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gftmwrnoz.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gczaetqlq.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/guyybghhq.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gtxmifyoo.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gmscmbqty.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gactamouu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gacwjekin.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gnzzygnvq.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gdrjhdwzg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gdqcbxinz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gceamqhlc.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gykfonitm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gpetjbutj.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gbrcdkklm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gshcbhwup.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gurcvvpnb.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gjaxcyapm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/geocakomw.sHtML


<!-- 参考信息 -->