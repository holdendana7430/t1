代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpynkvdc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fanxiaobao.xyz/Article/details/gyiwqwjxf.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaujxcjrj.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fanxiaobao.xyz/Article/details/gapuahdok.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdghvmlc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmifkacpq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxovvuep.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcsiqeoz.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gshfsmyfk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjacacgg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fanxiaobao.xyz/Article/details/glowewvfz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gtwrdybwg.sHtML

[B09] break 与 continue
来源：http://3g.fanxiaobao.xyz/Article/details/gtfwnxuda.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwxfwllq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gllivjmgv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcaqkxxk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuhbtabu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbrpysvxz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcjytxnu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fanxiaobao.xyz/Article/details/godajauhc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhnlbzvm.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrptylql.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqwpbsvy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjwhavcm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gjhtboeey.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgksgmmf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gipgjkfag.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnuujdvt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gemvcdzow.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gqssrdqrt.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fanxiaobao.xyz/Article/details/gpswqssen.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzqmyvya.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gxmtqcrro.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/glifgqrin.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/goboofjgp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gademkqpj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fanxiaobao.xyz/Article/details/ggmzrnrte.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gauhtdgdd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjauiwihc.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohkrieex.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwjynlcs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fanxiaobao.xyz/Article/details/giknqvybg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbvzbpqh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/ghmropylz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gcqpfmphe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbavjnre.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fanxiaobao.xyz/Article/details/gewyijsau.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fanxiaobao.xyz/Article/details/giknbwaqk.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gewcdxzcu.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fanxiaobao.xyz/Article/details/gknikihaw.sHtML

PHP:  is_numeric($x)
来源：http://3g.fanxiaobao.xyz/Article/details/gkypqgfnf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpvpsqse.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gasburxki.sHtML

Java: x instanceof Number
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdlwaehl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/gewcgglbs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fanxiaobao.xyz/Article/details/goydkijlz.sHtML

C#:   x is int or double or decimal
来源：http://3g.fanxiaobao.xyz/Article/details/ghqzjkniv.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpdhddlm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxvvkhsx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbznyuubf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/grghejuls.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gsvyikpst.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/ghkpavqbu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxtufsar.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjhiuadp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiiikiyi.sHtML

[B15] 布尔运算与取反
来源：http://baike.fanxiaobao.xyz/Article/details/gzhkpvgkr.sHtML

Py:   a and b or not c
来源：http://wap.fanxiaobao.xyz/Article/details/gftwqbunk.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fanxiaobao.xyz/Article/details/gdbonthrb.sHtML

JS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gftsitvmg.sHtML

TS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gulmdzbee.sHtML

Java: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gzpjmrqwe.sHtML

Go:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gkqqjflhb.sHtML

Ruby: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gnjfyabqt.sHtML

C#:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gdyfchkns.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gjdfhetam.sHtML

Py:   if not data: return
来源：http://mobile.fanxiaobao.xyz/Article/details/gclqfgduf.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbhyriifq.sHtML

JS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzscnhgu.sHtML

TS:   if (!data) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gjtkniavi.sHtML

Java: if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjamikjse.sHtML

