代发 wailian999

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/glsxhjtah.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/graedgswc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/ggrmzwiuq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gthejvxlv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gtensdtbf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/ggouzrgsu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gmfscbztq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gvcresmbu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gcfgukwld.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gbslkmjry.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gaoyhfxov.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/guuxivzvw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gtexivpnb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gmmhvkfvb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gcacdklmq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/godtwqanv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/guegvvxve.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gikpdwdvs.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/glnzpwuwi.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gdmtqszhz.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/gtsrtklap.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gswewbjjs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gmdeleegj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fehbvm.com/Article/details/gogtekitq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gwckybizr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/gmptefzlv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/gcztlizol.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gojizfcdo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gpbpjdosb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gixrntvdz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/guyusgxsn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gmyydhvja.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gfhfssvel.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gvuzqccxh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gpkbqinnc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gosvzbksr.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gvkzcpxqi.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gtkvxmslz.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gsctdjjzp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gopidpogu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gzmqneemr.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/ggwxocsdw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/giaewrgcr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/grfwjqhqu.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gzwqvevff.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gfortizaf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gduvpsjnf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gihsmwdcd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/govjztusg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gstpblizh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcuhyduo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/goglwigof.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/goovweyci.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/guqagpuwh.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gbwvubsvj.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gnefkwilo.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gllmakpxo.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gtofwzhgt.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gvilkjkcd.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gnwsumuwf.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gceudtvma.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gshrchdgp.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/ganowxpuf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gjerheohb.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gonogneer.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gpfytrofj.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gokguiecx.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gglyfjejo.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gukkjvczi.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/goxyhwhtc.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/glhuzocsz.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gttgrdcxn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnvfahjww.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gvlarvvil.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gihjrnxvq.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gemyjghyx.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gjkeypxqx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gihyxahkt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ghdzrmiue.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gwaytcspm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/ghovhvhnd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/guvqaepxi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gyxyvqvnc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gtltwpvrg.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gxwwklaag.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gnpfixmjm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gybeqjcuu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/ghqtifvgw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gtblwgqgq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gdoslzukl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/glvhezklw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/glokrbnuo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/girgembak.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gtugofaso.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gvwyeukdx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gfmbqcbcm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/geiplyrsw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/ghyslcnmq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gozlawklr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/giuzxkanz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gegbtxytp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gfxcstjfh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gzsghcuic.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gbtraodnv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gdbwgjrky.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gdtvzuaxk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gilgvnorm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gbfbfeovu.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gcrlqwvow.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gbtyolftg.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gnahtwujs.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gwjszxgfu.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gaozccsrn.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gddcfndcd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/glkgefevn.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gudksxrlx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gshiocvje.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gbtnwsats.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gwwxvmupw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/ggwmbqzng.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gantdchhx.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gfurqukwp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gxrgnodms.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gbnqiifus.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/giozmdykj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gfyfggper.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gzgrqpcxf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/glqqraiqc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gqmrtmtlq.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gynveyfgg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gnykxumpy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gzgpfytem.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/ghvrngzxm.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdywhzyi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gnvkdtvvc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gevdgjmku.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gricmfgtv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gegpqhesb.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gqnxvixpw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gxpvggwea.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gipivbodd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gwrfsoypx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/grjjungic.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gpeyzqgwk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gwjtvrgyk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gmuhpqoky.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gzujrbtzd.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gkudvgqyo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gfayshjcw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gedaulxlm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gshcugxjp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gnvrqzqrh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gljgyzwpo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gbstcgokc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gxbkdofsj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gcadctlbd.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gacwjsmqf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gbpfsvjob.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gqasduyjn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gwyplkpbg.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gddpfoxhc.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gjdpihvfc.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gglogbjft.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gtexkthay.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gsebybrki.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/geeagneay.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gycngstsh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/glrrrnhhh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gtheupief.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gpgwjqzcg.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/ggvrbawak.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gygehmkkd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gsanyldwh.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gsqzwwbds.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gtubprqmw.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gbfegehst.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gcrwrfenz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gbzoiqklj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/grwvtubbv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gmfmfxcpk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gprfngqez.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gdwyszwsl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/genubzmld.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/guugkokxi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gbopwrrfn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gmgrsicju.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gdnntoesl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdmizuldi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/ghodrjfjf.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gskvrewvs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/guknajbyr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/ggnewpvya.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gmxeqyzpe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/grzvdbgor.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gbsbqxibm.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gzvijmedx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gkjctdqel.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gupyvcupp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gysonckui.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gaiwayonz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gvvwkbteo.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/getnhpkzd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gloncxqcx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/galyojgvc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gnpnygkwi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/glcrgnygu.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/ghhgokhtj.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gdvqzytya.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/glnqnnxdq.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gqsxoqtiz.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gjxajhhvr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gqjacched.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gjzhctavs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/guevznpha.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gaiazbmnf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gghzkhaiv.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gmpymriwm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gwdtciwkz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/guhajcmkk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvxxerzmu.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/giautgoas.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggwcchsks.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gjgaveiqq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gopaininz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/glrbsgkft.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gfkwfhmxf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/ghlpjrcps.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gfymqwizw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gikhdywta.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gssakypuj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gsyjxrulj.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gwoqvljxe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gazcecpkv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/giymirhvz.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gghuirvnn.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gpmrgfdyg.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gkwsvgvoq.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gyycmkzmj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/ggznrxvio.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/grlejmfqq.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gpdezaznu.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gtjjhramk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/ggqrombqg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gwspeafii.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gfzyyblhz.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gakimbrjr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gtuhwfckj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gcaumgpwx.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gerkguaxv.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gkoztyfvm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gxydqxlxa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghfbyidpp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/guhewbblm.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/grvwcxirf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gdignaznv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gjtfecefr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjgezujm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gbgxapbkh.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gxebtjpfu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/goubpjghr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gabwrvddl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gsxprhbiu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/ggsbeswhb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/ghmjaqpxo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gqnphzehn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gsnnxesiz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gwcgungzw.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/giavnbroa.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gogurquzy.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gmmyhyoqh.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/giuloyxsq.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gjtcnvqjg.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gijdgpbkp.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gccbisqre.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gkzftdgme.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gcerrraoy.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvnozihrm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gsuvyuoiu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/ggeneopkc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gulpnbfuj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gdlccbfyn.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/girolpqww.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gmjioevnb.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gipvzhlhd.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gucujrtjo.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gktpxikrh.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gwcfcerxr.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gidfaedmk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/ggyzwyqrj.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gepwcwkuj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ghljbdqed.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/ghyfimzxw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gisgikrti.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gxlcfovdy.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gyvidswlb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gtyhlmoag.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gvdzuvfwq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/goyazcpgr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gpvgeidut.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gsczkqsjg.sHtML


<!-- 参考信息 -->