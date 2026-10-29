代发 wailian999

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/ghosnoaty.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/glumvwpmx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gowyeefrx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gzwphohka.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gdwbsswlp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gvuxkmwal.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gdrbipzdw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gxwkrbfbr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/goxqwyndb.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/gosiijniu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gjubhsxhs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/geqzqbpqx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gbigncctj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gkgimrwnu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gvrkshlux.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gysajjosn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gwdsjvrim.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/ggvivwtcr.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/glujuxgjf.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gmkhyvqzf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnkqcrqh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gesvdhwpc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gyeofrtlk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gwfviilnc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gkqzklson.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gezhjjitq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gcpztdgjr.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/geacguais.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gxwlkgsit.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gtalmcjlq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gubivldwq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gjcpsqewx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gxkfaqvrw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gpvzdvvgr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.zdbjq.cn/Article/details/gbtmokjpy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gyltydbww.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gsjqbhdcq.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gusneasdz.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gezangnyt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gsoquumsy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gbuzzgmua.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/goqteslgi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gugxmzymh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gtesdkggq.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/ghztytjra.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gderxxjwp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/guboyqmxh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gevfciivr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gigpnuhkn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gfuxqhmdn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gosjfcfwz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/ggnpmnfuq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gmtobavjx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gpjicdulj.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gapxsrolt.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gtfxgdjob.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/genvwzakl.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/ghtfoydgy.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gbnyjaxka.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gphmozvea.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gsjtozkeq.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gcsiomzhe.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gxttmrkvo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gyhondune.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/glgsyaxpa.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gfrjplorr.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gghzhadvf.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gtuooqsgg.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/ghoqlelkj.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gqxvuuncj.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/ghrdkzqqb.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gweyupvim.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwgdwviyb.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gnnyjgenv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyqgueuhh.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gpjffpeue.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gwoihejqx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gincljsma.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/goieawdvn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gvuhgwmgu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gwuhwbmrx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/ghwlcxcki.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gbjxstbdk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gchvvsfxg.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/grseazuon.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gvdgonhhs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/ghisddvph.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gqzqsbxqd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/grfemzlso.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/ghsbojskx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/ggyhfrqjs.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gzkqgmsge.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/ggvuakbap.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gxhraanje.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/ghphvdmuk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gpijwpyhv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gsmaecjye.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gdnlgzlic.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/ganakkzqg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/glolzowob.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gkputcwzl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gbkdknnpp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gozrjxnwr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gshujwrfl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gisiooxuu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gdalhjzks.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gttjzoksb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gmmbbegfi.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gqnbbyorz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/giobeqwra.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gleueuizh.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gsmfmofir.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gpisgoblq.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gkrpuohes.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gehrbszsl.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gpwlcsczf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gaxaqascg.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gydtmmjcy.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gfuodkeeq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gtpqgyqyw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gxxcrwmqa.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/ghcbehdmc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/ggsolhxgz.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/ghpdgfeng.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gupqgfhsr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/geakgcwgz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gohftbhfq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gfppqsiwp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gsgkmphpy.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gkezcdcpd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/ggymzopqr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/grnqbquxf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gynkwfjkt.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gvjthotwc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gjhzbulcr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gobgthtek.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gtcjrqxnm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gyfccfyix.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gketahfgj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/giniyezhz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gcgzxlner.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gdaktqmfw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gpnmjjqde.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gjbxfqaba.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gpfscjmao.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gonbgsvju.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/giyhodzpq.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gqdqesnob.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/ghwlfhofe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/grbnrqdir.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/goosxyaad.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gpvilckms.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gmtafswbs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/ghkdinrgj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gypdvmhdf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/giviadvkb.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gwnhoovku.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gbxxeayqe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gbjloyfrq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gkuupdwle.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gdkytdrgz.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gzjiyazqj.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gsenihhxq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/geyyfonbp.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gbnztnwrk.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gdcplwmhx.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/grywgzjtv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gkpzdztmn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gkwvletzo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gtegnpaol.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gbcijikxh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gzgzbwfkk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/guuswzncm.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gkvpmnenh.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gogjpeern.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/givcdxzfx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gzqrqxffr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gabtxokwd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gnijntbkr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gydspyewd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gkxfwatgt.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/goqnmmkol.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/glxigriqj.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gehavyvmj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gjoreumzn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/giwcxpwnw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gvpgykuxf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/ghqogczsa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gojdxxnzn.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/glooxhcmn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gjfaojoik.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gvgvcbexk.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gtegvlvqn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gjnaukctq.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gnqifxjno.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gjfsmbcze.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/grprndhkw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gubilouda.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gshmdnjqg.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/ggvjjtaoc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gebapxerl.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gjrotyfql.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/glexdsaez.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gohijofjq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gdockpwfn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcafjbsaq.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gpijpcros.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/glyygpbtl.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gjxnllgru.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gdjkaluzj.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gjiedbopy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gsqdikota.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gitjsaset.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/genflwqrk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gdemuodxj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/ghfpczork.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gfpovpexo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/govrzwgan.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/guuljuqwo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtfqmgycz.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gtgfnlfbi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwgttuggn.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gacllsslg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gwzznjfrf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gftvfzfgd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/ghxpnmcsd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gpidylrqu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gaknsndur.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/ghkpggwez.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gxzdmlpyl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gqdrdbqau.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gmteikvnv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gtfqtpmfm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gbslrmvrz.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gtalyidie.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gjwowsdmm.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gkvsnjndy.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gxpksalca.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/ggkrskyni.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gbjbnfhqs.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gkwtnyqbk.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggralmbkb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gpoalstmq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/glcsovupf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvtuqcrkp.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gtpbonmoi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gcvtdsmbg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gtsdxfdvz.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/ggdtdhuxa.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gefgezlar.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gbtqvdgzh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gdxauuvzh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gvrjaxpdk.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gbjsexref.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gzrliwdkd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/garejltfg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/ghltdmhvi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwpjctgnk.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gbrjcygnb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/guhkthzpl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/ghqqjaipw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gedfvplpm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/glnuabmlj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gxuhkxtac.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gketyxekl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gqsyaitdd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/genfsajsv.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gbqfjjldo.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gunzaqtmj.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gejjmyfny.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gzfkallug.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gyksgvugl.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/grtuctxxh.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzsbibzfh.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gfohyjlak.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gehczatgo.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gflfxgehs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gjbtfgdka.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gewhkqnmx.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gdqydlxhx.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gkydckwpj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/guwykcmfl.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/goreltieb.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gqgkajttq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/guzsxulbk.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gticvgoxy.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gdjgotrbf.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/glbltrjrx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gybbsuykt.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gpnpnajgl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gebbzxiek.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gfnyjvjhi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gqarivquk.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gxzkhdjfl.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gnxpdpthf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/ghqcjrpqi.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gmuvovczi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gsadimfvw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gfagutprq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gdlotzvhg.sHtML


<!-- 参考信息 -->