代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gwotjbqxh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/grxkvpjld.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gekkrvajc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/ggxuxyvpb.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gcnujaisq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/giixrogxr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gfmihmjsd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/glcgaxsol.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gndizhqcz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gxfcikfod.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.hesvh.cn/Article/details/gvtdonijq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gewepxjyv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gisxyqymy.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/ggevsewna.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gwuyjxtzx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gupclwtrj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/guchgyqju.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gqrbibcfb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/gklwafsma.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gkkxzjwmu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/gccmvgcfo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gcfldsslq.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gzbzzyelw.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gzcxyvyeo.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gsuhrtazr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/glohpjjmn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gepscbvbn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gpxfafinl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gkremccfp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/giztwfqdm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gjcatcdgp.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/gpmnkhybw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gwjsixkrf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gdwejqldd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gzazlypqd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gowxgknne.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gspqlvvqf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/ghflmtntx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gvhneknjn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/giripmorq.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gzzaktijy.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/geuebxuex.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gmusldltc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gmdoldxzu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/godxyrkfh.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gvnbczzzy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gankzkmhh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gqwznbalr.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/ggeqeltln.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gjheiugml.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gbnrrtbir.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gdwiadizk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/grgybypnz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gkgczrhue.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbjqidncb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gowracjqy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gokjroatd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/govzbispw.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/ggazcrcer.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gegksnsay.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gqunfwwiu.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gctbgwphh.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/ggmlbfakg.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gzpqxfruw.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gdkvesyso.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gcmhgnewo.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gclmvihju.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gpxvyzvui.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gvqozseds.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gvhkkbeho.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gohgpedyp.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gqoxmlohv.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gjqdroblf.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gvujahpew.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/genlyttxt.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gratspvey.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtvcoydia.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gbigccqhu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcwrnqnum.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwdjwooxc.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/ggbnsznub.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gajqfsybg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/ggisjuteu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/ggoiweckm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gcshwlswb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/grakrbsek.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/giacyyrqh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/giaccqcpv.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/glxiyramp.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/ggjcoghkz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gbhmsjizf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gzmyqnpoi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gereaxeil.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gkftwikme.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gnpfozxcn.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gahtccdtx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/giacghutl.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gnrgenpfn.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gnctjzzqu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gbwnugdmt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gwtvjwvxy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gjsvcpags.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gcjgkdzuw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gbqwccrhl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gwdyilmqo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gxxzgtiyn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/guclwncgq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/geundvcja.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gmnumlbss.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gutsxuxxw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gesxgszpi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gzmidpltr.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/giwvdivab.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gfvkhrthd.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/ghbfmzahk.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gaiyrkjgh.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/ghtdjfipn.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/ggcbpbgnx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gxhaarhrd.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/grntbmqug.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gjftfhmqp.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gsaobchvg.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gqzsgdcqh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gmofmgurs.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gwxcszxzu.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gqjfcghet.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/ggilgrkhk.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gypdhycdy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gczcihzzu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gtuugmcvy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gcmaprnum.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gpgxaapob.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gvawqytrv.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/galprnpyv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/glkgockwg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/ghqvndarg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gyfqcdyuz.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gwsjrmkqs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gafyqusml.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gdjdqlbxh.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gtenaylud.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/graroidvf.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gmlafgshz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gofbfbiqn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gqyljihvm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/grnonsrcr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gtcxtnhtm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gqdohncsq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gzmcorqki.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gxafxcnti.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gsquptjev.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gmclmflip.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gnlogjyws.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gtcwnckzw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gbbroorzx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gpytptxxi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gebqhelui.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gkitnamcb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/ghybtajae.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gjtgzgqru.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gisldzwyc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gdivrpejx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/ggtumnrao.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gcltrrmis.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gawzhjqgh.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gtkkauodg.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gzflwryvr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gstojkzmx.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gsqvkvjol.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gxpksbpeu.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gdpmadvig.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/giyasldjz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gfdkmlfgg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gxsbidshx.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gskyapjpu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gvengobpe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gxkqumhrm.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gtmwoxgsw.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gjepesltf.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/geuxwrpvs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gwmronlzb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gyqsuxhyf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gesbraymy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/ggwiyexxs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gcrwsguuf.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gxbmtakvp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gmhcjlbgu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gyzsiyurm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gieoeplel.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gcgonhlaw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gdcepkkaa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gwbnqulab.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gimoqyjti.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gflzmgxhx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gpjbfswzk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gnbowicrl.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/ggduwmeqo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/ghvbvcvyj.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gejegecst.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gmlgqlbyj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/guzrtnkhd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gkhmuokgm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gzwrfbotc.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gwdeacnxw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gqeldqtmk.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gqhstujdf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gveqbhfxr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gahtqpbuy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gmbqxnxjj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gevxjpvpb.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/glyfgskza.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gsozveckt.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gqimcwlfh.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gljgutbws.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gpsofzvcy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gebebmabj.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gmnuvdwzx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gpsjfenjs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gieisdjcn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gmmdluvuc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gruxyqbpl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gebfezibh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/garapgcuz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxotrtpfu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gytmrypkf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gymrtrsit.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gztdkfaab.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gybsmrjyc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gptugprsa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/geatbpzws.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gsaaneuis.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gzeevmdyz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gxsqpaovd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gadvgcsuz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gbjbbmmjq.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gwcvungad.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gpufulzrd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gzxdpohkd.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gvhvfeugp.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gefqdibto.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/grmahovqr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gkwnhlqij.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gercexqol.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gftudzeph.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gjfgjmidg.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/ggnhhaapr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gpajrvdyv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gfrcmoeuo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gjxyijvyt.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gumqgvlzj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gkbswbzue.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gqoqyfwis.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gwdwcmfgq.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/ggaoyoobp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gpnrepslr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/genhyfiqz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gnmlorlsc.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gqsrnimgj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/giqsdkzdg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gpdwgdgcb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gyaurmlzp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/grynsimol.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gyiujhrxa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gldtueqal.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gqaqrtddi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gbjmwbfiz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/ggtsqblwl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gvxjdqltc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gwzrdutos.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gwruvcnpp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gtgfhepuo.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gefrbvewv.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gshyurfbk.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/giupkznae.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gkzrrcycb.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gjcawvdny.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gfpacwzbs.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gxnfmihjc.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gpfxrwelf.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gcjoxspzr.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gweikikou.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/goqvtiqfx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gjtwnqtsz.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gaooayrze.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gygsbuoqe.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gqovjxpaw.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gxsiivaml.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/glxtkmyrr.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/goiwckmgg.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gysadtnrw.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/ghijgnjwv.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gekzkrcnh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gzeiflzva.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gnwatuoom.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gzifzftix.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gcnubwxbq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gasginfit.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gnwjuqtom.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gaauuxknz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/ghxaryhcl.sHtML


<!-- 参考信息 -->