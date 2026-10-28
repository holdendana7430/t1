代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.ivvv.top/gtioqsbmkm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.andypj.xyz/gtmlfojzze.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.c1oappe.top/gthyczapnf.html

Ruby: arr.each { |item| puts item }
来源：http://hz.tianlin.xyz/gtexcdwwua.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.tian-w.cn/gtscwsrleg.html

[B06] 遍历字典 / 对象
来源：http://hz.nanxuanxn.top/gtaezoipso.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.haohaochexian.top/gtwnfcmhdt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinqigfzy.top/gtrjcbnzcq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhongyouzk.top/gtdifbwdng.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.snrcjt.cn/gtqdluiusc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yj20258888.top/gtjjbybwkj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.daria6918.cn/gtmenpplqt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jinqigfzy.top/gtoihosuzl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yvedp.cn/gtsedhvkhq.html

[B07] while 循环
来源：http://hz.0kj1m.cn/gtknjwrivu.html

Py:   while i < 10: i += 1
来源：http://hz.xinyue.icu/gtndotmqxq.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ydzc1.top/gtpkntvrwl.html

JS:   while (i < 10) { i++; }
来源：http://hz.hammf.cn/gtijrebwmf.html

TS:   while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gtvecppgke.html

Java: while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gtnnrilqjl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.chenzaomai.com/gtimezgxna.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yj20258888.top/gtkqjvpbng.html

C#:   while (i < 10) { i++; }
来源：http://hz.ivvv.top/gtuwshtjgh.html

[B08] do-while（至少执行一次）
来源：http://hz.c1oappe.top/gtsztiocmw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.wangshuangyany.cn/gtynzquwgp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.guannengcc.top/gtbysfbuvw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hongshengwenyu.top/gttetbuunl.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gtdhkqdttc.html

Java: do { i++; } while (i < 10);
来源：http://hz.c1oappe.top/gtuafyhzub.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.nanxuanxn.top/gtzmprnyiw.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jianghu66.top/gtbzoqqsjt.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangtech.top/gthbgvejqj.html

[B09] break 与 continue
来源：http://hz.hywenlv.cn/gturgdhjas.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jqgfzy.top/gthsxleead.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.chenjidiqi.icu/gtqqmulqws.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.iojbl.cn/gttcgbksxc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigufen.top/gthqbxihin.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuanzx.com/gtzpchydee.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.andypj.xyz/gtiebdaawj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.sweek.top/gtmdqoevhz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.9152youxi.cn/gtardzvbrv.html

[B10] 遍历同时拿索引
来源：http://hz.ydzc1.top/gtiwpmlwrj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.316326.xyz/gtjwaaoriv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zycfv.cn/gtzlvlndhk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.pycfn.com/gteonmumng.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jlsjyb.cn/gtlwruqsne.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinqigfzy.top/gtthqijgrk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yuxming.cn/gtkdalyxpt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yongpay.top/gtrcqokbty.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinqigfzy.top/gtdyqikknr.html

[B11] 生成数字序列 / 区间
来源：http://hz.xingfuxueyuan.xyz/gtfpqnzhnn.html

Py:   list(range(0, 10, 2))
来源：http://hz.yueranfly.top/gtahqegwea.html

PHP:  range(0, 10, 2);
来源：http://hz.zhongyouzk.top/gtpvzfgmjh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cqqwz.cn/gtycgexjei.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zycfv.cn/gtalzjqkaq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhaomingkeji.xyz/gtkhfckhtc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.nanxuanxn.top/gtyehxxqur.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yangfankeji.com/gtwnkkjxle.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.daxiang520.top/gtxmmgbavx.html

[B12] 跳出多层循环
来源：http://hz.sxryk.cn/gtjylxvcil.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.havefunace.top/gttgepbyrp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.svipenyu.cn/gtanuhhfyw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gtnlnvtlxg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtqhwlkadf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gtnfxhjdvq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shanyushiyangkeji.top/gtuzxmfdiz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jiagoushi.top/gtghsitrmg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yuxming.cn/gtdowbmvia.html

