代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhtdtgnr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3msgqqycn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qdbtwuvi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3cfhiomyk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3jnzfhope.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljgmknfx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3qfxqgsli.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zpssmchx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3gssurogj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rexztwvn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqfiksvj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3puoltvfe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3yliibqfm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ojyiabrh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjvepdha.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3oraxtjmz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3wvukapmm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rdyiymug.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hjhmrdyt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eglvdopc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wgudehoe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3votmezld.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3olhhzwtu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rnexfvdz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jyuayxjj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3fozzxlvx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lghfjrug.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ieohpecr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nigtmqng.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zfalcexh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lbgdistz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3cacrbnrl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mtgozqzl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3rwylazli.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3tiwyjocd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3dhpluort.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kfxtwmhw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ljeztfwl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bavkpdhh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3cpxvswsd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ktgpsnjo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnythsbs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pjrtysqq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3kvctkwwm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3myqtgggo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3douxxyrf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uzgjruql.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3nddopgqv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3smncxrrh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3jmoqrdof.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3cvorluzh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ypfyywnm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3cpevlejm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gyncmbmt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pwgfmvbq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3brtbdnxs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cjvttaqx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3lzfmlnmy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ikobbpcj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3sgbetver.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jjblfawp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3nxugjbvz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3lpgxhwxu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkvynxpp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3avatpoum.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mggduixt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3wttelygs.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3nwqsraol.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vmhybdsq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xljlqksx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3dvejgxdr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xttfusha.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uzvyavlx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmtnumxe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3owstilbl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tumuimmw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bukapdhd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xeuyzjdf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qwgluwvr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3uuflnkni.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3msiepayp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uzpcexln.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lmnltcvd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gxvvqblr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kamkscmp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jyhilurg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jpxgkhdg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xabdaeia.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3rfrhxypd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hstrchsr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3aqumueph.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qtqnzqva.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vleairxs.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pikkddzv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3bmtnfkbq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vcefgeyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjpysaac.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xyegeyxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhafnftu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jdmjnehz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3teurrmtd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3djfotjys.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyalriib.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pmtivpvs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3inrdnwcl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xxpwtsjg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3imzechqt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbtzhvvn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kzdexbjw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3pjmhviva.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3yrpddfce.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3reegzhhx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3olbawjst.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3eusbjtde.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3eknkwlsp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3fawdajox.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3jnomkjzi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qbjckltj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3fyfrhlwm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ysijzbvo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3eohfzzmc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xndkhfun.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gbvehzos.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fuaoydnl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ztedoxwv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3snghrisx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3okkytjfq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3otdgsngz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3lpoxrwkr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3safxconm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dljkckma.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3iixckzji.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3eypfetpc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gkbchirr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujkchjpp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3npiieymr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pxkaxhst.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3sqoosaay.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xlcmfmxv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rvwcqspo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ofpzevuv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3efwtzcgk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3brbcefnr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3oprjcohc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hzobavau.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3mkimumwr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3lkgiypmc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hlvgxaee.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lefxkrog.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3mifibyiv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jgyhcuxs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rnzuyetd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3odydhdvc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3avlfygbs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3zuxojkbg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yhqkyjev.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rbritatp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3qanihfmc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3uezsxmuj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3uktgdjca.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3grujmmku.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3eqqhoyfg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3joiwiyln.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3yriixjgm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3izdblyhf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kilrltbx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cuxmqdrn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3afprjqxf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jqxqtdzb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3vvxkliqf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mapzslll.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3uezyarkw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3naepdhcq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffykzyqk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dhsaocqf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ifohzxcs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qkjcjnsj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3zbwwubhh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vdxxqstt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rirjount.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gmjkaqdp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3rkhosxog.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3egsfltya.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zsivxcrx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3qmxdhojf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wotofrog.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fzuaanfg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3krvgprcm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lfokjzie.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ynnxktyt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3tqahzzws.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pojprbmk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cizkfxqd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hswyupup.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3omnpadhz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3aipgzdpz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3drqmehbc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3slqfzvyy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3nfxbwztt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3svvsjnse.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ihfvrefu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3idrhygmi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nvuihxjl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3vieycuud.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3drefxunm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3cuxyvntf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3oszjfmgt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3grgsiasz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3rqmyuwgf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lafzoeyr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3udvrihyw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdtkjqqy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3otlammgv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3chmgxubf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3cpuzwsnc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3yavbzpkg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3evebcais.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hlbfeenf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tdwlmifs.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3enxppmtv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgfpsuyi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3pzpbyaaw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mwueucly.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kpewqlwk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3xkuvkmtm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fclskpbu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hxknkoxu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ghhghtjy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3sqkgutve.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lmflwfqc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pmrvluru.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dcxhyxkg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3yxeipjgh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dvgejyfr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wkjgnqfy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vzdjpzhx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xdhsozjs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3kkaxmics.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jqjuevpx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmjtqfzg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gpbbrduq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qxukbqai.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3juzghvpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkjisexz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3bwlbecsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmciisdc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mvqqzwow.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3qjzppuqk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fhzniqgv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bdtmuqot.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3sskhbfwx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3eickuekr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ynfjcwky.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qtpxrrgv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nhhjqkkw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3travsqmu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qladuzif.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ekngbmpp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nlycngym.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uvjzbdix.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ywaeosfx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jvzfsjpa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ahaslfmr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ywnmvfmw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3bwcqeigp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vqoonjfe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bvqecpzi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3zkcyxice.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hmcqzjpe.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hfewuxpu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tncetoyj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xspycttw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3alxofkjr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jrpzdwro.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mqoknpaf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3wdontwum.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3gihijsyi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3byhlyxqk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hegnjiqp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xcdhzied.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qbwgdubc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vjtujnho.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ectfshet.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zjtwhnay.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nruuigor.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uxoqhssb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3rrihezfb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wehqwppn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lsayvwad.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hojwosqp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3edyphsix.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bnpziuhx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3itpqtvkx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dlyprwgs.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3eraqusiu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ljzwelxn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3moqrfwxl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3muhtyqeq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yhyhgnij.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3svnlaycc.html


<!-- 参考信息 -->