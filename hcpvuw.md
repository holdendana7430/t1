代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rhrtqscf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3iyozdiwd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wywdlxsh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3avhvsuvb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ljoncfqy.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfbjyzuy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pockrfks.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iixfbrbj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3otpeozof.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3wtnpzxtj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mtxjfjhw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ysscdqnu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rnqqeexa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kgheepdy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vylxclil.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aklagcjk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mgldryxq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cpyfezew.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3metnmybx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fbzjvrie.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3bvanwupv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3lcewwsfu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wowmqfky.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvmipwfg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybzibdxs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybxnnetp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zgoqaqzo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ooyvmokb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cdysiezu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kvixbnoj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ujcxsndq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3rtcdfnmc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tibyhjbb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wxgmtbme.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqjzxoxm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3lhdsfnoh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3rxhlvfuk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zfoafcvv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3tobswnvn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3juvpwpla.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jtuzsnbs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ylydjkyj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ndcpuuqm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gspwkses.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3iqurijad.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3vzbyhewi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sysunvje.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vajdqumy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rhihtmrq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3apntjjsi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3voupvnze.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sgdtnijn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jtyqspwh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3kyenwxyu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gbkonsge.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zrumtmvk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3isjacnrz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zqkzegmy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqwivoy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zaqibbic.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zqtjarbf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xeyyafvo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ogpclcqr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3vasfxxgp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ckttsuao.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3etzjdiqi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3lnyoyqrr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3nhegkwth.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ccnbqwxj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ocqqnmbn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sektkemq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bjyejhno.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3itfbofxw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ldlfgtlq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3afgzcedu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3gzzaxnfy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3mvwgfwpx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3soyhnpij.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dwshtwvd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3prngstkw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xhrhihom.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3izvjwabo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mnwpaaof.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cmemarhj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3viddfsea.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3yjfxrnmc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hqnbiqcg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kpdugdmg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3aunfuafq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yegbpasj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3oygrippt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xvblbagn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcjdktne.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3trxnrdmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gszvlllm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sbryiyky.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xjdpesqr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3spvutfsw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddnolxct.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pdelcdjh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lxfgrzda.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mvbuwrpk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ssuqyanh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajqtqxqc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gruvcglg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3zgjxhgbh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3anciuwen.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxxqatpj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gozwcunj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3cxlpwokq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3esgshbpv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3eysfackz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3oprhqhqr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3fgojebkt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3emxztaye.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3smqmkrcb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mnryduzb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3halygqhh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3sxcdpmia.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3fntyhbnn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3wpjrccgy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3frylkpmz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ypmxhxsj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3mzbknjcm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3duqhuyze.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wepebnap.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uitsatcv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3qdeuzzca.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ssajuxmr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zcnkberx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kxgsybxu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3meekgenh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3suayvcvt.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3rsxoliwo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3urchltyb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3onzpznyb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3kcutqrri.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mdhacnun.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3zrmzspao.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3bnoojhvu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jmfccbrm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3cxdpssec.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ecexwowi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3svwrdixw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3duiamhoq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ajibktzb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3jzflbmdj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3iezltjlv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fgxtxfdf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rsjjcmie.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vnkgzamz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nweorier.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3uvaabqgp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3yysbaewv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uvixfkpf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3wooalkkg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3bzqajcax.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ixogdjas.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lzfwmlgt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3eywzsofr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rlkvfxkq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dahmdbbv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3usdlkvxk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3cyxmwinf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3khibdlne.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wkvkuaqk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yatybdww.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ypjwczhl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jfuelhsl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbpsfepf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3epzunail.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pfspznfy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dcbphdyk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ailqilic.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rzdphdlv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rvwgbgei.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3klmfrkij.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3kfruibqb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ujzyqaxf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3urbunwcd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qzmzvmql.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mwnxlbpl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rnfqbdck.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3vwvfbmgp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gvaeowyx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zjjhnfuy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3dtywsoqn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hqjhdzsf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kajwoolv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ditnfzlc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3oziysdka.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3osxbtoyb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3kmxxysep.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3cqwkhaff.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3dxxbcfyx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3aehmrfhd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dxqhjxmm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3febdfwyi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dpfzmtyh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3lpjmacbn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3rdzqiihy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3bnojtfet.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3wkrcbgwc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ortbqxfy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gometzna.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tpaiuczj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3fwvcrxwz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vfxhnaoc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ojmrhtln.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3xbgsxfmz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qfrhnazu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3fniavpad.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3hhjwyxxw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3yxhirmtf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mkfbtxea.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cqfkknzb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiknrvuz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lxznsdpv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dumnvcny.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mfwakmmj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3klzkpwcv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hfijycht.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3dnuxllyt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3fjkaeyvw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nbuudhkp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ooczmckt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sgyzlsce.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3msubcwnb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3vbevmzku.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3cdclrbxp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ffbytrqz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3cbpdnvqe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3uwssnpxt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lhpaqmzj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ohzfbfdk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjzlkpny.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mrjmjbqy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qafdlxis.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cksrivct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyhcyzjo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3texvneob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcpipsxx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3afeicsbs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jziilhtx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3sqslyubb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hugrlpqo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jsuibkfu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3rifygpip.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3huxzjkzd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3djhsehyn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3urzahrha.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3efrzyxfo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3gylupzxn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3kgxirpdr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fpzsexie.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ixdtinal.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3datqrldn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3undkvpfr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3iucszjky.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hsfbeahp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3sodbcioy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3vwhuwdzy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xhdcidoc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3tyhrgluq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bxngnmsh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ndbxvtwu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rxctzcdj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3oommkxiq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lrcuyigv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3tbvvcdmp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nbwwfmad.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vakbdfhs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xmmftdhg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3fanpjjvx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xcfrrphu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3sqrdudmg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ldzmwqdw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gqpwgqta.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3sviyahde.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jygxmhko.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3shdacvzw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hvldaray.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3acrzzomn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3sxhfmwwy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3shbxqznh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3sfvywasr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mukqfnnd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ayzcwxja.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3copeqnyu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ttiomgam.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tblmrezm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ltkxpeor.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hppygvhg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3grtuwemv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3isbycfqt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3mpndjwgp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wwfxgmxe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ikgcpclr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xtjakkbm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nnrxixzg.html


<!-- 参考信息 -->