[B13] 判断是否为数字
来源：http://hz.ehwqpu.com/gtuiooojth.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinyuanbaomall.cn/gtxvcrnmwt.html

PHP:  is_numeric($x)
来源：http://hz.zhixingplan.top/gtlubkdsql.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtcihziazb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yuxming.cn/gtfalvpzgw.html

Java: x instanceof Number
来源：http://hz.yuxming.cn/gtigxbhqut.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cqqwz.cn/gtrbjifywi.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nwbrower.top/gtbhxcqchm.html

C#:   x is int or double or decimal
来源：http://hz.chenzaomai.com/gttatcfnus.html

[B14] 判断值是否在集合内
来源：http://hz.wangshuangyany.cn/gthdhmgauh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ivvv.top/gtmvctjgsu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.cqqwz.cn/gtsqttswru.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yueranfly.top/gtnzuzpsxz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xuetiantiany.cn/gtcmgbgbdd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtknqjqfig.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ydzc1.top/gtyzegzpou.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hnqzz.top/gtcgacylin.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.gzhubu.top/gtatqvntun.html

[B15] 布尔运算与取反
来源：http://hz.ydzc1.top/gtkxjtsbzd.html

Py:   a and b or not c
来源：http://hz.bjfxy.top/gtuyblresm.html

PHP:  $a && $b || !$c
来源：http://hz.shanyushiyangtech.top/gtjzrgabfh.html

JS:   a && b || !c
来源：http://hz.jyoumei.cn/gtsgilnnbz.html

TS:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtndprmvix.html

Java: a && b || !c
来源：http://hz.316326.xyz/gttyopzncz.html

Go:   a && b || !c
来源：http://hz.shuidangran.top/gthdkntlab.html

Ruby: a && b || !c
来源：http://hz.xuanzx.com/gtatouqwfj.html

C#:   a && b || !c
来源：http://hz.gzhubu.top/gtcvjnityc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhiwuduotai.top/gtqbbfcdgc.html

Py:   if not data: return
来源：http://hz.xziqi.cn/gtbcmbeyem.html

PHP:  if (!$data) { return; }
来源：http://hz.shangyingyoupin.top/gtmflnugxh.html

JS:   if (!data) return;
来源：http://hz.jinghuilouyu.cn/gtdcncpdlu.html

TS:   if (!data) return;
来源：http://hz.xinyue.icu/gtyfkpgkom.html

Java: if (data == null) return;
来源：http://hz.wangdashe.top/gthrstxcqj.html

Go:   if data == nil { return }
来源：http://hz.jianghu66.top/gttbzryeey.html

Ruby: return if data.nil?
来源：http://hz.cashguo.top/gtjdgislkp.html

C#:   if (data == null) return;
来源：http://hz.jlsjyb.cn/gtduyubsuh.html

================================================================================
来源：http://hz.cqqwz.cn/gthgnezseo.html

C. 函数与作用域
来源：http://hz.yongpay.top/gtpmrwfaxe.html

================================================================================
来源：http://hz.jqgufenzy.top/gtfkyemkss.html

[C01] 定义函数
来源：http://hz.jinqigfzy.top/gtsqpzahgi.html

Py:   def add(a, b): return a + b
来源：http://hz.iojbl.cn/gtxwuqycuu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtvejltbjx.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtzzussnuo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gzhubu.top/gthijjjyng.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtzfpyoqdk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jqgufenzy.top/gtwmtwwaah.html

Ruby: def add(a, b); a + b; end
来源：http://hz.wangdashe.top/gthfdzsqjw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtdhqhxjyq.html

[C02] 默认参数
来源：http://hz.cucudq.cn/gtyhyzipkh.html

Py:   def greet(name="World"): return name
来源：http://hz.pengpengdd.cyou/gthdznlnbq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.pengpengdd.cyou/gtcmxczvgm.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yuxming.cn/gtggakgwnz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinqigufen.top/gtgrvdfken.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jqgfzy.top/gtpixaopwb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hongshengwenyu.top/gtrwcdmksz.html

