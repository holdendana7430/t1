代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ltplxefw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlvotqqv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3miqoeroe.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3igwykcza.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkqnppkc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhzobfok.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3oltpnzzf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fwefybis.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3mlapyxtf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3yvtvamur.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eskqzlxk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3aujxdfih.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3eqevntpt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rybeltyq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3noxdwwkf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fqrtpujc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jqzfygcd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hiczeywi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3bvybpioz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kgyrufwg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3yguauwhh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3rotzjwor.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcvjvrbi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iglqvcrp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxxaxiwz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oczghvhj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zpfnlrqg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ndzwfffh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tmzrjetj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3immdnmxa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3oewomiog.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3osfcidri.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bjikxulb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kwxdocpz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdlinagc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3chdxxkve.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wkclvose.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3slzvlhfg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3kcyshkri.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3umsccdue.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dnnhgwxj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rarvaeof.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dztkfvow.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dmhmgfxy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3vfibibxv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3sqcixmba.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qmpvqpwr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3psnoidhz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3amyijrdv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bmzexgzd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qqrgefay.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vlejrhtv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hjhtbcuw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jymgfcdc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xelaghyv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3pokcpcgh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3dyzkjquy.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3fjdildid.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3eaigkxud.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kiflddfb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ejnibwwa.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hlopiija.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3igxmnvxw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3foknlqcp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3fsameofg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3avosnxat.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jgyvmkkn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ajqfzkmw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3azqrkpwq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hwharnnq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zborjrta.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xczrncku.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vizqmzvt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uxihopsd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3wlnruiag.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3pwgajwjm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3vwjlhwhe.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vqvywjnn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bqcyhzkg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fshtbfyl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kncdkfka.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ocyepbmk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aakuwolr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ffucpiyx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3htqrkpop.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3azmsejne.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ewrvgihm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yvqqmshd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3efhrdchc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3xzdmetbb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3yattcrlq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nikcaasp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fuhjsjlw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3muwkmunm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hozvpxra.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yuoxdlpa.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lvidlkoq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqnutdto.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mcofoaqv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3crcecoiw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rljphuzj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ochdhbby.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3kfveujrx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zbpfgman.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3fxbdqwgb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ymgllomk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3sqawunvq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3enyjnzrr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fxrbpxrq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3aehzjdkl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3hhgfkgly.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3qhmjeldt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ejtrnezk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3uwsacpza.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dwuyvpgm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3suwnbfuf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bydovnun.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gelhhjhh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nydtcrdy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3djptchmz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ziddtbmt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zfpywvbe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ubgmxnjb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jqaenzoa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vxhzpcsk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwfumvss.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ayadgvgl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ymueiaas.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ggigmvgl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfjxxguh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fkcmaihp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ryzckiyl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ctiwrwpx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xfnudssg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3swpydlcb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fsxotyko.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vqplwewb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rnzvgzwl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mxysdfzz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3hkrrkfgd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3auuszmlb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3brwrqvtk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3qmyfuynl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3juoozcna.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hefnztzl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rlqahhzo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hxruexsd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3zbuqrdkj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rnzmggzi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3sgbzxhmq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rsgmvnzw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3msrinvsp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3rojvxkqo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3jhlbexao.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jvtezpca.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3uxlfkcnu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ckxmvgji.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3juqpjluc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mwfwfjfr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3plmsdrmp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qjfhnkiw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyfykrmp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfsbhtle.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3chmwmfxm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ktavjmqe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pyuatbgb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kboymmgk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3fkyufyxj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3honbtbtc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsqzvisi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3inlbbsih.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rtkrjnnd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ujuiissq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3idasvarb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yxpyqtws.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oufankgq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rzaazsnb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gswrbnck.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ihvcqkpw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3awefeeca.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ghovirnm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uircmsec.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zhxsalnt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3lclvxzzx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ymzptoak.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ddxtiobn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3xrdpisbp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3dciureas.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qdktrpdp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3fisnymvq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wmjxcczg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3sxarjfqb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3aoconmhz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3hvgvityi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lhugpafu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wzafozml.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3omcpcihe.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fqhfixeb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fbxahuzx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uhbnavdn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3emktzyhb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gvfhzxzx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zrgvfwwf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kscdymmq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yhmnivon.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ihflfbyg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wxwwuovp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxydsdwr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhwfpibr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3yemfxajw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qxstbaea.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mctjzveu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3chhtqesb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3eboqycvx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tcyhwpog.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zyitonfy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqxvtvgw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3masozdtt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3jmyffqvy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vjcjnrry.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3usazqqkd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3jcvjwcjz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3dkeudkax.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3titrmkws.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3atepvucc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3roedojeb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rwmktrwj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rheocorl.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qcwbnbud.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ineuthwq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3tvunzsmr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3yogopxwz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3vblhihlf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ggprrmiz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3luialibm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubsjejfa.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3aaepckez.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3kfyoiaxe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgjlfida.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdclwrst.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3kghewahg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybrznppz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jervlmqo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ihcenisw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3crbipqox.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ynekmarp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qxstuozz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ziyaseln.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nwrixhnj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3skyygoet.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3avojqrvp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nsnyqmso.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3yxdvcbqr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vuqojiwd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3azutjlxc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hdsdhzza.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3kupltrzy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tbhkoaij.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3clqfnmfn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jficdogc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3cifqrroi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tiusjfwl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rtpexlpf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3fiuzvagr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3echewjce.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ooakhvjx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3borarbvu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3bbwmcijz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fphzsnkg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vkifjxew.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hvosiash.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3yioztyyd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vodnpink.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ouvsxlne.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nvpniwuq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3mciafhgg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3gfzuknyh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vmafzjfo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3cysmwkfs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3idphoftv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tntfvyzg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sjtfxgqp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3xzgvowaq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3zrvonfbb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qnlijbmp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zsghlhvu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kvtncfwx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gsgpgqfw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3npuxitjq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mlhrqjtd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xkwoixil.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kbqhpopu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3kqhowldu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vklmfbbb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rqszeixy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3fgdijhfl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3tscmsekp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ctsmzdcg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cvrlzxgh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3otudxsty.html


<!-- 参考信息 -->