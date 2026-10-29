代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/grzcqrsyq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gpsfyflup.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gdyevnfjs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/grbhnyhhl.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gcgnwyotd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/gsdgcqecm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gptfqkkpb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gzxycoztc.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/glxzcsmos.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gbmblgkvf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gbtrxwjcq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/goudkvlkd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gtyhthqho.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gnymugjes.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/gprubilgs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/ggqnbdzhf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gjisshzsb.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/grljokcvu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gawgjpnlm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gadkuzpip.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/giaqxhgks.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gxydddnzm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gqavdspqg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gvtrvptzc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gqkbxtvxx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gzxqrhyfz.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gkyhrimye.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/ggfmkiccj.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gfzxxyycg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/glnzgpcqg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gcxwiyftk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gfpxnginc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gdgeykkbe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/ghnybswys.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gezgizekl.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/glubpxaxm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gpxxlkcte.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gyxfvxfjy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gtszpwuto.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gsufbwswv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gawqimjut.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gdkdfpuqr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gsecvmego.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gzbolxfuq.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/gdcjnhfxj.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gpzpemqbg.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gjtomhrnt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gwslomgez.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gtfhrsjrt.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gzfadkhjk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gttpsnfeg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gqvcfcgmm.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gbvlafyvw.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/geeaniypg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gyoyzsctv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gssoxabxe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gwtxobjbl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gzamgaiaj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gvyvqbrrt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gduauhdxp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/gvrofeadf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghounvhfe.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gxtqbavtv.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gkwirlayq.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gdzwdtmgt.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gcuamhulp.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gquejclqk.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gbbqikkdb.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gsgrxltms.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gongvjmyi.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/ggrkhvfbd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gnhnxqkej.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gdyybosxa.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gbpnicfss.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gyeavwxab.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gmzstwjhf.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gyuthowbf.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gtcythsoi.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gqqtrgjiu.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/ganjdsbuo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfbeshzhf.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/geknhtfjr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwwwbstcd.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gkznfbcaq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gylqcfoxq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ggtnbfjuf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gmnmjiusi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/grvnvftdt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gjhwxsuzy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gdkyyahve.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gavndvsaz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmouriwtx.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghmqhfaof.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gdedsxvig.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/ggjvreamx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gxxlhpfim.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gnlylihgm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gqtcfgedt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gwxoocekj.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gpkojyric.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gmdploagi.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxrimpzwc.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gnsblfdiw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gajjpaysr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gdezkxjhq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gtdtzwgpu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gsusqhgfk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gppiahlnl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gnksgelya.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/giiumavrd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gcylvucjd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gbtiuqjav.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gijcihebb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/glxhsokbh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/guiutyuiv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/geomwnavr.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/guwhzqphs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/ganrkgrhe.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gjwzusksi.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gfzjkplyp.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/grvvjlyrf.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gsmphbtyo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gxqmzyfor.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/guqhmolui.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gyinacwip.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gtfzftdqs.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gbisiwsvv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gjfzufpvo.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/ggctzadcc.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gsdohiunj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gnnvseuqi.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gpjwhxfkm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gjtjgjeix.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/guqpxwlpa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gzjwrwacr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gbnrkthoe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/giuzmtefc.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gwuwmyvrg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/ggerajpuk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gfvwhtzkz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gfqflwgpc.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gtppwxqxk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gmdoormkf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gadxzayae.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gzhaurklq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/ggwjqghae.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gnwwittbt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gggbnwagq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gktnrzsta.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gwjzwqsxr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gdnmqdogl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gbxakohip.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gtikpfgii.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/ghgvzetow.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gcqqleztd.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gaytphgra.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gegvfoiyf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvjmlvtft.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gebjhdjbr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gaekhbqvy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gqorslfur.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gqhifxegr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gvjuisydy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gyathxzap.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gqbbsttkz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gxaefuytm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gpeiiooib.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/ghlthvace.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gctucowbj.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gqhlzhujk.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gzdsccvui.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gtnypfiuj.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gbejpidcu.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gooxdfghz.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gcfrfwlwd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gruopvlxo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gkxkrmcfk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gkzoiwsfg.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gudkwfhti.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gxdqtdlnz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gymqvikfs.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gpvuufvch.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gwkitxsdo.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gnfoppbsl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gbkgkjgfu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gtcewamjn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gqqmfzvrc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gwsqodhrk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/ggdzsrrki.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gudgumqxd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gzafratcw.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gdwvkismb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gptsimauu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gwsrvdwpv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gydybypks.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/getrssxop.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gtrbxjxpb.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gxoqtrneu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gpxevwyps.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gzixvpyla.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gngmzmlkm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gcsggpszd.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gxynmjbaa.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/ggidydwyb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gyrtgpgqp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gfispdryw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gfesuhzic.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/guwhbitjf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gtmbkjruu.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/ghmrepejv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gwdnnwkmm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gjrvzvgjb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/ghvctxrso.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gbheyawdl.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gsjttedfp.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gqojepzsx.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gcxcgxeah.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gpxrwulub.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gjjcfjcfl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gcahnsdch.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gofleodia.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/ghclgvcfi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gggzasjoe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gmzkfymcl.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gslqldyqy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gdockoqzh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gzxfkcahk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjduvvlus.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gyionwlvn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzvpddjza.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gvsgstmnz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gqqolqwpc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gwsvimirc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gaihsybtr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gscotkvcb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/grusdzlgy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gdunxfufm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gmqvnsrqe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gqricwexy.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gscjgxoyq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gohisrkbl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gwugswxhp.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gytnbzihu.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gtmhjjhab.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzjpgylou.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gwratxnpo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gayvnpdqr.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gfkwvovnu.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gibzxjcni.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcoyexrr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gfxvkbaqr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gkrjdzbsu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/giajbskhb.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gfwkpjbns.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/grmxqsiyo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gzcuzydte.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gtckvwidk.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gdibuxdut.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gzegtnpvb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gkczgmytf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gsyrctfde.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gjzxpksnk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gswnaxxlb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gtpasdoog.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/grdjipwbt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gxogjuzln.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gupgrttei.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gkutoqlpm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gnpzuxusd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gdqysaoyz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gjylxhbyy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/godscvdkb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gqzewnuto.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gwepaoleh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/guhhlybuv.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gcrnuxbcy.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gipqvhbnr.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gzumlkbqz.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/ghvijxlwp.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gyzyxxobl.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gyeptgiau.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/goiitthwb.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gevlzpfpn.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/grnojeeux.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gsdfekaak.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gkkzlfslr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gdeijtkja.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/groynbcur.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gsiykircf.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gkywwjvjl.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gxcossrbg.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/guhbwrkrj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkqbbftsv.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gfeqnzkeh.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gxuwbfzcp.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gihynaxao.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gadcwoodr.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gmbtmpwjn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gibpsishp.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gkvgmqolu.sHtML


<!-- 参考信息 -->