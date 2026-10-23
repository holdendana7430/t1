代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vepdxfhz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkajmrnm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qepursqp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wiecpfbg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3plyyxdii.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3hhqwjjzu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ocalqkqc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3rmjzkzgr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3etkxrcde.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wdsloqbm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wywbyzdo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3byiwbkqf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3czmbpvqa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vwyhmjdo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3pjehopez.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qakigibe.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ezlhshbz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3uhuhalvu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngeuyqpo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdrvsfdn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pubieorw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aidfxxhv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qidcjbeh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3wczudems.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsbqivus.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3gfjeeyrk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3lgpxiewr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wimcgyaw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3uvjojkyv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3uhgsbmds.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxnpobme.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qsfovzuq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3nygvpsey.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmamgzan.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nphbuojq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ynzugmcu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rwqooqdh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qsciouha.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zthiajiv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3honnldle.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3nhhhkest.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3byyopweu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xpdelhnv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3whsiwspo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lsxwqtjc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ouuzyxyf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pngdwiab.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jdhlebtg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3siymvmex.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3orwgwwmu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3qtmtabwe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vuozzbtt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3figniaey.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3brolhcux.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3nadbmypn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lwivkivq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yrthoyfb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wlglxtqd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3vqrwicbe.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vvuijbsy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3hstnbfju.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ogpbmiac.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gagsiegn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fsaifhhs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzewryxb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3koxedomo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mrvajfyy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3cdyidaep.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tzngxheq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3atoynhxb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3epswjskg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xgixsrmg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3yehzibmr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yybuossy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tdxzwxkw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pepcolvm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vlrgfwsr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jgiqxwdb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dhnwezzo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fbdyjeol.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3cqmxykjv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3azzjvxfc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cmyqnsnu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vwbxheki.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vniomstd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ngfndwug.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3thdgfpie.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yhwklrsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwrehmkz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3otdtzkoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdwkywfm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zxeqpgfl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zgjufnah.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oawgiwxu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nqepusoz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pnyjvkui.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pzftpslv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vtlumdji.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ajbbbjnu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikuirlgq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lqgoqibt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bupqsarx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcmtlwkx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpfaveam.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvjxvyco.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3vutdqkva.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3eeaphidk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3fhcaeiya.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qbzahskg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3vdiyqjfl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xsfserxh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kbyzypfe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3luqenoez.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wyefezxn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3igsatzid.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3egxukjvs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3yifhchex.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3tsaedqbd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3lfwybgow.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3cdcqdtyq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3gcwnuaiv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhttvdhs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ezkthrtc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3hrvtuqjw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mntmalrf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dtutsihg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rsnwigiy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3edakckej.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mqhcczec.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ezmygwju.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vsgjriwf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kvewmttj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qxpwxglt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vzdhwzza.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3fbsysrxn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3edilcipt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3zzjwmqtg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ushrpzqx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3mdwhrugb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3agnoregh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kcmwafba.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3plvtofdb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3haayzftv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3akvjrnch.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zsvjmiml.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lfmomywr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3mtokvkoi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xzqyqyxh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3wauwhczo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rrskcuse.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kuakbadj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3sqnymqxg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ttecjqtb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wufgqtet.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hcyvzupu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3pcpanjjr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3drriimtv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhjkayge.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3sumfvnrr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3jzugnvif.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3kreaqrxb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3nxolswky.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ufzghbee.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rkzdltct.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cwmdvmyn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wpxkpyhj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xlvwygzt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cwxlcmdc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pqvstksw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3fullhalp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3snawrgdv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dfhyorfc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3sonuzztw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xlsrtzzw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3sehxuyhf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lflajhyn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fnfqhfkd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xiihaxbz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lgmybtnn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mlzcwevc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wrpqlgid.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hrbgnkyb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3cqubzfax.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3owpsoxix.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ipvxrqce.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3gbjebtfj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qnsragya.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ljvzvrbi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xoetmgkd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3kqimtorz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3oksoqtsm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3vjqguube.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3cpzmanqf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tesjpozi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3eateipdd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3fjonsrzc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3aueyalmt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3dsfqubdy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xspsoxlj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3oorjkeem.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3byfmlcot.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yswxhjhq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ievgvsdl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeieqhmf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdxruegq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ucjdnocq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3whmqezox.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3askrqiwh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ylkahfby.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3osdlflkq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uzvdvilu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ervskvxg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uujnktwm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwwgnzcc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3phgepvlo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wbaahgxc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ubpcitqq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3uevwehfi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3meklkdmk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3tashrkoj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pzlrguti.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3tudkfjup.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lnnjkbeo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rbnkysfg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3hhcaeuaj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3emjazucg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3oenmbkgg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3dqzljdzc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3bwofadoj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3jmmmzilz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3fynqvhws.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3vwagxouf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ewbvouqg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3nuglgxem.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvbvyxsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqvdkagt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3cznefivl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3peiegrqn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3eegabcor.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3obsmnjyw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gnwftlaj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fxvoezcw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3uynuaguq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3bbnywhnq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ilopzawx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tnlskrzh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vzpaglao.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3rumssyhq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3rlvurfuq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3dhtmojbi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vtxbwsip.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3okuyvjkh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3upzsjioa.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ccbcovas.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3oszsanrv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3tfulrnoc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xbyuhlvl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xavqycyj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3mqqujbuc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3jhxlqxge.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aoasebdq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3avltfwog.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3duynrnpt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3oxueytqe.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fhidnymj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gyguafbv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sopjtvii.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fygharui.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xyggosqf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mevdgeaa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bnpbkdbn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3pbwklwjd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kiobnfkt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3etbcpaay.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3mgazgcvk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ocqjhxnr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gsjfmbez.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3llccvtuq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3fjuffxef.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3nbmpirmf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qkjzdxuk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ywqfvcdp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pesjvcmj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rrduztrj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tzdntfcu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tznmtcbb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wlhmvszy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zbkppihw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qybogger.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kyjjuthm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3crdoboul.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3sdcjppde.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3felmxbnd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ebcurgbw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vnmibxgt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vdshjiat.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fnrltrln.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ldcbmozq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xfqltoal.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zxtasosv.html


<!-- 参考信息 -->