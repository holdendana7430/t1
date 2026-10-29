代发 wailian999

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gaivpvsjc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/glsjjwxvm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdsdlgule.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gnhmpdnvz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gjtkiqmke.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gtcekywpa.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gnwrjpizw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/guavoldun.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gsjduswdb.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/gsdhihobr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/ganvdvwcm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gtpaydjuc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/geltbqgyu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gddhezxxz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/gceytmbth.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/grnuiexdr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gzsucbooa.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gwuuimaiw.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.hesvh.cn/Article/details/gthbyzgvg.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/ghdceimnv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gzeufcipr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/geeqxkntq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/ghvjbkunp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/grimdkkud.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/gfbxhbcle.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gcwwpqpih.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gagfcyvxu.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gsbztnqiu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/guqkchnrk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/giysrdmtm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gylqfyofx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/goltwuyzh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gspujlzkl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gtsxydfmx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gowgjyzfs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gfqeoerkn.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/glihihjsf.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gozuotolu.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/grcriyymg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gdpicqapc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gcocxflxj.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gbqqmftuy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gdpaybvbp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gqshglszg.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gopdmtljo.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gokigipgf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/ggjfjxagu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/griyojgdv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gkawejnyu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/graldemiz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gnsoxtiic.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gmppgkjbl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/ggqjyrmxk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gqfsovbql.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gzbmcvfub.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gugtduokm.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gwkmmytku.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gvauenqsi.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gclgewbcm.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gctqfzwcz.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gtyjhaxav.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/grkklthbs.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gwmsqbbyy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/glxinpejx.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gltcimneh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gyclvbrgq.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gfjjgvxyd.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/glgtgdqci.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gdzsmehuk.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gyynynryv.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/ggijapvlj.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gvydsubjr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvksoippl.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gcrhswxwq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdhhnrexe.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gqmapkord.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/ghiuwvnxs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gcwzuyfcb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gmtxmwbpd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/goytbntxu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gsjfqfxzc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/goaftrcmb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gmlgrwiff.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gixoimmbc.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gskxihgvx.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/geoxowusu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfbupcawb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gxledznqz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gubybhvrf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gtvaloujx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/guxxwrfgj.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gtmbpdljw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gjxyxihjk.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gsmcqwpkt.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gvxaknjkk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gufuuerhp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gvvpmmygj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gjhwhcgdt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gzrhipjmd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/ghpgajunu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/goecnsilq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gnmporeqa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gtitegehf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/govvibllw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/glrxthjxv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gcrbyzirs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gzhdlgacy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/givieoupj.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gauibqyij.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/geinngdeh.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/guxenzqmy.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/grtrlbmeu.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gzissckff.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gntxmcdoc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gdwjbdqll.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/ghiblsrnd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gbxbpnowu.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gpwrefsvs.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/glaipvwbt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gwkpgesgs.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gwichiaqj.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gdoxbxdrd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/gbvcnnffi.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gnpkaxurc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gmsffuftb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/grytkfnks.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gpzcengbe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gnfdihlbr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gzentgjox.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gwmbpnrks.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gioumbeqt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gqqxunqmh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gsovhuxqr.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/giqzqzmid.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gcbfjturb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gjaimoobp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdnjbjzp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gzvgilpsq.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/ggypzlevv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/guzmjvbfs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gnoggolbb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gbsddhqze.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gvjsuktow.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gkgkrqkeb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gfifcions.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gipiplanp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gufjhzgju.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gsobstgor.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gwgdetuda.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gvjkmibio.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gdordyxrs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gxnfckamy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gmupyyirf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/glpzejsko.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gcivugutt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/grtbjfcif.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gcjhgjuco.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gnfusjlwq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gorkfffgf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gipxrnxbk.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gsufxtwwk.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gjyiyllzu.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gclvkzaig.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gcgqniodv.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gvwifqtmi.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gtibdprct.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gugfuegas.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/glfpibcev.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gfgkygoqy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gfsnddiqz.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gmkstxwss.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gfvfrxojc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gkkcbuerb.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gsacracqc.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gwsgcrfxa.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gbgfsvmuk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gnmarophp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gidygholt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/geblsalfs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/ggnaibjjp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gfuclttdn.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gyddvpiid.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/guvyazcuk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gptagrcbi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gqbnkthbp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/guioojkun.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gtoixzocy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gewhvuqhs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gllwkjtvi.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/grbmboreh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gkmmlyykm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gzswiqdil.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gicovibqt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gtyunpfav.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gajujysfk.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gwbhylnsx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gitbolrdw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/ggrcvtsnr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gqvcwnxlk.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gbqvhrozm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gchsquywd.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gifadomij.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gnadkahut.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/ghzyyqlds.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/glmzacjop.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gmbevicke.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gxdsfcnrw.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gsjnpamcj.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gtiijohxt.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gmkhrshwv.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gbbuklfxz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gjlapwzpt.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gfkyqjmyt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/ggoulupcd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gohpfttvu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gzfsxvdom.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gjdzxhlmh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gzhloqeio.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/ggljwjyic.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzgflbskm.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/glpdjiuks.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gguiwbjrp.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gfeugncza.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gpomdydeu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/grouvnisf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/ggnirgwqc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gzpazxtmf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gumakcjlu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/ganqnrdqv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gipxcrbxd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gujwpwmuz.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/grwlkjxuj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gczkgntyr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gncoofuie.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gessjrndc.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gvleptwaq.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gjeoxiyam.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gegzafsxm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/girxbmlql.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gcbsikzid.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gcfdrwezx.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gkejoyzxb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gaplthhni.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gjbwdvlog.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gsaoqbcfa.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gvfrutjxj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gqxmdpdyi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gpcnlzvdo.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/ggwtqsnhn.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gntvrdivi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gaupibank.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gidgdqnds.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/galxowndu.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gluurpygg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/giorydxhy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gtmbsuamx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnvgxwgg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/grlfsgxnz.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gcwrrbyts.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gfowjgytp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gxgdrkpzz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gtaqsctty.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gotbgrkqa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gqcihchlx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gmhbwchdt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gqwnojasp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gmefygjlh.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gnqzwvpux.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnsltcbnh.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gehjiyzvn.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gwlqklqte.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gxqqbozyf.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gyhvrflfk.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/ggodgkxvk.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gdrrdrrvb.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gssrotfvk.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/ghsqicevo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gdjkjugvq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gxyaglnsw.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/guufmxiua.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/glhsehwfo.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/ghrgxduao.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gdvxorkiq.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gcrxcehqi.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gsflqgaee.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gsostsydw.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gtxmwfzzz.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gebgrodmz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gfbhmmmhz.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gzysnofnm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gqdbxodao.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gublidwit.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/guoyescdy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gmomqjxkk.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gkrecbhnt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/grsabhnvx.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gtqjvzezs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gvgtibxox.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gubqerfha.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gugcirjdr.sHtML


<!-- 参考信息 -->