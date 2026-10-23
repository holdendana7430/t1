代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rzwkpijl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hdtmkadi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3bklclbqy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3xpvuzctp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lzirwhov.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmozpcbf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xcbnltye.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wrewcldj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3vrfeulnk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3weutmbfg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3blvbmcmk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3omcrxqsm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3sosfgdci.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hgmjmwim.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zzjdfvmb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wwugpafs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rzhvimjz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wleionoa.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3jwnnxjdz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mhohxbnt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ldpwujgo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3njfviusp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fmhmhinc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jhhqdiqx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzapkcsp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3srdbeoaz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qhlhyoop.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3wlglxwtc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiitplne.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3tdqswizu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hwkgxylj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3chahxidi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3foxegoju.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gbteddrx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwgzeuwp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qzmxqfow.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pdozibxv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3scukamqe.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ittnfier.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wuotfdgb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kvhpymdw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zwchgrmb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wwgirvzs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zjfrsiyq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3hmfuztgj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3buymxhcg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ppwmmprz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3eoqmnzzz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ooakzqao.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3bqezuaic.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xyzcxwom.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yfugkvup.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zphmwpft.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3iosdlcuh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rltbhhbb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3dddryfdb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3qhhcjwph.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3susjqbad.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wyapqrsr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ppvlhrqp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cczencfc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rsomjgmb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xfhqsiaz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3veukploj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3spvcybis.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3smsteakj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bdqjtkzs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hqiokayi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nkheensk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojlmhpud.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fypxmtvu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3suxvdptf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fnxistpf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3quyyskqs.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gukppteg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3emigmpcr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3dciewjfe.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yqkfvboh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3glofyads.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ywvotwsv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zbxiswym.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dxsjmdjy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mppurlsc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3woziuire.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3yzcgywrw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3uiblgdgm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pulyescb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3eczqigbh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ywocpkve.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lywmgtqi.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3potuwbbo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ulhqzwmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avontvrx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zrreutdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpysrdhi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3scpzpxlq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3wkpqipqq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kpxjaxgz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewisyisv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipkcuskr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zxpmrzmj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vpgamdem.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3fqobjkyi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xaqocnrr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3yipcwalt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3mtyvqhda.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vxewbwrx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yelieyxl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3izowxjru.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3hqhhdamj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3wbqybmng.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3abifukyi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ppkcoxsw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3kbhaqfon.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ktilbwrp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3dbrnbxhr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oehawmex.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3demasuiw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzlluzzg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3flouhekf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3zoieqmhd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3dfusioea.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3umgezjom.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3grqbskhr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3jcmjnqmw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bbubddqn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3aaulmwvj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ycxpgwjt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3iuixnibv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qltvwpwx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nuiuwcgh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3cvnhelkv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zmkudayt.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3bsyaejwa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zwmvipwb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gqkfhpjm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vxwycypp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vlukwnrb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3otxaxjmo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3jebdwqjz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3eywrikkb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3gexjnhvw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jeutzzme.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zlstesfs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yiwgvxkm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zgzwmthx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qdzrwcbw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qnqucfoi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ddprgcva.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ihvhclro.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3wvowffuv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bvkzivic.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3kzkdzusx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3pnlewvea.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3iqvsaxhu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3gmdeebji.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3orkrmxfi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3yonmohoi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ecvtllnn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3djjlcicj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwvougqr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jprxgbug.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uxecqsvu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3xxnzkequ.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3fefolatq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3qokpjisv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdilxppx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3magwdwra.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pojrowwg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dyqqrbmo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jwnlopuq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ojeuvxfo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3icfdjysz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ryxlerce.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ezwitlhm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rwgckone.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kipdmywu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3hqooxvxm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ljxggifz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3xfhtatrp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3erywhwfr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tvdwegvm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qfeajmtj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3befmjmls.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zsaebiyx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ltpqjqtj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3lgefkold.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3evxysaoe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nigjekfh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ydpwkpvh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3eqmzixhg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mymxnrya.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3etacfrfj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3moehiytm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ycfjwspd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ghlefnyi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3vlbggpqg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hyouiqhe.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bpoldcpy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3powpbhno.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3bfcrkgxn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3letwtpnb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tvmcxwyw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3dyjeqcdd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mxappvwo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ipagvazu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jfhrkcdb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jefgyqeo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3byijmzkx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hwkjtsav.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3heejnyaa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qkmbhxxo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3bzffyjsi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ncptshod.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ahvbmipu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rfdjbcvf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhdejxdv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3vaqifwtu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ycwwbnde.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3flyoujyu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3duprbtni.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vafxzomt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3qteroztp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3izypgldw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3plmoaazd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aaucieui.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3roxqlzik.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hpokcifa.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3fxelzuso.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vsqwwmzs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gbfrpsvl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zrdithef.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3rtcryamo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3fktsuqpr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3frqofepj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3szvzloet.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3huzexzti.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3terqdmpd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3whubntrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omszgukj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ljfweukc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmygauyu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wcwlzjlj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jmfwzfmq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gicjhqch.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3doofhcoo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3yzqmocem.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ewmulbit.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3pcbxdzbh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cypydemt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3wwljiuln.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3apxxvyux.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3autvtukw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3cjdilcrf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hxccymnn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lshnnsrj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3lqtafqyk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3kydveioo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdyafuu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3mjwskiqp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3btksuftu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3exndtjzk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zdizjygh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dzghvbcl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sbjkijyf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3swmhbain.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xqywvnhu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3eldyhdlm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wjzfnphc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nhnhyrhh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rvhqzxtt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zlsyvele.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mojioaji.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3dhmqoams.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3szdkaied.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3yzhgzmrk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ctdlqlsz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3wzohxatl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ckrxoewx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jzesxkir.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3erowyubs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fjyfelbv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3tmmrlrcx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3puntjtpk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3beitvttw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3snvhgubu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cdoxpkkx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pcsrzunv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cirogxki.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3teeubkvj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wvfpodhl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qwiqbwkj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3brpfcixv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nreomdak.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ikfynjlq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xvnrxptr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3giabopru.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3snosqyqp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oocjtecc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dkoaaspj.html


<!-- 参考信息 -->