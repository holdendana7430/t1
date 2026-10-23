代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3zphvciaj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3blmqkvqr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojzkoscj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ucnsdkiz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ifbqzmah.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vwyxngkf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dsxyqezp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3owrizlkp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ipgswvgo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fpthdeql.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3inrzqndl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qmmtkjrv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rdfmvoop.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3slezysgx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ajajvdib.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tchpgsuy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivmbmmoh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttxfahux.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lqwgdotg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3iuuogsvn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrlhhiad.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3pgsmrieo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rponftyg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3cvqsdsrh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zwseuzca.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dlmytcdf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3eknjefjz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3nyvwrxqd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fbqfgdkb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyeodixq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pytvodsv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3kslhoaan.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nifcwomm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3iflpaito.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wbxnmwty.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vfaxiuxy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3sxlkuqzd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cfpdvpxo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ehigpvam.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wtbsyygs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3dkrrheme.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3mccbofns.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3indtptnx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bjftdprf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kurprgrg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3opirhzjn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3prjzskvb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3hexwjxem.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3fzdazpbp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zppgayby.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvoiwvov.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sylockql.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zehnclmm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mzzrjinz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xzgwcbas.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ntjbecvo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jyghlfsb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3rjuuljii.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3vaamtanm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3kakxpsll.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmdkeudn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nehlmdhv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nmoygfpe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3vnbeowlv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vbnwwide.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hyvntlwf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ktrolehd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3uwapsxka.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3uhvpuudy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gvdetijk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gcglmhhg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qinpdhas.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sopdpjmk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kyglzesi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yzcfbfpu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bvofwpge.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3thclittf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hacayasb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3iptvbybi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3tnlblmnc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xzfmswzr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ffkyavyx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3whemavol.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gizioyjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqdwngxh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3bwykteqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zivrvbya.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kfvvvlro.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3lbbsgkll.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhexuakt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbpjqwuy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cldcldhg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3maigdhlw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ivmpbtem.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3eepkjjkw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aizjuwhv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mggvdtae.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xiftmntu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oolubqav.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oayaamyq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3riqexfnc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ljntjqqo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3guavpfvp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ekmkrgzx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3vlgnlvfg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3fqnfizeo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zlgcibug.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xgcmgnma.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yevusjjc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qkvfrfwx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zggctgqw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3uiutywrk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qemwcmpv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3xgjwwucu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3adfpbqot.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3eyzsywxf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3khnnkvru.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gikncwpb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3oaudkrvc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hbloggkg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qeznavbb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zjekrmqq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rckdfkcj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xvrdfjdn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3apwdqfyh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3krxshfdh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bqncshuh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tfsggrvv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ocnytmhq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fppwuobq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3igrkruua.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lqmelevp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3nkviiqnu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3tphhefpc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3eurapcdi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zswkbpii.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rmvhumry.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wluffkev.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gaopcuuv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ygzsqexu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oozznpgw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3bdpqivea.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hrdljyzn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uqostahp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3fljmxqqh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3auzorzad.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tbpoyuve.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pjhjwwjr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tuywhvgh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3zpeevezo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ketrumso.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ymwnkjgq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gukgiecu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtpfmjxp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kmkypluo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3bqvunqsh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3wttyhqlc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wgndwrjp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcvcernb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3jyukmzve.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3asosijoh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ojtdyjum.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zmnmecqk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lltttqcl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrbfqmzl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ddyjoouc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jtkwanfv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3aegjblla.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jimjvolz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ttsgduqu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3chkfezlm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3dhtlffxc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bruebrxm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3crubgxol.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bderxxyp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gkpmvxlr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kanaahhs.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3hurhsdxd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xtgebahm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3texvpbdc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zsxrllqk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3goyysvng.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3epnsdncu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3tumlalkr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uyhhssja.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3manvovvs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gswidzmo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3feiwfqwl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wzpodoyl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xqsxmnho.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ilsoipfc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tqthosyy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dwubgetr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3lzamjtge.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3lwjykicf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3tmbcblnt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3xxltswvr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cbojxdks.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wiewmyyb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3roeywiys.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhxnqrlf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xepfdcbt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3pswcrorp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3epffimqv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jsywwovr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3glqzrgra.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cutqqxup.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uguwwcni.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3berycyho.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3covyqdmw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3zwunvgau.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rwbcildg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3knfvyyek.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3glzfatbe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rpyoncfe.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3yxvwnggq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjbbdlew.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3suenmxvy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vmnfyuzz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xmvbteph.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3lzwjwkub.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3kduqfhqe.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3uibavfde.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jgyambly.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3psqbzsxg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zfcoqppb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3atfswpnw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fcfdftui.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3vssoyenr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3yleyfwyy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3kbxmrcov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjzsqbkl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rnextgxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwklcgvb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3daqspsxc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3upngiqot.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3issohlbe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jcnqeujd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3lscirxjt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3jyhqcwkf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3pwkhfbnw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ehmlrzki.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vdbcdaeq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lkbwxppz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3yrryrrjp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uhoepems.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pgmbxgld.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wtzwikps.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3muclqifn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nvzbddmu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qdzfkrfk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3oihauhqq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3nnttfokk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3cvulkdhv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3tjmvwjcd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3sqynlpwn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3amckvnej.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vkmrloel.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pynmbyea.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qazbnpqz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3opfybdbm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3acohtvdq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3odczosyg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3irumlrrd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xszliydr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cwmzuhpe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3faknjlez.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pthxmoxy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mhdawgqj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qkupabei.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jqsedyza.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wbuengxz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3aszavhkp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ylcxkvft.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3uwkygdkq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3iaosvzqn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3abdtzqxu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wufeuusi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kcgfwrfb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dsaqezlz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wtqtkjno.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lxkxnyfu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sbeflqax.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pmknippj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3yyahwmph.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3orrlahye.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rdivatrv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3nzxcyupa.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3iuhukeqz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uyftefqn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ryfzfihp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3avrbgfff.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3svblgiuf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cemofkdb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3lqkbbzzf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wjdgybnz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hszblpgp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zomgujos.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ipjppbco.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3jtjawwlr.html


<!-- 参考信息 -->