Ruby: def greet(name = "World") = name
来源：http://hz.xuetiantiany.cn/gtretqrouk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ppjwa.cn/gtcmhqgygj.html

[C03] 可变参数
来源：http://hz.shzxlz.cn/gtsclvebeg.html

Py:   def total(*args): return sum(args)
来源：http://hz.hnqzz.top/gtmiazmdua.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.aizwys.cn/gtkulunjra.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgfzy.top/gtnvevxutt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.vqdsnc.cn/gtrfjhfhxg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hongshengwenyu.top/gtjxmmxetr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinqigufen.top/gtrexscdjb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ppjwa.cn/gtyokeyyxj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.andypj.xyz/gtqugpmijd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.aizwys.cn/gtqxjhuyck.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhengqikj.top/gtvthyabdz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.birdmap.top/gthkyoycih.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hongshengwenyu.top/gtlcnjlraj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xuetiantiany.cn/gtsfsfdmgd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sxryk.cn/gtmyljjfgd.html

Go:   // 无：用配置结构体参数
来源：http://hz.shanyushiyangkeji.top/gtxyihwwbf.html

Ruby: f(a: 1, b: 2)
来源：http://hz.52xcode.cn/gtkjpbsnez.html

C#:   f(a: 1, b: 2)
来源：http://hz.cashguo.top/gtqdjjaixn.html

[C05] 返回多个值
来源：http://hz.svipenyu.cn/gtvwnyhsdy.html

Py:   return a, b
来源：http://hz.nwbrower.top/gtufrsyuyx.html

PHP:  return [$a, $b];
来源：http://hz.jinghuilouyu.cn/gtzuktjgdq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.chenjidiqi.icu/gtqvfukszb.html

TS:   return { a, b };
来源：http://hz.shanyushiyangtech.top/gtsryuuxvf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.dashuyun.cn/gtiucbvbux.html

Go:   return a, b
来源：http://hz.fzhhl.top/gtvcqxitvr.html

Ruby: return a, b
来源：http://hz.daxiang520.top/gtbczqdfct.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ydjk.org.cn/gtddhnpfle.html

[C06] 匿名函数 / lambda
来源：http://hz.hammf.cn/gtyvvgvpks.html

Py:   square = lambda x: x * x
来源：http://hz.jiagoushi.top/gtkarmqzhj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xuetiantiany.cn/gtremexrpv.html

JS:   const square = x => x * x;
来源：http://hz.nwbrower.top/gtadmagliw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xuanzx.com/gtgrjzcumv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gogol.net.cn/gtopbhbrnu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gotoacloud.top/gtqpglvrlf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cashguo.top/gtusutnqzp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yueranfly.top/gthjhbpkez.html

[C07] 把函数作为参数传入
来源：http://hz.chenjidiqi.icu/gtnougxyas.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nanxuanxn.top/gtsrtsgprj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.52xcode.cn/gtlxwdrmzx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yj20258.top/gtgsviubyg.html

TS:   arr.map(String)
来源：http://hz.jianghu66.top/gtzgodgoqt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.tanke756.top/gtfrypojjw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.9152youxi.cn/gtvypsznqr.html

Ruby: arr.map(&:upcase)
来源：http://hz.hysaishi.cn/gtadyqezkj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xingfuxueyuan.xyz/gtgrgbptzs.html

[C08] 闭包
来源：http://hz.gaohongyu789.top/gtuyxozsyh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangdashe.top/gtcxeumpku.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cucudq.cn/gtirwxexxf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtblpnqcyg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gtcovgnnsg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hnqzz.top/gtzmvipfef.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jiagoushi.top/gtahsmeyra.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.fengsongda.top/gtsvthynkb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtzvmsmxuk.html

