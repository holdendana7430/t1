代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ctygfndz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3phlpeusd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jvztxgoq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3wilcyqkh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3knmwmcmu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3kktcsvxs.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ocdtcuyd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3tskmvltc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wsbiwbkf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3blopzbhs.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqvvczsj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3svngwctm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3oubonlgh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ymrgfics.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ssjnipme.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3qkxunkze.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3clypaapf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ypfdqdbe.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vonpkmzf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kgyzsxgp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tmvdjkcm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wugbzfci.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3mppoxyyd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qidgnptk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3aismjzyj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3napxmfyn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvnsfaye.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3exvktggj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nvgcvhdl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rmhbdeok.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rweiunic.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gxigzrwt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vwodaydq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3hgaiywgr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3odfkhmrz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3scuvesur.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qbynxzol.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vemtcxzd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3puytigfe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cebodnyf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3erggyapw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3czfmxevh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3yjktosla.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3olgrcltb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kziujjbp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3amepolzn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qfwxdpfs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3munpqgxi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3cjejrdat.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3jrtnpkmc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nmyvsxlh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3upzniqlr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3nonmlggq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3lpdlngpk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hrtbhslg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jbhgiviv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vgtvklcl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3vupgnwqn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kztyyztv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3wdkooahi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cetcxtby.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3zbuhuznf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmqnuabd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bhbqbzaz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kjeqqltr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3tpchihhq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3qxhwsavl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tzduqqwr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3cyywtnvr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3cuzesqwb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3mrafawmo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3qtdxyuiy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qdpdnrek.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzrswyyh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bnthxuwy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ydopqwcp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dzhyvfym.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jhkdilca.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3capqgfvx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lyyiddzi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kcbnijbn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nhfmbjfd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3htorzrqd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eozuxcjp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eubeakgm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3itmrbkms.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dphzbvfh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hdhbrdfj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kbbenjlg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3nysxwnoi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3keahrbio.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jnfpmuwu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hrdeaahd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3rrrswxqx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kgigolrr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gxaasjsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxcltpwq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3rmemjort.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lapvldts.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zfzvbhvs.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rqxkowey.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nikwvgwm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhuubpvl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcnfhmqw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttlmxuns.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3eimavced.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jszfoebo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtlhtayd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3kdsrnjfs.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3owvbauzv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3dlfxhrbe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3toaklmew.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3twxssuet.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3neplsozq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3jnnqiesr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zkhiuxzm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bokfwwei.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wyevtiyo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3vajmjdxf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3kurrsukq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xnpeevmx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3geqtoyoj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fefzfcsa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3madbansh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3zwrbagmo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3yytoiwah.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ppkwospi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jaxbtmlx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3kbfxpmbc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dyzrabav.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3peuyzmag.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nkmpjoew.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lrcvpogr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wszteajc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rsijrjdi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wjygnofy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wcfxzbgy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3kswcjdvw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uugvuqza.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wrnzvjsr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3wnkgmsrh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fnrclwez.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3jmqetykv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3enaotzvv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ynakbkqo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3jehermrn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3brupksgd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3psmpagbl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fhdtxalt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3onveakvh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nunqtnbd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3amyfvdde.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mngmmacs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3czrcvhgw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3reyrqcqu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vmvsuhzh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3fejsvyhy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3relgebdk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bzfbaphc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3dzexckje.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3nmtkijur.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ompzygmw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vgewqrjv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3guwqnfmx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytchwbwy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdnahzjd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukkkejgs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pxwlsymj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qnmrukgq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3hhomjlpi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3inylliyv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3jcwvyzdo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3grdgvbbz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xbakfzvf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bbmvebst.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ofkeuoxt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3odjbavrz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xksdcbvb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3epddnklh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3bmzxuqyd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ugfhxfvm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3cltyssmc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3irfcjmth.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tybimskm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nyhtstzl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3glozvvyr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pspskebe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3gyobvsci.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wliuzowh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ronkqiuf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3tdcetezi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mewalith.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hasjimyb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zcuxiemb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fclpotba.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3eeajtcpw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ioepwtdg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3maexhxjw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3oldoeehr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3sgqwbfoy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3cdmfysgp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ftymbkmq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rqrtrzwa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ojcjwkxb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3esixafxp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3qpjmzmmb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sqpwyqwz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3oruwyyva.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tcpqsdca.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3knvrycok.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3lroypfgk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uneyxbfy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fvfaxwry.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3rvywromm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3eugouvqc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3wrjilmae.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ijmprvic.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3atfxoycm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3eppjxhgf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ksdbspys.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3przsqlpv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzihosdw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vijptpcw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3horalffi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tafxigwj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3yysgydkq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3pndajtwy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3vbqszvaq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqiqcqrg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3zbqfcdeb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gnbafsiw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cgtjcpug.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xnemhfli.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3jidadxcf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3mtaifpzm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3qbkbgqmz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3cxlrwswh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3rnrxocgk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3qcxxzwcl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3zlzecrti.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3yutcgkxs.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3wcijkqnj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ltbdykkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivguihvx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ficgtxbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eiqjqliu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yskfgvom.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3rjodniqb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uhrytxlh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3avrunlyp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fjbwnwgb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3lmszxagh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3iwxhqriv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dwearexl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3oquitgeg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ktllrsdf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3pekepzxm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3scgosdie.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3onmyarnq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mkzqaztl.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3jmbubtas.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3rshlcool.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3kmgcuzyy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ckvcsjpq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hnknntpt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zrrnfaoj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bwteylzd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ilorzcem.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3abpyswkj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gzcyuufs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3umiosskp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3nvwdntqk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vekldcpu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3nskgknaq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3asnjefpf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bdbvvhpz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vsdjpfoy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3drlcpall.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3umzognta.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3oxpidksa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ugxicaab.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ezfywaky.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hgeolueh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qgmeknvw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ipraswcj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ytvlbvxp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ltqrgiwl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3zjkbvedj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yrefklfr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xjbedqpp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ymfeyaoc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rdytzfxv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ugrqlyym.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xiseaqpt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ttwfklcr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bjerersw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3cextbzqc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnfvkly.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3whtsiskb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gbdotwxh.html


<!-- 参考信息 -->