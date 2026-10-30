代发 wailian999

[B09] break 与 continue
来源：http://blog.fanxiaobao.xyz/Article/details/gmjmlwpwf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fanxiaobao.xyz/Article/details/gjjvcjyht.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghfhvdzjn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gamfddgvv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwzblmkvr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghfljnsje.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/gicisulnw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fanxiaobao.xyz/Article/details/gakvmjpho.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gibrkqauh.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gvovrithc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrqrsgxq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzcqqpag.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/grypryovm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyshstvfe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glgtlwtbi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhiiftal.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayxwzxut.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giutoclqg.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fanxiaobao.xyz/Article/details/grudmjpgk.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiattrbd.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/ghlfdkxxt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/ghcgbctkt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gelfxmohd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gjpniaawz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrzlzqbh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gedxfznsi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/ggooccgxk.sHtML

[B12] 跳出多层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gxkfjsrej.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fanxiaobao.xyz/Article/details/gddgggxbk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fanxiaobao.xyz/Article/details/gjqfakdfj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuiohngx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gqsiaqstj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfbvlcpu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhgytosi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzqbhncu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fanxiaobao.xyz/Article/details/ggpnkvtnw.sHtML

[B13] 判断是否为数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gxduekvol.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwmlelaa.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gowxlcodg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtdttcqu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gwuyjfczm.sHtML

Java: x instanceof Number
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyaubrwv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fanxiaobao.xyz/Article/details/glhipzyxq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbipehyyp.sHtML

C#:   x is int or double or decimal
来源：http://3g.fanxiaobao.xyz/Article/details/gyxtslxax.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fanxiaobao.xyz/Article/details/gtnfowzuu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fanxiaobao.xyz/Article/details/gmqhpblei.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwhxfdxj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gbvnvirtd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gygjfjzpz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnghkvgkm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gxaoabdxx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqxcbfer.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gegryhimr.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycndilol.sHtML

Py:   a and b or not c
来源：http://m.share.fanxiaobao.xyz/Article/details/gfykwgoiv.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fanxiaobao.xyz/Article/details/gpvminzwd.sHtML

JS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaylooxu.sHtML

TS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gioncbgww.sHtML

Java: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsedtemi.sHtML

Go:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gsosdouzy.sHtML

Ruby: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazqpnbrp.sHtML

C#:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gnewlepyr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/glqppvciw.sHtML

Py:   if not data: return
来源：http://baike.fanxiaobao.xyz/Article/details/gzoxezhgq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmikdcuul.sHtML

JS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gedjywqxc.sHtML

TS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcfmglpb.sHtML

Java: if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gtmwnhfcs.sHtML

