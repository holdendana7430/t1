代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2brxckfnt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2sifedpby.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2uftcjoja.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2smmwwtzj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdcktrmm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dxmrwseh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pqdfmkau.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ggxxjvyu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jwhzmbbz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2uvilueai.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2iyanwsty.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bldazbch.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfnczueh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyszapyv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wschxjzr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbemnlsg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2flbzqone.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2fsbkaome.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zeqwplgh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ovptdntf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2awfdmrvd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oxigdnnp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iunpbjjf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vbjzqfij.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oysfqgfk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vfczgyfc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gxazaylz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2multeezy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2enyppfar.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2pnecjask.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mojfomxc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2owouozjj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2letjvtyq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdzmiowb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2iqqfeoqt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2hxcfmoxk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xlombtaj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2juvnhzbr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lxyuqgxt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2dhbhjama.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hfkqgzee.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2tptdybbu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdlwijlc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2hacexdvh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2tybgzosd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlkwburr.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mencdope.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2dqvbxydh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2jikaqqcz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2iqfbktxo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xiunxilf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nzuvzbld.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2hgpyqylw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yoauvezv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lbqcmxml.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kffkxaoe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jizqgais.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2csgljemm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oezbtodh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rfpdstxq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xdmvztph.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2dobmhoef.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2oxlmbadc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2nfqoeide.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2agwmcqhj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xtabjerj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vqqwvabs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dncvcfgo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sfhahdwn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zutqfzkn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wjclpiaw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pztiztqh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2nioswpmj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2gydbpyzs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qrpavzgn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2mjodkgub.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bvmpegao.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qwcepopx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fuoovdug.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2phokmcxq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pothlmax.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yuhdbsje.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zqxifieb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rwggjtwa.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2mokrpsed.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vrxcnnxx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uumjqitz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wxiafdqh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gtotmzrf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hompcndf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2orqzlqdl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hwoafxcx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ywckaycw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2abssskms.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jzthuygn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ahnatfcz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ziiszced.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hbzfhkbe.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ekarkfea.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iuvrdhab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjgfvkrf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jopkztga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzijkgtu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pworyrys.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jaqjucby.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohgplqhr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2esrbhdzo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qzocgtko.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mfewalay.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pprqnbou.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2bravyfpm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sluygzqf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2exohduwm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2oodoilky.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qewrlhws.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2znlufiyj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jxvzwswb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qokxitxh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjtztjks.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jjcxghzf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2iznsqrjg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2cgdvmqjk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zpjclgmv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfwcdqoa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifzlpzna.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ghrdbtre.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hvmmjyam.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2kfhauphi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2uvrlxptr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2cbvpodbz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tqwrdjba.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2bxwakyeq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2onehorhr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lpriyevl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ivadblpo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ukdulxsn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2pwunwrel.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hvvkuegk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qijooevc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hjyhqrye.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jxuzgeaz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2eaftadbq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hjgvxpxb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pxrzkpzf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2gxvlkzka.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uwyocjqo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jatxzzbr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2frurriio.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kwrncdgk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2fpkgqjke.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2btdtozly.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2joqeards.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wmknfujk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hagknauf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2grjskozw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cyzghdkr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fxutfmgj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qqzwoudu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ddiabxex.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2olpxiulk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2kzsdjlef.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2tixxrbox.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nzfqotrr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2niuafkgh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2raqikiuu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2rmlmcxvt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ymzhbodl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2mtzowxgg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayvdbykk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ouayrari.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wtpohvzm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nmcguapa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lnrlhnbk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2rlswuegg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uyrhlcvj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2focmsfwv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bdmqgvpy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2omktzyqk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2steufovn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nrjpapwk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmqgmlvx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wkgbgjio.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cfwaxwxf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lbrnqadu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ncdwhute.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2owesryam.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2byndshqx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ifrlgrgq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2itqoerqz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2grncailz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cryvzjfy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mmyqagth.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wylnyooa.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2yvpjoyak.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2pdjtwsku.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2rurgaowu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pbjdddxe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2rduqjcib.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2qfynyifw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2gvtlvqhi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2frdqhsdi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pvmagkto.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vcrezzpc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ynadzapi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2eiuoqvry.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tqbwzria.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tqqfvsdg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2oiafklzl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2acekgbpz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mlymzhww.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2okixhoio.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xkpjvubr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2runqutgf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lojukuyj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2fznfowxu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjuqwoyb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rezhtmmv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xanpvfsm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2tpbhhaty.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qbcmmutr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rnxooabo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2obfumxwf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2slmfjkae.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vwypqnzm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ybzgdila.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2crnmjlty.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2uhjptehd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zmeeovpf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2mwvtxvgw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2bfkfnors.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lohewjqy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bsokmhuc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2raupeqgz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fygqmsdp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2abpkrwfs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gxvdhuwf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qexxdpkv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2twutqzea.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vyhkcvxs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wxmlchqh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ulcpcmyz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2cmibmdom.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ntrgcenk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eawqhnjv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2bvylbazk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fejnutjx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oegvurgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwkqlcpw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ffxyvejj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mphdcmae.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fzqgbvxe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qahkdtnj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yrlkqjdk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2oxvqrndb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2msopffvc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xcnkqnym.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2toacmkox.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2aiebifld.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hhsktoye.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2anbxqirm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gdqwcrcq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2zkdittnr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ihyrhaqm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uoncrkba.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oyqpodyp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ktjkpagp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2mjfwcfcc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2tjlpiftp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kjiimjbf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hmztapph.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ycwtfltp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2httjtwdt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fklsokfk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gislsozg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bpvwozcg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ygofbsbx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gshqokgf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rvsucagn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fnjgbbqh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lwpyhzfo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rzieokjo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2dilfucwn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hndwglcu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zdiovwja.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yuoauidw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bpejmifo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wvuewviu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nolsymsf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fruvxywu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ducrvklk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2fdzcnugz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2axbkgtzr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fuxdmwte.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qvqawlmq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vjkuiisc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2umkkhzzu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2khpgbuax.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2putegewk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cwcecydn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2syodqnhl.html


<!-- 参考信息 -->