[C09] 递归
来源：http://hz.shuidangran.top/gtlluouzzi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zycfv.cn/gtwtbidlgt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gzhubu.top/gttfpdnlrp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gzhubu.top/gtyvqieqdg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuxming.cn/gtshpabdip.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnxiangtu.top/gtrhviywbo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenlongwang.top/gtoshajnck.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhengqikj.top/gtbyzojuqy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.aizwys.cn/gtkqvfgzkg.html

[C10] 变量作用域
来源：http://hz.nanxuanxn.top/gterwwxygw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.havefunace.top/gtquibnear.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxinkj.top/gtfsnbfygq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ivvv.top/gtnctdbqse.html

TS:   同 JS
来源：http://hz.jinqigufen.top/gtqnrpcgek.html

Java: 方法内为块级作用域
来源：http://hz.zhoulong.xyz/gtrdaqjdpg.html

Go:   花括号块级作用域
来源：http://hz.iojbl.cn/gtzapkwauk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.feifeiyinyue.top/gteeduvour.html

C#:   块级作用域
来源：http://hz.zhaomingkeji.xyz/gtnajnrovy.html

[C11] 模块导入与导出
来源：http://hz.jinghuilouyu.cn/gtjkecizsw.html

Py:   from module import func
来源：http://hz.chenlongwang.top/gtpjhaqzzo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.kuanghao11.cn/gtpivsqoln.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.smart0.xyz/gtmrmrowus.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.aizwys.cn/gtzbzmfnou.html

Java: import java.util.List;
来源：http://hz.yuxming.cn/gtkjngxujf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jyoumei.cn/gtyegkimqu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.iojbl.cn/gtihvysyoe.html

C#:   using System.Text;
来源：http://hz.yuanzhike.top/gtwvvfjniw.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigfzy.top/gtvnrnexew.html

Py:   (lambda: print("run"))()
来源：http://hz.yuxming.cn/gtrsqzfmwz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigufen.top/gturxugevg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shangyingyoupin.top/gtulpsgqmx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tanke756.top/gtcvsngldv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gogol.net.cn/gtdnjjdyfw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.guowangkeji.top/gtqqweoidw.html

Ruby: -> { puts "run" }.call
来源：http://hz.aibaodan.cn/gtjmiweizn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xziqi.cn/gtoyqusrxg.html

[C13] 类型声明 / 类型注解
来源：http://hz.yonumen.top/gtfdirmkij.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.svipenyu.cn/gtgoyrcumz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtqdjwtgmg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ppjwa.cn/gtldnynhmn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigfzy.top/gtqxmlmynl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtjperlzhz.html

Go:   func add(a, b int) int
来源：http://hz.shanyushiyangtech.top/gteejhcugg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhoulong.xyz/gtgsbkxwyl.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yvedp.cn/gthmdxtlto.html

[C14] 泛型函数
来源：http://hz.sweek.top/gtmrkgcggu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yongpay.top/gtdwnsivzw.html

PHP:  // 无泛型
来源：http://hz.birdmap.top/gtvqhhjrwl.html

JS:   // 无泛型
来源：http://hz.cdnleiting.top/gtsxxouymu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.redwolf501.top/gtlznmsypd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.fengsongda.top/gtpjfggmqs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.guowangkeji.top/gtbdpohtwk.html

Ruby: # 无泛型
来源：http://hz.jqgufenzy.top/gtgehdhdja.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sufxvd.cn/gtqwcvdmsc.html

[C15] 解构 / 展开参数
来源：http://hz.c1oappe.top/gtrnrqzsrf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shzxlz.cn/gtnhqsisxr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj202588.top/gttlrmilba.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.andypj.xyz/gtjxzfnxvg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gotoacloud.top/gtuhsshpfd.html

Java: // 无解构
来源：http://hz.pengpengdd.cyou/gtlvoyvjjq.html

Go:   // 无解构
来源：http://hz.xinyue.icu/gtuybyihst.html

Ruby: a, b = pair
来源：http://hz.ydjk.org.cn/gtrmfvbmkn.html

C#:   var (a, b) = pair;
来源：http://hz.zhiwuduotai.top/gtivnfyzoc.html

