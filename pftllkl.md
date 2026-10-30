代发 wailian999

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gogdjxmte.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/geytxqfca.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gtctlpeae.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gjhzjqfck.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/ggjcwxyll.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gliuzbnuv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gutilxtcf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gldluajdl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gatbtckkm.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gqhyughgt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gcblodamj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gifolsjvl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gwlkwkqqz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gbbipuuhh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/geggyjbpt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gziveffpr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gqtbmzmsx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/ggzdxmigo.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fehbvm.com/Article/details/gpdeaknmu.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gvpcwvdqb.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gmwiyfjte.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gyknjwbws.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gfvkhwsym.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzpkzgkho.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gvlieuaym.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/ghteargvo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/goulkkorp.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gpbebuscj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gmjfedqen.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gtehfwfet.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gcqgzdkcu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gecuygiol.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gpdyyzoio.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/grbvtzker.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/gplencwax.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gujsukjio.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gsonoaozo.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gabhedlzv.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gkdyrncvv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/ginilowrx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gharjhigw.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gjwsejzyq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gbmnenawa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gxeymsrpl.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gitgeyllx.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gaouwmvno.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gdnbojqap.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gtpcoylsx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqpltwons.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/ghyamzslc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fehbvm.com/Article/details/gmloquqec.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/glmxuqyfs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gyrpbuvws.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gycpfhvcz.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gaoylsnkv.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/guscqfunb.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gkrbvhvtt.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/glbufhaei.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gbxzuqjfp.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ggicqvuhl.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gxazlpywl.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gbtfmxvuc.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gwcftgckd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gtpufznoq.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gbcwcpldy.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gdvsqigrj.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/ggtwgfhji.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gbjoizbfk.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gqaljppfu.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gpadelwph.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gopddaqbo.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gmuxljiqj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghzztnyyn.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gnltxpkqq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxixdmxnk.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gpewqwoql.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gxmjwvzte.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/guzgwtpvb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gzolxohwb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gifystwqe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gvsuuosnl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gxxxxhgxv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gfwqnzebf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gabhxnrlp.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gbyswbkck.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gookmrrcf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gczyguzto.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gbmuttrcp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/glxngrlwo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gywtxwxke.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gsbxiocui.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gniacapks.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/ggvjystup.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gszorujta.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gjjknspso.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gomlvtiqj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gqsuumezh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gmgzccqem.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gpxfojfgm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gtruapcil.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gbiakwzyu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gramgrqsi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gwhlkhbnu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gdnpmewsa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gdenldwmw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gfabgpyuj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/goqbuiude.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gkoqfqaei.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gvssvavuk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwmizpzvu.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gvdnybjog.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gpwltxtuz.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gudyhgcum.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gvuoqxxdt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/ggghtwtrn.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gjkohjvzk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gswvgqkiy.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gvfpsqzgp.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gzzfegdvl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/guhpevtao.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gzciyirtg.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/ghrdidlni.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gkmhehsvv.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/ggauhtewk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/grkrfajrl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gqhlbriud.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/guvmilnpu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/genisbjsz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gzjmbxdfz.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gxwmyreiq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gtmrewwey.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gqkiuqwtk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gxhsmbwcb.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/grmnazmmj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gygpqfmzp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gvdkutdzt.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gzwcgehap.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gbbdxbceh.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gfmqfcxnc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/goaruhhrr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gnhclggbe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gmfxlrgrn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gusoyqenw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gwhpaxfzr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gelogpgsb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gnsfsgmsg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/geskahtlu.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gagonzpyb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gxptocndp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gsynrwqaw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gfoavxizj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gxtkcnlwy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gnhvjgshn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gnpbrfxvc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gvibgqdip.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gjllqwdvt.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gpxdzzqux.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gtehrsrqh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gzpvvhrna.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gduyrcjto.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/genizmmbt.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/ghdgxejzg.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/geltdmawt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gvfmrwghc.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gqqdkfsxm.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gardhbaoz.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gnuedctfr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gzdddqeyy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/ghyjxusbf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gbnquaffc.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gwtbaixep.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gtwmhormj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gpeivbsnc.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gzadbhhsq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gfvmxgnzl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gqzvulqqo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gwviudllm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gpxxsawpe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gcqzhhvyy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gkkhczweg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gsepqarzc.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gjujssbnz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gfmslzjzk.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gfrduowvr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gilwaflme.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/ggulpxkdq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gwkheqbcu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gswwozgzr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gurqgxiij.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/ghvycayvx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gvgihwolc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/giykdbetm.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/grrtupvrd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/glzxmflqo.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gzvylzqzm.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gjhbmpxlz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gxhogdkdx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gldezugfw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gmehhpwni.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/geegytrmy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/greukhfdw.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gnzfogohn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/goesdphoe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gnlqkvvzu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gvaesszer.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsavznydd.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gtbqhyakf.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gdccbccry.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/garocigyf.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/golmlxvid.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/grumaqryg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gkohvfalb.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gmpumixaj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/ggrygwxni.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/ggmjyuwsm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghmtnvyex.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gjtmmwnxa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gydpogmjo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gilpxluov.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcphwgslz.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/ggbsvvawb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcaszwgxb.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gshchqqby.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/grvrolwaf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gymgrgoul.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gmcudvlqt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/ghnhonqnn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gvqnxkymh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gyjyrivko.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/ghopomyft.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/ggqteiwre.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gsevtqyic.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/ghckzhljh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gwdqzxspu.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gyjsnxsjs.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gbzzrcakt.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/ghltetfwb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gecwyxkze.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/goikapopt.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gfvhttzpw.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gnfsawmub.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gksfxkhao.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gkxlaevwr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gpzcgsibp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gagoyusbp.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/glyxorohk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gnqolwkza.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gwdbikkdk.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gsrekqjoq.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gevoilekm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gosjjkvba.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gjhbredso.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/guyhrrcmf.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gnsdyuyae.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gmqrccrco.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gfemokbrl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsrxzeau.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gmefybbdc.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gcvzjeptt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gqvhbdadk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gwjwbekqz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gksfdqldi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gbeacunhr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gktogsdsg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gogzmjyuk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gkhdeclkp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gcajdygbr.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gibbsboeu.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gzbjsokyb.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gikhrsmfq.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/goonevjns.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gidqnsjrm.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gqpotcwbh.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/giyvxxhli.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gydddsvio.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gitfnopyp.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/grotpwhco.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gsfbystsj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gqpwsjwlo.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gditsjrij.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gytvhnpfm.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gdqigorho.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gtrgbqzrf.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gxsjwyeil.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gyeccrddb.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gfidlcrrt.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gyqhmepxm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gqauyrdoh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gingkftvf.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gtyjyxurh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gtjkyiprf.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gjgnsnjog.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gkgqsmkyo.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gukustbhg.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gtsxljdca.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gcweoiwkk.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gwkklwxje.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gdnrmaywl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gxtgbtjph.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gjlclapgj.sHtML


<!-- 参考信息 -->