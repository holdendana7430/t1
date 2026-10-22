代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oomqnnje.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qqhkdjzv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2gzljaatb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2wcfqbwao.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuhqetmu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqcwfakl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2oybnqiqf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2cmjjfxtu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kspjhmsc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ennuktza.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ytfsjknq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2dykxcdrk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2mofxvlov.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eotvabna.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2magoygfx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gvcaatos.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ribumewi.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2viljokul.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhhjeggo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ycqaquzn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ioocxbmp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ixnhuyiw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nttcwdqi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mswillrs.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fqgfoziy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pnwsclwt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2dsdmdjtg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eotrebro.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ieewxefp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2lbwxqgox.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gzdjjyem.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iwtgbbxw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cjuwspzj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqaulqup.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cpwgprom.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2elssymuw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oxwwlmtr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qyhaewxt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2knsiiqkw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2qpwqwipl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ihasgjss.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2muriyajr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ldpwthxb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pmflcncw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dqfnnnyu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2miioryeu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2pcckswtf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2zfymjgca.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yrwhjidm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nzgeohcf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rutfzwwj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uhazaian.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2okitjomr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mucdmnsp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2zwortkvy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2emibfzjs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qhlnbmml.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zymxwkvc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hgmufliv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xrnfbgzp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zgulfqgf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2clscgoqy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2zyzxqmnf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2afiuanfa.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zdtphila.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2fzletdzj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bizgalam.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rjbzqzid.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czhqqdxy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gnmatrjn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2txzbvjtu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gmuwrbcj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vafofqvx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qlwigrnr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2pnmlierr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2mlcvmnos.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmmrxcfi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xlazjijy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oksuikcs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2refgntrp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2onvinypl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uajiqgza.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2amvtcxbo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2eeaelsme.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fgzxispk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lufccztb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rruilakt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wqzxasjv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sofnsxhm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gblnnfzd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qawhucqh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2oacchbty.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2inhncgka.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2pxvknene.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qhmmhdsq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2krnpbiao.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2uwdqndhc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2knrwjdbb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2tzpoptcf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wmxfvall.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjlkoutg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eftyqfdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcalipzi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vhcstfwv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lxrfoefn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqnvrkrc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ytyymbzz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xzekoczj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozigupur.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2azlntlkq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tpdlbhah.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwaavswo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2nasjmxzh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2gsbszejf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zczsgenz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2drpzsprd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lullfmqn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kvffgadh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2stleowow.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2dglalexz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2bfjtlesg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2labjwjtt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vagfspem.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kizsoqdd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqvbdnqn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2tvhquxrj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2juuipjky.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2lwzccbdi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2dydgeaob.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2yvpixqoa.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2xforznxf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2enyqldxn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2nqqixfjs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jazuchqi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2igzqrmji.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2tcefqfgt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nirpbghc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rlqyvxhl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gbtbxlld.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2arszsdfu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pmvctrxr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ezdsocgt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2aywgzqht.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2liqlevsk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2qbaldatt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ivgmcxkn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2krqcgoac.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2grotrtmz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jkctgsle.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ahcizmwz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2nzspudyc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zoimnemy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ucaljgtz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qtojmcqc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2nunnhukf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uilmyctp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dnvoyhdo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2faqulgdm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2mtqjllmi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ppmoiuio.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hduaiknc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2lynnnhvd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2euuxtrze.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xftpvilt.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vckydpxs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xomzvlbi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2xfamxoch.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gjyvcrry.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzjhepgr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rszmymof.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yktavuqw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2txwgmsfr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ghsskvcs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2emwjaywk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2izasgufd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2rnlzwmrz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uayknlum.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uegesroy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zxqgjkyk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lmqzzsxy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcoxbxtr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2waejxqot.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2szucetzp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ggeigalo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iipyatow.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2zciouxlk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ydwnhhry.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wvuafaqm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2knsbjbak.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pboolezc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zlaldysl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zypblwua.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2juuuwqkk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ffoqszfl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2nrhmgoft.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2iwkxmiro.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pfvptevi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xsxbemhm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2lusbpkxv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2cvstadxn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2duxnzbsw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2dddrvego.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2tmvnrkdy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2yylhcnhu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2saqzxqam.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dgffefbh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2aoceusdm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rnifbqcv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2kcgrjcrt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tcikunwc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fxflijnc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2tvduiugz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rshssnfh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pgeoktyt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2swnomhdb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxqutgsz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkdrsqcr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nepmcxyt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cclqsenb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2fdnwlgke.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2slqxfkeh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pmacjspo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2snxdxkfe.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iibgdnse.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dqudblow.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2bbicstst.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mujmmwqd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2azxaxbeu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2vmybhump.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wfgjvpmx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2jqewpjyo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2genxsxfd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pxrclmia.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2dqlwvjmv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dnoqbrur.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pzruitpm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2tkettnum.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cxwwkewi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2eibppxru.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2abucumhz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2uilfoebq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vqlcmsot.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hxhnyulw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2gqeqysym.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2sajfqudi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xagxxnkn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kljyalpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uijcvupq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qggvrqkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tplxwxfl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wjgblyne.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2lqqdanjj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2umtmicns.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2agapmafn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2iughbuot.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ilzlxynr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2pjhkyhmd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pclbigmy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ntonilde.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hlpoeekj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2babutokj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2odeeoplo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rowssqii.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vzbwbjtu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lknxkqew.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2uzymcyno.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2yckajjxq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2cvpmlbnr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qyotltbu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2apijvsrn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2mgnyaxpa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2lenktvkn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nxycfjxp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lqaenofc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uxslidth.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ochhviyw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hgvqvsel.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yklmtmfd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2elhabbhr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ajpiqnzp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kpvpqncf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tufvlyvs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fxpcfcuu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2soegchip.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nfzgxcip.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ohneepvw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2itwnorto.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xqojrmcl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nlbjhzwy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hqfjwmzl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tohjxxdu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2myfgblku.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gxlibdtz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ungapmmj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zanvwfpy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vegieesa.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tbprdddo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xauqfltb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2njpqdhrp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hkbzotzh.html


<!-- 参考信息 -->