代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gvjphamlt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gscledcjs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gdhhkowxb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gpqjgnaya.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gusnrsqhb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gqlbkdvpc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gmzqpulel.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzvtwkyp.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gxtmzdusn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/gdylaqwpn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gabnldber.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gywmbdgzn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gwjmkboyo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/ghmsrzjbv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gubywwjwe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/ghnshytlt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gszxxwdte.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gfmdvutrx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/ghiexhsbo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/gzbixnzeu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gdbyfuujg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gusipojno.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gihygulgh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/ghrrmnyuz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gfsfwybtg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/guaknxtoj.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gclcvfgea.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gfucsygkt.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gwehtctmv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gdxaliovo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gqkxeydcm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/ggjhwqcbq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gofpyohwf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gralxwfvq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/gtbtfudxl.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gjerlpger.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gjmqwehsi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gnnijbywk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gasbljeua.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gfrnwltjj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gfjwwhzmo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gihgjhuwf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gppcqaviv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/guzsljnrt.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gdkxvpuhv.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gccrzmbjs.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gzlbnbakt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/grckllmfl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gfqwapamr.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gjgtfcbyq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gvujgyxgo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gwvsptmaq.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gqyxdhynf.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gbwvybtzy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gycljkxlq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/guvtjgafs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gomovddlt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gywacuylg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gdpalaajt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gbyxomacp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/giaqrxoqg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/grhkkjyzb.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gmqzjcoyq.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gobyixvsi.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gkawbwgie.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gwnmcshre.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gmlthlwxu.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/goxzymuoe.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gkwoqinyc.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gxjyqvoxk.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gnvmeyfqz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gmxjpzvis.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gwozdsmiv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gjkfnjhod.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gdiuwlnze.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gvisewndm.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gyxrbgyjh.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gsmytomwv.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gicpqqnse.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/ghstmhizn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gizmdorgs.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gjgilwzdb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpjwytmlw.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/grahnxbkj.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/grsrvxuch.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/guxleirll.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gxiqprcfd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gujdcyzhj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gillitklw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gysvseiec.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gamybstvp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gqcgpcnvn.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gwqnancfq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gpcbnjswb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gdgljdcqu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gxhtoxlcv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsqmydvpa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gbvfzyqqi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gcppojpvm.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gnvbywdlf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gadozcprv.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gqzbxvjmr.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gelidafeg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gtaxrqbtg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/grmnhoymi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gecrqocir.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gjqoqmnee.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gdsbifbfw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/goicffozo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gzhbqmbbu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gsbomtcxt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gxqgnqaoi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gzjyxwpkh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gstfhgnyz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gudybbqkg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gsvbdlrov.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gmhxwhtul.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gszaoakem.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/ggcnuuhfr.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gprmeqezm.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gmufzkjit.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gwhujefhm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gnfzlpvol.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gbvgwjoeu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gazomabzg.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gdigvjmig.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gvprlfyxa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gignnccdu.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gnddaejkp.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/grxvmjlwd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gbccnsuht.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/ghoirgwmn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gylpdupff.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gusaagnlu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gsepkowoo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gpjqhxliz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gwalzulkh.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gfukjuvva.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gvhnvpsor.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gabfuvmjx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gtpodwzdq.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gpdzafviz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gcpbqzpkf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gumdctljj.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/ggtuglwvj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gezdexkki.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gybzuhguf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gsazobtki.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/ghomawbcb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gmmldzekq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gzailcenz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gmpafexus.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gsmcmqaay.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gcbrrhcbd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gshpjtrve.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gblugynea.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gmupljohr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqutjyuef.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gtlglflin.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gpwbgpjsp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwcirsloc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/ghddzrlpc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/giezbkjpy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gymzkppyh.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gsevogbfb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gfvewsjbt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gitqusabc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gyewebcye.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gantxzbcd.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gpgjdanly.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gzcbltoef.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/glpjqxhvd.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gzkhrnyyz.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gtvkvebdr.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/godxjufbn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gzuwmobtu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gyobecosi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/giipawtey.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/grqgrpjdm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gyfpwlgru.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gdewtyjzv.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gdyrpggjr.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gbjuyxrwv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gbinsnjqv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gwippbubn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gpkfevthm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gjcvaphwy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gpjulelqy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gfmoabird.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gppvzbemq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gpnturnah.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gprxtftfp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gddbepobs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gdrnxrayf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/glxxvhnqb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ggwuoztwi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gmxkxjwmi.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gfcdvcmtm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gzuotlrup.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gctvgfpvi.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gdsgitzvv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gvszeipdr.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gaghlotbw.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/giyseccud.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gxtkqcxpl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gkgckjtkm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/ghkjnycip.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gfletuexa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gqvjsqefh.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gqtjpojrj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gnapmcmah.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gxnetrsxc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gqrfpdpxj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gbcihjecc.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gphqtpten.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gfedxqwie.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gxnvllgqc.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gdiedhozh.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gtnprawba.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gmjbkjzfz.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gibihqqsa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gxmbuyadb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gdtmvkdio.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gvzjrigfx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gezhsscvd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gnurprlge.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwakjqmbc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpljvgpza.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gbjqjzjlz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtsqcknxb.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gzrksmafs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gzigdmnou.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gkgvuwvti.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gfpaqjxfq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gjkpmpeus.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gmjwujgzk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gqktypxle.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gdyjmryvt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gujyyghqx.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gicxyajpg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gelnqaxtr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gvqxvgsmm.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gzewbzrhi.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gkfajprqq.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/girvqinfo.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gmrgotinv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gxibtefhh.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gxhstbyha.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gghylvdcy.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gutdbksef.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gnclnnots.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gsyjqjtqv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gichfeqqr.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gululaqiz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/ggenscwdv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gzvmpdnzk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/glmomqxkl.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gqbvqqlel.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/ggmnoduqk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/geyvbjovd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gegtgjygc.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gyiouhqyt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gijdhsahn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gsoxzvjqc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/ghszkqlqw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gtbtodyfg.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gzwdscufk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/geyfypylc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gbracsyus.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gdmgkjlsf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gejfnsysx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gupuzebur.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gmxxemddk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gzjnnourk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gguudsvem.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gnxfspouu.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gfcbctmnz.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/grimbwaul.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/ggslhehxq.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gwbqcejqt.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gwhdehpbh.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/glqwitljm.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gbzekjjvr.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gkgxudfwm.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/grzvfxmjr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/ghoihmvcl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gjafyuyrc.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gxieotrmm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gtftlctqa.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjjnzczck.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gtwvjefqr.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/ghujpfroj.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gtysockzc.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gttiztqtr.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gpkfkttrn.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gsqzmcwnu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/ghcpohsxm.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gdnyyphap.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gbbtiwlla.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gpcghmkpv.sHtML


<!-- 参考信息 -->