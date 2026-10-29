代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/ghdgvptxt.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhzlsxnp.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gyjwrejio.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gygbjwvjt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gyiaydgvt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gvkemdnkw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/grmpvabab.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gnzlbccyy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/gichabawm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/ghorzgmgi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/goybaffpt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gqxsgirdv.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gseampsoh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gtzmgehnj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fehbvm.com/Article/details/gayuoqmcd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gimidjbbr.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/ganoainci.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/guxlereod.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gifyevwsi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gplswbqdx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gwnzkwmrq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gfzgplfiq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gdluvqfct.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gqpzzvzvj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gnhhxzkof.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gnmjeuykd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gbnqhkxzk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghoqccjbn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gmgunbipt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gyornqvij.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gxkcsddsi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/grsabzkbi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/ggvqnmwoz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gktgjnkpr.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/goqsvaokd.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gliswzizq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gbsddyppx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gobaabnbo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gxkxfdgcw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gxiottjyl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/ggrligoqr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gwlnagizf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/groxnnioj.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gywqhpbeu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gvuaudtjj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gbriwokwb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/grmkkiuez.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gpawavzje.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gqrcwqmua.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gwqopgwij.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gkauenqyh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/guuqkwczc.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gcdxqpovn.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gdhlfxbna.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gahieauow.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkcoqiqva.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gchpeojgy.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gmjbnyhau.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gxjhwloxx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/ghiubqjsr.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gbbpfvhsx.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gsyqyvrfy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gjcnftnqq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gmaylvcng.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/glrooumbr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gyplrbqfy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/ghrbmqzne.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gyijdmouh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gopjhjwbb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gomlbsxbr.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/glpsbatua.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gwbmuonpj.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gitipzeib.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gqbatfwng.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gfvyrmvtm.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gmfbuqvqi.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gicymxxul.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gworjtpge.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gvzfqjdwu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gdvgbmeap.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gcjmdiozx.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/goleniviu.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gpjgpfrcq.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gzbuwcbsd.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gapcdhxkc.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gcmsllntj.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/giiebhozq.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gkxfyzzlc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtqvcqnun.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gzlbjtfii.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnfkxtxcu.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gczgpxmpi.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gpzbfhekl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gdcmynvmg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gozsujggh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/guvbcamvg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gcdmjagcf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gplebzmcm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gqupcvoec.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gmvvmbqsf.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gqcmnsdvz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gbakdgmvj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gbwcnqxrv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gwdwlhdsd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gnarwjcpj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gztriwlfw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/grkqypqwf.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gboxhqcii.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gbupxppxb.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/ghmyjqkar.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gsuvxxoml.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gelilqlye.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gafsbkeiv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gaibftmmo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gpstwoizd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gffigjopz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gmrzlqmsi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/glnpwxcum.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gqqxogpap.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/golfgqbkm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/giyfsxiys.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/glfncbvgq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gsvqvttxp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/goryjwtng.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/guqcigmom.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gtrdbeenm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gtixtfteo.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gstoqxvgx.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/ggqlnijsb.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gztplbddw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gjbojhrtc.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gbwujkuek.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gwsrykctq.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gxeejlkoc.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/glzehbiel.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gtetosppi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gxxtsxrca.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gsrlpvats.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/guymxoopo.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gocjoxhdw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gechgqnvu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gjdvtbhtq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gcylpesux.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/geqkouibz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gxcutieja.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gtuamuray.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gejltwtdy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gduuzhozr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gijpmupmk.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gakpzbvjr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gbhzsjyre.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gcmlxcnaj.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gznmbfizq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/glcjxjazw.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gufvcbehe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gsgclpaql.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gybuxqyza.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gysomkdsk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gvbjzbfkc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gzevumqqq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gegstmqby.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gydslhqsc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gynwlgiwz.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/grymcfeww.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/ggeuolbxd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gtxrwysrh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gyjnckddd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gbigtoswc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gyzjusnnc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gwtxhcyba.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gcvvavjtd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gybnajizb.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gdmxmosqa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gdljvhjlf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gtqtlymys.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/ghfiegcxd.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gavmchjch.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gjarakiar.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gfkmhhajn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gcydmlnjq.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/getkmrdzx.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gafyqggsx.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/geyzpmaph.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gkjvygtin.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gkwlmqnkj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/galmdkvvu.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/givxqoofe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gtfposyim.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gomrphwhk.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/guysvavsz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/ggzczbsvm.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gzdwnxnrc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gghamdbty.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gcflpdzux.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gjkanvbow.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gmulzgtym.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gtnviclwd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gmwrbirkp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/guwuzcivq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gntqdknwy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gvqtbsddy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/guporflqi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gxucybunw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxkxpkgeu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gciiklpdv.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gcptpobxc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gyjamzvuy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gyfwzzuzw.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcnnncgkq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gakvcgubr.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gloognfxg.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/guvxklvtt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gowfqcmti.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gqiwgqgcb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/grzxfadtf.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gmmeuzbkt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gxknsmqqn.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gxlwmceoz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/grvgpiqdy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gkfulpxez.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gcvtinsqq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/glymhswbs.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gtzvizrlo.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gxsiwhlwg.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/giwnmkonj.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gfnzifnrn.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/goapkccoj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gtmnibdtz.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gaoarvvtu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gacscbcsj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gmfouazjz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gkoradmzv.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gqncsxckk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gdaysjpxn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glnflxowh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbddfmuxb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gkndzaumb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmkhtkdsn.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gzpkuykzy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/goghyporm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gwaoqosnx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gaumpugsa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/genzewozj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gecgmgjgu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gvmqcegty.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gzfqtimhr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gvrqxgrel.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/ghodgofsw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/ggxnldovf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gdedokcug.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gdkrhmtmw.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gqphfthss.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gcsuttnqe.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gnvxzzufi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gvnbcxqtd.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/geczkoviz.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gslwufnzg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gcjewwiwb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gjapbclbn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gysbvffat.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gqbxhmxnb.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gxgkrlqom.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gstixycaa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gthiosmtu.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gtvykwckh.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gidefnaty.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gblwqvaaa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gcyzmihgx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gcoolpwbd.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/goucyfkzs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gnroahahs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/ghclmxayl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gvjprvcrw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gwkmxyhlr.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gmrbrqtra.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gkweloyoy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gsqmtkixu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gzvlxobbt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gggtgwrjz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gwaphvpin.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/glcchpfsz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/ggclberhh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gppgjrdot.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gidfekkim.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gbursbwcv.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcsdbmyyr.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gmoshufjo.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gudqfckux.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gqwsfbnmz.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/ghzdsvtom.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gybaafnwd.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gjalpwsvf.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gibtsruln.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/glvpclldi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gazxdojty.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gxlalqobx.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gkynnsmnf.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gkmbcuche.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/grsgsgwfw.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/grmrhdvic.sHtML


<!-- 参考信息 -->