Go:   if data == nil { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrovaybc.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guezexcnj.sHtML

C#:   if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnlcxcmv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbtrxyzxs.sHtML

C. 函数与作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gglharyfq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbglgalvf.sHtML

[C01] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpqeulbs.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsmjgwuz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojgtwhek.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glhlbmgot.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuqextsa.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfqvbfbj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznfwqtir.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfsipmzy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzbcgqre.sHtML

[C02] 默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbkqcywy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsiuyuiq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gflfcakfi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbhedfae.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/glsnnqmgw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fanxiaobao.xyz/Article/details/grkaxoexx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkinwpvda.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/girffncko.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghokdvzaw.sHtML

[C03] 可变参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghxkfgasn.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fanxiaobao.xyz/Article/details/gfziwvvpj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfubhfuzc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gfkdfaakc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmljwxcdi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlywbdeg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fanxiaobao.xyz/Article/details/gfjjwtxza.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fanxiaobao.xyz/Article/details/gcnxokjte.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fanxiaobao.xyz/Article/details/gmiculkth.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwojhbult.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfqaatwe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibfzkywx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzepnuab.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/gpsayhgfh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhxcrbeb.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fanxiaobao.xyz/Article/details/gqpofjutg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gabtzkrem.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtcxwyqm.sHtML

[C05] 返回多个值
来源：http://blog.fanxiaobao.xyz/Article/details/gxkcktsck.sHtML

Py:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/ghteyioom.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewtkfdji.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzceolmoa.sHtML

TS:   return { a, b };
来源：http://mobile.fanxiaobao.xyz/Article/details/gcywwckvy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fanxiaobao.xyz/Article/details/gttqyxrkw.sHtML

Go:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaylowmn.sHtML

Ruby: return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmemkroml.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fanxiaobao.xyz/Article/details/gdumlpepc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnfdshgo.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblzrfaaq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoudaeht.sHtML

JS:   const square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gatsclyyq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gbxmifvmn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvemxifsq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdfuccqe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcxzakdr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/geuqedpyc.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fanxiaobao.xyz/Article/details/gmhxiimqq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fanxiaobao.xyz/Article/details/gygprrjoz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/glgahfyqa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fanxiaobao.xyz/Article/details/ggqdxfhga.sHtML

TS:   arr.map(String)
来源：http://baike.fanxiaobao.xyz/Article/details/gsypznrte.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gumuufwcc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fanxiaobao.xyz/Article/details/grmpvtjjh.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/glgpxxglh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshowgrbk.sHtML

[C08] 闭包
来源：http://blog.fanxiaobao.xyz/Article/details/glsexctpj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fanxiaobao.xyz/Article/details/ghxpwefqw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkwpxvqmu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggcwwaza.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxfxlpgr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fanxiaobao.xyz/Article/details/gpkbpwbxw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzacjoci.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fanxiaobao.xyz/Article/details/gzwlwapvt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guucpbjhd.sHtML

[C09] 递归
来源：http://wap.fanxiaobao.xyz/Article/details/gkxrwvoqi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrbgyftn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guefhuldc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gtonxnpvg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/glzlxeoyr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvorlrjv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fanxiaobao.xyz/Article/details/geztmnrog.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gegdsefjk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gwbqdbyjj.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnmnjmxr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fanxiaobao.xyz/Article/details/gvwzbkpfr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fanxiaobao.xyz/Article/details/gekpygpyt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gipkyzgme.sHtML

TS:   同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gallwidbi.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbyicjhx.sHtML

Go:   花括号块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/grcahekbe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fanxiaobao.xyz/Article/details/goysodkbx.sHtML

C#:   块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzuicrpa.sHtML

[C11] 模块导入与导出
来源：http://www.share.fanxiaobao.xyz/Article/details/grlszxihl.sHtML

Py:   from module import func
来源：http://read.share.fanxiaobao.xyz/Article/details/gltlkzlqu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/gndmfxvys.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gdcvvultn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbvkfwmi.sHtML

Java: import java.util.List;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gophloelq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvctrtgis.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fanxiaobao.xyz/Article/details/gcncaakwa.sHtML

C#:   using System.Text;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyeyfmid.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fanxiaobao.xyz/Article/details/gquwgqwsb.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fanxiaobao.xyz/Article/details/gvbbowfzk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwprssjdw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfodzfxq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzgpbvlf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fanxiaobao.xyz/Article/details/gmpnmormx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fanxiaobao.xyz/Article/details/gqgkpxayj.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/gedyicxla.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaaedfai.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxjjggzo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/guydksgpj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gajxlemhj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbjxmfpp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvruwajmh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcqhxzwcf.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlgnxclp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fanxiaobao.xyz/Article/details/gpanslawp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fanxiaobao.xyz/Article/details/gnilnqoij.sHtML

[C14] 泛型函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmltzwyfb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqvgrrwj.sHtML

PHP:  // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gpnhuqdii.sHtML

JS:   // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gvbaqgsqn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqdvlrmrm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gptpsrrwq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gewkbbbpz.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geopyoyat.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtedozyz.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geivgrcas.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnzcatti.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugwpafuc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefkbqeja.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcemfart.sHtML

Java: // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/gkajmmqhm.sHtML

Go:   // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gjstzppim.sHtML

Ruby: a, b = pair
来源：http://blog.fanxiaobao.xyz/Article/details/gjkgjkext.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/glkdwgycy.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwlwgnqf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwumdhkgg.sHtML

PHP:  // 无重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwqxnysv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fanxiaobao.xyz/Article/details/gjdszmjnf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjfuwtnt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggmldwvlg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygziepuu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsurtanoz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gegtmhsar.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbfajwdi.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fanxiaobao.xyz/Article/details/grtxfueno.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkqwcjwgp.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gjhyrirrd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtcchckx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynijykmi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdjzqzir.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsmhnheg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fanxiaobao.xyz/Article/details/geydrqoqf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fanxiaobao.xyz/Article/details/gnekiiqov.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gybpuopor.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fanxiaobao.xyz/Article/details/gilfbcxnb.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdpbbcqs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fanxiaobao.xyz/Article/details/gjmyezmag.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gfldzbsyx.sHtML

JS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/glgpzooqa.sHtML

TS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfkoljjh.sHtML

Java: list.add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gwlvydzoo.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/ggcdkbymm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggykfpmwh.sHtML

C#:   list.Add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ggikuprak.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fanxiaobao.xyz/Article/details/gcsjhggya.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gxccczpqi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fanxiaobao.xyz/Article/details/gbwtsjvbc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fanxiaobao.xyz/Article/details/guhdhwpiy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdvawtla.sHtML

Java: list.add(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnjwnrkg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvftcvls.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fanxiaobao.xyz/Article/details/gsvhgxzgh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzljhwrd.sHtML

[D04] 删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcosforf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gzdecrjaw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvmenxqg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhxdhlcq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gnxqppsqb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlnhwanw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fanxiaobao.xyz/Article/details/gutwpsunm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/guxdkabks.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibrskzje.sHtML

[D05] 访问与修改元素
来源：http://wap.fanxiaobao.xyz/Article/details/gfsdroldn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhcvljjl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gdfszjhtn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxruinlfv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gviudioji.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsyvydhh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikeummfm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/ggjekqsnv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxbxowvs.sHtML

[D06] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwtduolw.sHtML

Py:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gsioxauef.sHtML

PHP:  count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gcvqdthgd.sHtML

JS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/grfujvzqa.sHtML

TS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gklcvvkdq.sHtML

Java: list.size();
来源：http://wap.fanxiaobao.xyz/Article/details/glzwvgnpd.sHtML

Go:   len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gjsfjfbji.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjlrnbrg.sHtML

C#:   list.Count;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdeeelhd.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gskuoacbi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fanxiaobao.xyz/Article/details/gavxqxtda.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcocbezzj.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gpriuudta.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmapkcje.sHtML

Java: list.subList(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gifwuilko.sHtML

Go:   arr[1:4]
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjyrmryf.sHtML

Ruby: arr[1, 3]
来源：http://3g.fanxiaobao.xyz/Article/details/gztomkrzk.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/glgsgfsnl.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gtordzkvz.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gwrtftbtj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gektuiqst.sHtML


<!-- 参考信息 -->