Go:   if data == nil { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqccitte.sHtML

Ruby: return if data.nil?
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvvdtigp.sHtML

C#:   if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gabdlqefa.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gydpsbbiu.sHtML

C. 函数与作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/godgkjcsn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtjlvjocn.sHtML

[C01] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gabyawcmm.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpnwaucs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goulwimeh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhnucmbz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gscuekwil.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/grypsbxrk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gtedlpvnp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjzslexf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gakbvowtu.sHtML

[C02] 默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glohyznkj.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fanxiaobao.xyz/Article/details/gbejmdled.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gliyplbmf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyihbtoj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghehaxblm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fanxiaobao.xyz/Article/details/gghggmtnt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuvtpzbs.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fanxiaobao.xyz/Article/details/gworpahdc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclydmjbi.sHtML

[C03] 可变参数
来源：http://3g.fanxiaobao.xyz/Article/details/gbamhbugm.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fanxiaobao.xyz/Article/details/gezvygtnt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fanxiaobao.xyz/Article/details/gornzrmzb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gbxfzwgkn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyfnxzvm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnmjihxn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyitbkzd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnchlarv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgmrmnnk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxirzppn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fanxiaobao.xyz/Article/details/giyhgkzhz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gknipcvzr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gstsfavph.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/grfmdewkc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fanxiaobao.xyz/Article/details/govnrlpwm.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoumygnn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gayvozybo.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gukyopssl.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrfhaczv.sHtML

Py:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/glxvkkumr.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuaotlkg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcykzhmj.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhrvtpcm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fanxiaobao.xyz/Article/details/gmtpzygfg.sHtML

Go:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntdakcoi.sHtML

Ruby: return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwuowtou.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fanxiaobao.xyz/Article/details/guwezuccn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhkdagxd.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fanxiaobao.xyz/Article/details/gzsxgzxbw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gsuwyrvud.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkwhhvgu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gepznhxik.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gltsazieh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gkyckbiom.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/glrlpgyuv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxkdbdvu.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fanxiaobao.xyz/Article/details/gtaqajkfe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fanxiaobao.xyz/Article/details/gejjnpoyg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyiciqhh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fanxiaobao.xyz/Article/details/goadtonjb.sHtML

TS:   arr.map(String)
来源：http://baike.fanxiaobao.xyz/Article/details/gyksrxxcg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gihullrqo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fanxiaobao.xyz/Article/details/ggizrmvfc.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgfkxxbw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fanxiaobao.xyz/Article/details/gezczbffz.sHtML

[C08] 闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnuehjjb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcyjgluc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfbeyqjjo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpokansd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghswltysx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fanxiaobao.xyz/Article/details/gsxpgtaaf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fanxiaobao.xyz/Article/details/gppjbwnas.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fanxiaobao.xyz/Article/details/giychkilc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvymhldsf.sHtML

[C09] 递归
来源：http://blog.fanxiaobao.xyz/Article/details/gthyzcsms.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fanxiaobao.xyz/Article/details/glhwggirf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszksfbgk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gysmcatrq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnfduxhe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gsdcvhbgo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gizywpozv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/goajamgcp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfejqkhbw.sHtML

[C10] 变量作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gxeudsfwq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fanxiaobao.xyz/Article/details/gianyyqnn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjlzxosx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwublliph.sHtML

TS:   同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/ggszpqffo.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujqzemnd.sHtML

Go:   花括号块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gaslssajh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fanxiaobao.xyz/Article/details/gemlkzjwu.sHtML

C#:   块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/grhqwhmjw.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzlrwasj.sHtML

Py:   from module import func
来源：http://baike.fanxiaobao.xyz/Article/details/gngzesdyp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fanxiaobao.xyz/Article/details/gbapgpsce.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpyqgoaz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fanxiaobao.xyz/Article/details/gjdrwihhl.sHtML

Java: import java.util.List;
来源：http://baike.fanxiaobao.xyz/Article/details/grkekmvjl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fanxiaobao.xyz/Article/details/gmzshhmgs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyoklash.sHtML

C#:   using System.Text;
来源：http://www.share.fanxiaobao.xyz/Article/details/gunmcmbqq.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fanxiaobao.xyz/Article/details/glkgesovp.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwymvpujo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fanxiaobao.xyz/Article/details/galekfpif.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/gzmoexfsf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtdxnphi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fanxiaobao.xyz/Article/details/gpmstwkpd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fanxiaobao.xyz/Article/details/gjoxaabss.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fanxiaobao.xyz/Article/details/gbioqmuuc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpacyiatf.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveuujxvf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiodrwwc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goarvvjme.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fanxiaobao.xyz/Article/details/gthbnrslw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gamjdaths.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gizxlbqkl.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkjzlrkv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/ginwrkjdi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fanxiaobao.xyz/Article/details/glkzruyxf.sHtML

[C14] 泛型函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejnouzrp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/glzbfsryr.sHtML

PHP:  // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghowmfzq.sHtML

JS:   // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzrwgnbo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbbtqmcfe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzvnvwxu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fanxiaobao.xyz/Article/details/gdsubyzht.sHtML

Ruby: # 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdvsflij.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fanxiaobao.xyz/Article/details/gaqbgjlug.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgpzodli.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fanxiaobao.xyz/Article/details/guipuufjq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacuqbtce.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxzgcboo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbhlkbum.sHtML

Java: // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/glqddbisp.sHtML

Go:   // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiiqbkpc.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwvtxiaw.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvpktjjb.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfmjafyc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gagkgdbmk.sHtML

PHP:  // 无重载
来源：http://wap.fanxiaobao.xyz/Article/details/gqcvvctgd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/gxnuvmqtk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gfewdyhul.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gpqxcvtyc.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fanxiaobao.xyz/Article/details/gtnsdlwog.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giitzrety.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gublceity.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grmahtodn.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fanxiaobao.xyz/Article/details/gvunatesm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkjrqnaz.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gfmslgicq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fanxiaobao.xyz/Article/details/gmqnzxwza.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gudsrjgbm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlzwmnet.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkttknza.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcizzicsi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fanxiaobao.xyz/Article/details/gwhwmgevb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbhpojzn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmkikrlf.sHtML

[D02] 追加元素到末尾
来源：http://baike.fanxiaobao.xyz/Article/details/gzufhodtv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fanxiaobao.xyz/Article/details/geahpkhxu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/grfepycht.sHtML

JS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/galfgrlns.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gwmylagij.sHtML

Java: list.add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gofehrljk.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/grvsrlswc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjohquwo.sHtML

C#:   list.Add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/grzbmhcfz.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzslmksx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmpidikb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggegrlakw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fanxiaobao.xyz/Article/details/gcfgllrnz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/ghgyqvstt.sHtML

Java: list.add(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/guceropho.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvqnttgf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gypvpxwnq.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/ghozyzlcy.sHtML

[D04] 删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gygwssdct.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gktkdsjoy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gonfhqahh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fanxiaobao.xyz/Article/details/gaueonuku.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpitvyfii.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgryoejh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fanxiaobao.xyz/Article/details/geupkymul.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwoqcdku.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fanxiaobao.xyz/Article/details/grngwovan.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqsbkrqa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gobbsnnmo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gvuwzppwq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznzlpzcf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fanxiaobao.xyz/Article/details/geemoqreb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfwyyqqd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/ghohjeaqz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqtfxjxe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmfrxrjk.sHtML

[D06] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjiffsgb.sHtML

Py:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/grmaxdmjm.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gflrmvrsb.sHtML

JS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/gmxpsqylq.sHtML

TS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gxojijnek.sHtML

Java: list.size();
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyikciax.sHtML

Go:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgpaomtv.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/gfyatfyng.sHtML

C#:   list.Count;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyemssmhz.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fanxiaobao.xyz/Article/details/gzkdjlcmp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlodkgwo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/grmmfmazr.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gaoerhsma.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/guqlpwurx.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhuiszaa.sHtML

Go:   arr[1:4]
来源：http://www.share.fanxiaobao.xyz/Article/details/gamvucbkk.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gxynzdgxx.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gawaqzclk.sHtML

[D08] 合并两个数组
来源：http://baike.fanxiaobao.xyz/Article/details/gidvzzelj.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhibslug.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/gcswahfat.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyepmzrvg.sHtML

TS:   [...a, ...b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyzvrqzv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gqehspkhp.sHtML

Go:   append(a, b...)
来源：http://www.share.fanxiaobao.xyz/Article/details/goejlradu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkncbefis.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjiuuiar.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnbvjese.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpukggpl.sHtML

PHP:  sort($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gucempmqw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fanxiaobao.xyz/Article/details/geendtmva.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fanxiaobao.xyz/Article/details/gipqrbidx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fanxiaobao.xyz/Article/details/gwcyxtulw.sHtML


<!-- 参考信息 -->