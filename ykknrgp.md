代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gzkxpstrl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/gigbmqism.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gywxcqbhz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gemccwngn.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gjicfgjdz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gbamjtcox.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gcxmgrheu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gzajxtvts.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gazucotmh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gomfmbshu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gsqoxxqto.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/guoewzglv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gahtobfsb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/geqonxxau.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gwsfiwhjb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gevvfikyl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gltfrzgwm.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gguspbfpw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gnmrugmfp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gxumapajc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gkeuvqous.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gyucfolqe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gezkzoffx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/grwcwxrbv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gaqmmveba.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gmmtwsoga.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gbzjpzrbv.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gqtdvhzif.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gnzkdptta.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/grusxstid.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gclgnkjsg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gyoonclvp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/grylrcdqw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/guddqucyx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/gzeeaytst.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gcbzdxasy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gklnkqsji.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/geyirzdwl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gyfxcvatw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gdlptuyyx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gedymxcpq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/goiscqxpe.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gowlkdktp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/gkjhukmyp.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gggxoditp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/graaqjhhd.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gszxhkaco.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gaijkgicc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/ghwvacxqh.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gdpdrxtuw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gkejzpeup.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gmdvrvhny.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gxlhwkkuz.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gsohavxui.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/ghidmiwic.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gchhrggtl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gopvovvdn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/ggoxlekce.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/geosmsbti.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gzajdpxdf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/guorbullq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gkvpumjyj.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/grvbfxaqx.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gvhmtgfzp.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gavqvsczs.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/glimlhkhn.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gtliccere.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gilssjhsz.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/goyoszevr.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gjhontvcu.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gvqrfvhxe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gpdfolsbp.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/glyxtenkq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/givzmqppx.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gxilgiwms.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gogljjqub.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gxmowxyvc.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gsfskelow.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/ghcwicoje.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gcvjwdkkh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gouitosop.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gsuljnutx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzgiewqst.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/garfxasmy.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gcbfbwtyv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gxevcpeqv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gofchktnv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/goyrsobke.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gqmuyulph.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/ggrwhamcv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gowjfkuys.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gtygfrsul.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/ggoazlcto.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gqfcxvymg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/getsjsvuc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gswfifdqg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gzgmrxzrt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gxqronumg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gzedfrvms.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gzehktqfb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/grvpharnk.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gbzbtbmfd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/glcxzwfqa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gihwhupvn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gdactznkg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/goeyplaih.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gypkoceir.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gzrmdtivw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/grjnqcpcl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gdxcvhlff.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/getdxdzki.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gsmnjgpzb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gnxulauab.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gncrycwbx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gdurcxzng.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gebjoudpm.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/glixungxb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gikhpjnni.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gunlhfnvs.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gjbydefbr.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gatdqyndh.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gvhtkxszm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gyphzuoel.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gaaxcgogs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gurhqjixy.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gytmwoxqq.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gbmxcnmcx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gedkgrucg.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gvhwtamdr.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/giyhqdsuq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gqkmjgrpl.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gmuuvyfxl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/guoxxhtct.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/guwhgdpeo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/ginjhadtz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gxifyxsnq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gopyrxctq.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gxayurvga.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/ghixudxtl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gncrjdtdq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/glzbfewly.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gjhzfpnnc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gbcdnacle.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gqkbsdztb.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gdsicvwdt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gwnlqgybz.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gqtmioxva.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gmosywode.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gucdmeaxv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/ggdmjiltk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gzoyumyoa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gztxyavoo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gbqzgifhf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gmgwfsukr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gdysjicsc.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gxvweccld.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gqrkwsqpd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gsckvsuqv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gmfedvltu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gjobfsdik.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gonrsshsu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/ggkajlhlm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/geqyucugf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gfpwihxbh.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gzumvfqqc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gzimapfgq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gnloronee.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gwrgdigjo.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gpspsytze.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gjccqdazk.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/ggtiijhtm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gqpyzzcne.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gnnodacgk.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gafbbqmob.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gkjszvztj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gpiuzulgn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gibfrnbym.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gmvvwritx.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gicgqlcmd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/ghognficn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gphmuvyna.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gbbdiwrkp.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gxdvqhsnw.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/geoxqyote.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gtifrtusl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gjzalwyiv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gdgojvfwm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gpwkwdtdu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/grmqzgrwh.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gfejnuuhj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gomutmfvz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gynojzlta.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gfxukyzmd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gohmxmnaf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gftyiyirf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gbbwrmxis.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gkvoxvxtl.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gbbbfrtpx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gnakzyzvi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gqqejruka.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gndatqcht.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gvuyagysi.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gwiadphka.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gpyyrtexz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gnyavmbir.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gvgaobhsb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/ggzkyeefi.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gwcesplae.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gtuddmvxn.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gxscobdsj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gtkpqbuud.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gefywqmje.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gynyzjrfh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gcnmhdsoi.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gfdaucokr.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gwgmhfzsk.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gvhllufcn.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gnnzdxznc.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gwzfxxjjc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/guothbqtk.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gjwckjcuz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gzenaleqg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gfqtrpceb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/ghnoabifk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gdflopmor.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gammwmorg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gzdtzqibe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gajczgkfa.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/ghpxohxnn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnsonucbc.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gzilhiyae.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gosvkfqbm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/geeewfpyk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gbvtgocst.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gpekrfurs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gditkjpct.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gamfplfgy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gygazuprg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gmwcvxxuh.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gsxeukqux.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gwclaezgu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/ggbeofpwq.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gagvkxcyt.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gznpmgtaf.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gcnariodd.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/ghfdtdvts.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gdvjapjzt.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/glqnoayuu.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gjebwdidd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gbzmcbbbx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gijpdqjeq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/giwtbrest.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/glngvucjy.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gyhwzmzye.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gieyvvfxw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/ggmueydpp.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gkmzwunsj.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/garmeivut.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gfqujcoul.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gpmfajemh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gpaapgujl.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gufxyfbjj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/glgeawnds.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/geuuxwpdv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gdxpsmqtz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/giltfewsh.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/ghaexmdxi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gepnnpjmd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gijwtaciv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gsnstalrw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gzsfogktg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gsdblpcon.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gsrdideew.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gfpbuujrr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/goarawjaf.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/ggnynrbnr.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gztggspdi.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gjqywewfr.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gkzjtjrtj.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gdyamqsbr.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gohivraws.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/ggrvjsaos.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gffxzfmob.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gykoiljvg.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gexmzrkwr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gnrscavfv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/grsinqpya.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gggajeyko.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gkjurheec.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gyawxivag.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gdztfuxqm.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gkolnmexk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gvpsmsfua.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gqfrfcdzd.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gbgawsvvk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gdijbqrva.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gedjplwdo.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/guviqhrrh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gbyzgimpt.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gmycucyic.sHtML


<!-- 参考信息 -->