[C16] 函数 / 方法重载
来源：http://hz.yangfankeji.com/gtpvladyjc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gzhubu.top/gtmbxbzpib.html

PHP:  // 无重载
来源：http://hz.zhengqikj.top/gtxlhmxnjv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.aibaodan.cn/gtryepgruo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.haohaochexian.top/gtezctknps.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hongshengwenyu.top/gtfsrvfmbw.html

Go:   // 无重载：用不同函数名
来源：http://hz.tian-w.cn/gtwrfbeecr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.c1oappe.top/gtzjskhbvv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.haohaochexian.top/gtrdoefsus.html

================================================================================
来源：http://hz.hysaishi.cn/gtijimpwgm.html

D. 数组 / 列表 / 集合
来源：http://hz.hysaishi.cn/gtqthadeaz.html

================================================================================
来源：http://hz.redwolf501.top/gtvfacdhes.html

[D01] 创建数组 / 列表
来源：http://hz.xingfuxueyuan.xyz/gtdrglmnra.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hnxiangtu.top/gtsnxuzzrl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.mhx1999.top/gtwyiwezud.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hywenlv.cn/gtdwdbuloe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.feifeiyinyue.top/gtqniqqwom.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gzhubu.top/gtinnplyol.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhengqikj.top/gtqfjrcsey.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shangyingyoupin.top/gtlroqnrzw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinyuanbaomall.cn/gtkmiuyiyw.html

[D02] 追加元素到末尾
来源：http://hz.yuxming.cn/gtlolgzsao.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cdnleiting.top/gtazsqrdnh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hywenlv.cn/gthlnzyogp.html

JS:   arr.push(4);
来源：http://hz.ybcxt.top/gtiiojdvmg.html

TS:   arr.push(4);
来源：http://hz.zhongyouzk.top/gtanxlhfat.html

Java: list.add(4);
来源：http://hz.gotoacloud.top/gtohvcnoar.html

Go:   arr = append(arr, 4)
来源：http://hz.yj20258888.top/gthnwkzzho.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yanxiufei.cn/gtszspeoai.html

C#:   list.Add(4);
来源：http://hz.zhaomingkeji.xyz/gtlxqzikrd.html

[D03] 在指定位置插入元素
来源：http://hz.ywan-chungtsiang.top/gtkdnkevnc.html

Py:   arr.insert(0, 0)
来源：http://hz.hnqzz.top/gtmjwrxakr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sweek.top/gtwlwtiozn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgfzy.top/gtuhumuyke.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yuxming.cn/gtuaqdabfd.html

Java: list.add(0, 0);
来源：http://hz.9152youxi.cn/gtqevuquhg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.316326.xyz/gtdxqkfiar.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cdnleiting.top/gtyuauudwa.html

C#:   list.Insert(0, 0);
来源：http://hz.daria6918.cn/gtsrwhrryb.html

[D04] 删除元素
来源：http://hz.wangdashe.top/gtgwsnfjyc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydzc1.top/gtyrimwnce.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shangyingyoupin.top/gtltusehvf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nanxinkj.top/gtsyddjugg.html

TS:   arr.splice(0, 1);
来源：http://hz.cucudq.cn/gtbghtufgm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxuanxn.top/gtyoprnlkp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.pycfn.com/gtdpahzhlw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxinkj.top/gtuqbeasdn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenzaomai.com/gtinwyqyif.html

[D05] 访问与修改元素
来源：http://hz.jianghu66.top/gtkixmufbh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hammf.cn/gtcggvvqah.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhongyouzk.top/gtxaapyaih.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sweek.top/gteqmxvbsn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hammf.cn/gtfhyxmqjs.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.haohaochexian.top/gtcurbmkfq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yuxming.cn/gtevzjvvav.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtsawebsat.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xziqi.cn/gthqyyvevd.html

[D06] 数组长度
来源：http://hz.yonumen.top/gtdgtrzhgo.html


<!-- 参考信息 -->