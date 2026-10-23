代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cwgjfrnc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhdvpclh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3sgnookhj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xopvzczs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3scoocsgb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3kytlsrib.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3bfayhcvi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3uumxvhge.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bhhuvoss.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tpjquyhs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3inshlwjb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qtnqoysm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3nqxfkpti.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ziihnrep.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3geuwyynd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3gabhvdsd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqztmghi.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bmvfibjf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uucwmjfc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoulyqqp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3phlefnhf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hhzrtoxs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cmjvkphy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3fahcwzyf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3hwazsfax.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kerbuvuh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3evocnajv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uarekmkq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ngdwztfy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wvfnkkgw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3mwbpfnhn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vbppiisk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3vmraaqcg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ngldhcpa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofoklvap.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3owvxhugn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqqfdxoe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3assxexpk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3khlvoapj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3vvlunurh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xfzcajsz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ikdpqvgp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zxkvmfpk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3kxszxgnv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dwfnycws.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ilzxajrb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3raqptlqu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3iqqumepm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3qjihgwft.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gumjjtut.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qlzwpaob.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3psklsygv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3swvmncgu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wgmjyjhq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3toyyahpf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fyzjbbzd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3dolohtul.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yfmcajdu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qsepibjz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3hpcwmsfn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3uraatsgy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3adiplgro.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nmcwuhbe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qpaeufyk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mazhhbjq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3cidtntmm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zbxmseqe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bcsutrua.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3frdsrvxx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3iybmsjdr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bkxircbm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mjpgxata.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bejxfazn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ajejaomj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lncxsulv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3pvepvyrh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jtovyhtv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3qxoifrlu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ysesebwe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3jwrmfukg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xzfmnwhl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3omtiadgy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3byucfqti.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3lahutyak.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vzcaeejn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mgnliamp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lmwwphof.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3okxamsgd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3qofojyel.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qhvnslvl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3igopqxnu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jxedocvt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ojpixixp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yltzpele.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3injcxqpj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3lufxypjx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3crplewoi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuocbhlq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3eozaatoz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jnjsubcj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bzsbffaf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gnxtgrvh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ipgencne.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3podnbtyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znwcpion.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jwyeokaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evttdbxl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kdzyepqw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3prskvgvf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3slhuhddr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjeogvby.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iacdmwex.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3boqvieka.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kjobsijp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ehcleuoj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhdvsqgl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3eispgbhd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3cryycasn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrpupbzm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3osgjnulm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3skjiadpp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zlsdaqil.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jrpyxoif.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3juqayfuk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3uolkrfvc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3thsciuff.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ngnfwsxm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuyfilou.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggvapcbv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xiykgago.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysuyjtsr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3vkjclwtx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dzoiqimj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3colecimn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3lrjsfhnr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3vjjeeact.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3sqavekdv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3inaorvpg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ozdzjgds.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vczhwmey.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3mrhqwyqy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gjyfvxcv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3beyjudje.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3pulxttbi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gyjtqjrt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xohyjqjo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gbqxnjsp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hsvooeso.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3btkabidr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3foygocfh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3uhdpykhn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ssqrjdzt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3rsnaqhvz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3njegywlh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3hlyyfcfp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uoefjdya.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uekhurbb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vslpqkbk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rnxyinze.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3oeaozloe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nkoxrxil.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3sltxqdbl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qgifmyry.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3oqalcqqb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3twakyurc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3iexvqozd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ccekpdxj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ddoxstir.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hjjuissa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3tyygiess.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ujlilxdr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tchdinvx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvuttrsy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ntsxxsmi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wlgntxkv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3uahltskv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3exbhqfal.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jrxrondk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgkhgnfc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3krjmxnbp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qjrfapdn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfdjqcke.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3uqbvvhga.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kidchamz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltrzrqzq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fniyivmo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cplfzjzi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3kmekrujc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fgesaeop.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wkumzjht.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3uokbzrgr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ebkxbdec.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3drelurxv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wfpvurvx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jomejrbd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3avbpybuf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3awcxfbji.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3iqypvkbw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3knmxouev.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hsnqnety.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ebzmgxwy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zumlvgtj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ezldsszs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dwgqmivi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rowfjeyy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3hmhkwzpy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wfzycbzc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3unrvyeqg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3uudnatcy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xyzepoqd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wzzaboyr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3iqwckqsb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3jyctboib.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3bxejqfib.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3whxlwkpl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3aootpwuh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iwlchtmz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zuebdxws.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3kqeezmnb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3njiyxhul.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqgewycp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zkirnnsf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3tulynnhp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3khhsgbiw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjgljaau.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3udgjqeqp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3udonyxsi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ynbcxiuo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wadlfndi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgpkzdcp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3etbclqks.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jffdqitk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3irsyeczn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3gwjydefq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3pnjpdqma.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hfeqtunx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zsudtvht.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xvvwgpbo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3txjfyxxg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3onapyljl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hrqruiip.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rgoyvkar.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3lczatmsw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3equyxcgi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fauumakx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wmrhajty.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3clbwbept.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivfrdyat.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3njqzgmtp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3erbxhuli.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rispmkxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3paqouafb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3kfoaykft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzechlpa.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pbdavocv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gjkflfgb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mymtwrfy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3immnrbjn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3xvdvnevi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fuzpfdex.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3teqviizn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3izeizwwv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3aalxeyiz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ppbbdseo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3eehzqmoi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vxybogdi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lznfjjwl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3terttobg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kdzqgdce.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jtkyugmj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3gozpctbp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jvcmmtfw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3uezqhics.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jurcemyf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3wgmyzvou.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lkudvyci.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wmuqvuds.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mlawvcut.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cfjrrrlx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3gehqfodz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yupugjtt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lanifzrv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3aqtokxau.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3bzlzulup.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3bpngjbyt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cfofzmdk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wyzjtfiv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3joteopnb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qkoamkxd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3wmxotycw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3tvokxtpk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3arcgsgrs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xzzjxxdg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wpmebtzj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vkbnkfgo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3eqrvldxt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zvidnrtf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nbkzjflj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3orifvzfv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ulxjegrw.html


<!-- 参考信息 -->