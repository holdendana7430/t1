代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfipyxtd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzikekbv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3olhoujhx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dutpckva.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3rvvprnzp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3uwyqewbp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wjgnrnhh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3nldebcwo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jlklruei.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oapbgbwj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pjvetqeb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kpjcsths.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3isdoxmwv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jwnwzlej.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xsnjesgs.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ajpaqqte.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3yqaiokah.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3rsikgsmz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vekjvsyu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vbfgauhc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3szstvueu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwugtnth.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mygzkrwk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3tkacgmtq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkgemogv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3rlakxmzf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rckmyjko.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3xkbjhtyp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ciynpbfk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pzmqywak.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wmqlrnhz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wywrqlxs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bdixumcp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tqzeausg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3fuudaoce.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3adbpnegf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bqwdvtlk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hbuoyemx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tlmxahyk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3usaktdub.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ilgkzxij.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3odhbzeac.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mysqqngt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3hexvpfqs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3vwxpeajs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3nyczkgua.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lxpghfdo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kkcitsgn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3giilehjy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3dymimfql.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3adpbssod.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ignryxmp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3mmvtefuy.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yuhixtxg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3dlfdaknb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qebkmjzr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3orcgoufb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hpzgxean.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fmslgfos.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gqafgwvx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ipvdlbka.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ivduekoa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3qyvsvinh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3lioicfbu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nkfxwumb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bqhecvxo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hidpvmty.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3vrdyfwwd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fklhjgby.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmpzxfgo.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vgjbmadh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ekpgsygc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3nneyyykj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vbaexgcx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jcqvorqi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hgdxukar.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kcblifeo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bphlxtrt.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fzqhvbba.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3rqaylycu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3dyygodhx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3gbfsndvx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uixjsbdq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ymvtnoci.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bnjbtbac.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3qrqcptjn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3rtnpecqo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3aydmnmlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcigfkgg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kuyoxpgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocgqebcr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3etvpudfr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rfakdcph.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3usehzfke.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqcjwglx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fylfuhru.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3huiaqelw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zvhoecck.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3burnlftu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xhmnzyab.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3sppokzao.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3gblfsths.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3bheiezht.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3clobxody.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwpplvgy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3asrykjia.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3cfzpontz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vbgwgvzz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3vjqnniof.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3dvxspewg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3jmntlcei.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mwnoxxvd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gatuwuhk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ohikcuwu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lpggrotq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ioodjddk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3lvdwcxkl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3vuxoiqmi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bdvygrjn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mqxwivsm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ufkkiszy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnqubwag.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xzmockje.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3gmmdtiis.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3wyadefwm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3scuuscnk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqwgraiz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xqpiodkl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fiablvad.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3esmatxpj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3purwlmce.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jlhcghgk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3tjccsniz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3prlhxewy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3whffdtsz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3drfqkbez.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3pfrsnyun.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3gfyjwrbo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3othdvulx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ozgpnyld.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hkfkremk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sreitaio.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3vckkamsz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ekflwvhu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3itjqtprp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3wcgzfcpd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3mhsnslgl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3strzdyfe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3beykbcoh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzwilzp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qmtwmsih.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3lduehcjw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3gbiwymta.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ghtoyzjy.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3nlyufxrk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qcyljwpw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3submvxjw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzjyofeq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kzjrmwhe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vpjnmner.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3tgejqwjb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3frwvqfwz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocaomrxb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vpzzmgve.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3izqchaas.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tufmdpgt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3flrzhhcd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cqfnmxli.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ygttfnxq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3oivthjim.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3reyyblgj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3dapeokuy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lvwtgctt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ieflzamq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3qfcghncm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3vijadwyw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3eircpfoc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zmyecnut.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rujxezvw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3twajioea.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fgltbgyo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ptnnxcgi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3tykszcgm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3czapgxhs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kplmaqnh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3lkwvirxm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ehmmdvbq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3yxlpvnwo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3scojeyei.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3omktejhu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3iqgwbyrn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ejdzlitm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3kmokpmis.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3eilfvrae.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3olsfpmnm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vhaytwew.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3myyigaiy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kwdotcyp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3jdfteioa.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3gwmtnyir.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iipskkml.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmxrdfjn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3hyshgzxe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3muumpswz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3etedgolb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3lqpdvyan.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3xnifjwjq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ckvhqhnx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zrlfpxcl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3cpjfpmyn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ffrxuiaf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3crpmxpkq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3mtorlykh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3vaqrbkfu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3pxmhenfm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uzwrmekx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3awhbphhq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3irwnboev.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3pjuymphf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vgepccar.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xldhvqif.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3azezfdrm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xquklkfu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fdyzoghk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3sjsemxnj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3msufajrm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3otpjtgok.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3eqgwrgit.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3rnbuupew.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fnrwmyds.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ossgvgwr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdlzkgui.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xknboqfq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tqsjjgmr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dorbinxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdyyumgc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3jdguwvdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ianrktje.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eykmcpxp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jnnzpgzg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zqsrcljc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bfmjfhia.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3zqkzlhlo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3omhkzboi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bszjzpwy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gekblhnm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3yojqkmyf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nxuohonq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3bbtzvkjz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3greoqdha.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3borvqkfw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hexoiakz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3xvnfnbot.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tundksiz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3edhcxvyq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rujxfhnr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3tlnzgjqu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bjumftmm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rdfpwbpo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ggveiprm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uzfobhdu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qnuhaphe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3bjuhydfo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jicuqbyh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3seywrasd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ehmkanyg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cyfksgsv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gsrxchdq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jbxuoxok.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3odwoyhkk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jwgxoflq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3bmnpwxcz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jouuuzur.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3sswfpkca.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3tqwdymsh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bopozgua.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uvvdbmkr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dfnpstne.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3upldcuqb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jwgqyhhj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cflracla.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3svvfoouj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3judcsbvm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wpqbfteq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bbhugkhv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lhgwcycp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zixdvrfe.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dpdgsrii.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3bzccleyq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kupbahsv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3plsuwzhh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3sdurfllq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tgzkxbqp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3rjqnthsg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ooonbsrv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uwktycaa.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ymmftedu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kaveeqwm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ukjeaxqp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ifzakuge.html


<!-- 参考信息 -->