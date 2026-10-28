代发 wailian999

[B05] 遍历数组 / 列表
来源：http://hz.yanxiufei.cn/gttlrdxafv.html

Py:   for item in arr: print(item)
来源：http://hz.hnxiangtu.top/gtesftzmyi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ivvv.top/gtmqgwrfys.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.gzhubu.top/gtbaybhimf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.shzxlz.cn/gtaefziqnk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yj20258.top/gtdjmfxpfi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jqgfzy.top/gtgjnonqoe.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ehwqpu.com/gtwdklnykk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.ppjwa.cn/gtlviigbbk.html

[B06] 遍历字典 / 对象
来源：http://hz.yj202588.top/gtskzveims.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zdqjudy.top/gtlxfwfxrn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.andypj.xyz/gtffrmiard.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.pengpengdd.cyou/gtpxqcanwm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yuxming.cn/gtkgqnntke.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhijiandao.cn/gthtdtvfvn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.smart0.xyz/gthvdhpwyz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jinqigufen.top/gtuyuoyiqc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.c1oappe.top/gtryksaddv.html

[B07] while 循环
来源：http://hz.ywan-chungtsiang.top/gtmjuubips.html

Py:   while i < 10: i += 1
来源：http://hz.ydzc1.top/gtnqbcrbqh.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.redwolf501.top/gtznzyzluu.html

JS:   while (i < 10) { i++; }
来源：http://hz.cqqwz.cn/gtqmhesmjf.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtobxgkcry.html

Java: while (i < 10) { i++; }
来源：http://hz.pengpengdd.cyou/gtxeawzwdy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.nwbrower.top/gtbwcbrrum.html

Ruby: while i < 10; i += 1; end
来源：http://hz.daxiang520.top/gtwwtzzvfd.html

C#:   while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtrkxvauns.html

[B08] do-while（至少执行一次）
来源：http://hz.shuidangran.top/gtzffagbzs.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xuanzx.com/gtzgiqyjxi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zycfv.cn/gtffzcmlhw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.tianlin.xyz/gtdeinomlj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtvewbhhdp.html

Java: do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gtooxcgkxo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.iojbl.cn/gtvompuddl.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.316326.xyz/gtyyhplkdy.html

C#:   do { i++; } while (i < 10);
来源：http://hz.nwbrower.top/gtjqamqtxh.html

[B09] break 与 continue
来源：http://hz.bjfxy.top/gtfnwtbjfa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xuetiantiany.cn/gttgrpqhgg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jyoumei.cn/gtyzkyszpr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gttyhvsilx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gtjylugfkf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gtyjacxhld.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zycfv.cn/gtqmbnujya.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.gogol.net.cn/gtdzftxbaw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtacfsnydl.html

[B10] 遍历同时拿索引
来源：http://hz.nanxinkj.top/gtrcnpmywm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.wangshuangyany.cn/gtnvgojhjc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gaohongyu789.top/gtqsceabxk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.c1oappe.top/gtrylrdyeq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhaomingkeji.xyz/gtjgycurwz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jianghu66.top/gthsrnmifq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.andypj.xyz/gtlkruccdv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tanke756.top/gtlghtdqph.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinghuilouyu.cn/gtsceuvlam.html

[B11] 生成数字序列 / 区间
来源：http://hz.haohaochexian.top/gtzlpdrzqj.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenlongwang.top/gtsuycdyvu.html

PHP:  range(0, 10, 2);
来源：http://hz.ehwqpu.com/gtaggnadpb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.vqdsnc.cn/gtsiqhssid.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.mhx1999.top/gtogexkhoh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.feifeiyinyue.top/gtfdhjodqk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.52xcode.cn/gtgajknhnp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hammf.cn/gtabsudcqc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.svipenyu.cn/gtvozwdcty.html

[B12] 跳出多层循环
来源：http://hz.meibo888.top/gtwxzprtze.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gzhubu.top/gtgyshssan.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.aizwys.cn/gtsixvvvjn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fengsongda.top/gtzibqecep.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhaomingkeji.xyz/gtidfdxmjv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jlsjyb.cn/gtlaitswko.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.9152youxi.cn/gtevpsqqxb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yongpay.top/gtibzbtjfc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.pycfn.com/gtjqgmgubk.html

[B13] 判断是否为数字
来源：http://hz.xinyue.icu/gtyapdjely.html

Py:   isinstance(x, (int, float))
来源：http://hz.gaohongyu789.top/gtmgxxyiss.html

PHP:  is_numeric($x)
来源：http://hz.zhijiandao.cn/gtzjpyotsv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aizwys.cn/gtossqldex.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtguygmfdy.html

Java: x instanceof Number
来源：http://hz.guannengcc.top/gtlppwlcmk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhixingplan.top/gteujyfcgu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.birdmap.top/gtjrnbpctn.html

C#:   x is int or double or decimal
来源：http://hz.yangfankeji.com/gtxoupaywm.html

[B14] 判断值是否在集合内
来源：http://hz.sxryk.cn/gtqiootpdq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.guannengcc.top/gtrcxtarid.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.tanke756.top/gtmfxpdtfy.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cashguo.top/gtylrqovir.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yanxiufei.cn/gtrrqlepna.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinghuilouyu.cn/gtcvxzsgfb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenjidiqi.icu/gtrmenwemq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.tian-w.cn/gtlnbhvbbz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hywenlv.cn/gtsmptefmk.html

[B15] 布尔运算与取反
来源：http://hz.ywan-chungtsiang.top/gtvrdnwkdn.html

Py:   a and b or not c
来源：http://hz.xziqi.cn/gtwrxxnzxc.html

PHP:  $a && $b || !$c
来源：http://hz.sufxvd.cn/gtbejejcst.html

JS:   a && b || !c
来源：http://hz.chenzaomai.com/gtqwgaucpi.html

TS:   a && b || !c
来源：http://hz.meibo888.top/gtbptqqzqk.html

Java: a && b || !c
来源：http://hz.aizwys.cn/gtpyebflzr.html

Go:   a && b || !c
来源：http://hz.yj20258.top/gtonusjarf.html

Ruby: a && b || !c
来源：http://hz.zhoulong.xyz/gtxohcpepn.html

C#:   a && b || !c
来源：http://hz.cqqwz.cn/gtxluymvex.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jlsjyb.cn/gtdkvahvez.html

Py:   if not data: return
来源：http://hz.ivvv.top/gtqaijsakt.html

PHP:  if (!$data) { return; }
来源：http://hz.kuanghao11.cn/gtqqomkonx.html

JS:   if (!data) return;
来源：http://hz.daria6918.cn/gtlkehbdlx.html

TS:   if (!data) return;
来源：http://hz.316326.xyz/gtaesibpiq.html

Java: if (data == null) return;
来源：http://hz.yuxming.cn/gtmbjtlgjv.html

Go:   if data == nil { return }
来源：http://hz.smart0.xyz/gtrbnwdxhl.html

Ruby: return if data.nil?
来源：http://hz.shangyingyoupin.top/gttqbmtjhl.html

C#:   if (data == null) return;
来源：http://hz.yuanzhike.top/gtnsaccrph.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtdhlaxvgm.html

C. 函数与作用域
来源：http://hz.xinyue.icu/gtrvwkrzcl.html

================================================================================
来源：http://hz.yueranfly.top/gtyohzixyr.html

[C01] 定义函数
来源：http://hz.yueranfly.top/gttnhshscs.html

Py:   def add(a, b): return a + b
来源：http://hz.shanyushiyangkeji.top/gtvaottjwv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgufenzy.top/gtnzopkuby.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yj20258888.top/gtvbgaeabb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cqqwz.cn/gtblccknig.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tianlin.xyz/gttpuaaohu.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.wangshuangyany.cn/gtmnmjxaue.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinqigfzy.top/gtcpnfbghn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtoxwtuatq.html

[C02] 默认参数
来源：http://hz.xylfe.cn/gtyejglghj.html

Py:   def greet(name="World"): return name
来源：http://hz.redwolf501.top/gtupzkaryt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhongyouzk.top/gtcnkywtnn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hammf.cn/gtlyqukzws.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.dashuyun.cn/gtvtrbxbxn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ywan-chungtsiang.top/gthkkzutjy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.c1oappe.top/gtvgolroqc.html

Ruby: def greet(name = "World") = name
来源：http://hz.hammf.cn/gtaatmokqt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj202588.top/gtalucugsl.html

[C03] 可变参数
来源：http://hz.hysaishi.cn/gtdnqrnrrl.html

Py:   def total(*args): return sum(args)
来源：http://hz.cashguo.top/gtetajckmt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jinqigufen.top/gtqvxomqle.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangtech.top/gtzsnqkswx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.svipenyu.cn/gtnkdxlnet.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.feifeiyinyue.top/gtvuxnbvpd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shangyingyoupin.top/gtgunwilnl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhaomingkeji.xyz/gtoprbzxtz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydzc1.top/gtgypljlnc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xuanzx.com/gtjkzqymwv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.wangshuangyany.cn/gtzkmxkjuj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinqigfzy.top/gtyxzntzhc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.smart0.xyz/gtuqxfcxsh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.pengpengdd.cyou/gtpffysynw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.316326.xyz/gtbzklqpkj.html

Go:   // 无：用配置结构体参数
来源：http://hz.nanxuanxn.top/gtobnznuwq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtpwbwnpom.html

C#:   f(a: 1, b: 2)
来源：http://hz.0kj1m.cn/gtottcckwg.html

[C05] 返回多个值
来源：http://hz.smart0.xyz/gtecdcbqvd.html

Py:   return a, b
来源：http://hz.sweek.top/gtzvocdfmh.html

PHP:  return [$a, $b];
来源：http://hz.jinyuanbaomall.cn/gtruldootr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.wangdashe.top/gtqhjteobd.html

TS:   return { a, b };
来源：http://hz.xuetiantiany.cn/gtocmtbkwq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yueranfly.top/gtgutqmszb.html

Go:   return a, b
来源：http://hz.meibo888.top/gtnzitdrkn.html

Ruby: return a, b
来源：http://hz.ywan-chungtsiang.top/gtpugqckbe.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.havefunace.top/gtmzeafhfa.html

[C06] 匿名函数 / lambda
来源：http://hz.daria6918.cn/gtnrtnsvqu.html

Py:   square = lambda x: x * x
来源：http://hz.feifeiyinyue.top/gtlknayjne.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.dashuyun.cn/gtefoblgcd.html

JS:   const square = x => x * x;
来源：http://hz.sysykeji.top/gtylrbddqy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhengqikj.top/gtfhkofvvl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.pengpengdd.cyou/gtmeaylyml.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenlongwang.top/gtjfvwucfe.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shanyushiyangtech.top/gtlpdguxwm.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.svipenyu.cn/gtlzfovbcn.html

[C07] 把函数作为参数传入
来源：http://hz.yuanzhike.top/gtlxbcdikp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.andypj.xyz/gtjqcwhnvv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guannengcc.top/gtahykecid.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jqgfzy.top/gtukrnkpwj.html

TS:   arr.map(String)
来源：http://hz.ywan-chungtsiang.top/gtspvebial.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.bjfxy.top/gtypijzqds.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.wangdashe.top/gthvakyfiw.html

Ruby: arr.map(&:upcase)
来源：http://hz.cdnleiting.top/gtqrnsbceg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sweek.top/gtltjjymle.html

[C08] 闭包
来源：http://hz.xingfuxueyuan.xyz/gtlevsntnh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jianghu66.top/gthfmdyoud.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.snrcjt.cn/gtehbboqar.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtltsgdlwk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnqzz.top/gthxsajxjs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yuxming.cn/gtocqbivxl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.nanxuanxn.top/gtkmeucppw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinghuilouyu.cn/gtieuddjiw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtvuwosxgl.html

[C09] 递归
来源：http://hz.shanyushiyangkeji.top/gtlygooajr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xziqi.cn/gtsisbuymm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hammf.cn/gtsgszfamq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenzaomai.com/gtekecyryz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxuanxn.top/gtvmlkoyly.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yangfankeji.com/gtmphxmogp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tianlin.xyz/gtyvaekceg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.aizwys.cn/gtlomnwwbs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.havefunace.top/gtgrhdwlak.html

[C10] 变量作用域
来源：http://hz.aibaodan.cn/gthxkmdduz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.redwolf501.top/gthoxzpbhi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.0kj1m.cn/gtdowezito.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.dashuyun.cn/gtnqionsft.html

TS:   同 JS
来源：http://hz.shzxlz.cn/gtrqgrmwdk.html

Java: 方法内为块级作用域
来源：http://hz.ydjk.org.cn/gtpxmmooky.html

Go:   花括号块级作用域
来源：http://hz.ivvv.top/gtvwbfojpy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sufxvd.cn/gtkzsnmpgv.html

C#:   块级作用域
来源：http://hz.mhx1999.top/gtpmbpbcux.html

[C11] 模块导入与导出
来源：http://hz.cheryme.top/gtypswakhh.html

Py:   from module import func
来源：http://hz.shanyushiyangtech.top/gtgycbtoqh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xuetiantiany.cn/gtnuwuzpia.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gaohongyu789.top/gtnmhlvuin.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.9152youxi.cn/gtohofctwi.html

Java: import java.util.List;
来源：http://hz.jinqigfzy.top/gtubzugroi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yangfankeji.com/gtprwysysh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xingfuxueyuan.xyz/gtkcowuywd.html

C#:   using System.Text;
来源：http://hz.chenjidiqi.icu/gtvdbdrajr.html

[C12] 立即执行函数 IIFE
来源：http://hz.ehwqpu.com/gtabwdppqh.html

Py:   (lambda: print("run"))()
来源：http://hz.ivvv.top/gtfqkqijhd.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shangyingyoupin.top/gtrpfyvcjy.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hysaishi.cn/gtecfpqtzo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtkpuofudy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.snrcjt.cn/gtvgeeydfg.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hfpthk.cn/gtukvyjqxx.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhijiandao.cn/gtwrdswqhg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.birdmap.top/gtnunipuxi.html

[C13] 类型声明 / 类型注解
来源：http://hz.chenjidiqi.icu/gtafzwgyyj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhengqikj.top/gtggdqxxnx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.bjfxy.top/gtytvkloqk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xuanzx.com/gtqvzzhqxg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shuidangran.top/gtpktjqdre.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.smart0.xyz/gtgricvdfp.html

Go:   func add(a, b int) int
来源：http://hz.jqgfzy.top/gtnvwppgkh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.daria6918.cn/gtebwqbhdf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.mhx1999.top/gtpxcvjdtn.html

[C14] 泛型函数
来源：http://hz.chenjidiqi.icu/gtnefixipn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shanyushiyangkeji.top/gtyugvbubn.html

PHP:  // 无泛型
来源：http://hz.nwbrower.top/gtwfpfkiiv.html

JS:   // 无泛型
来源：http://hz.0kj1m.cn/gttxsnqbcs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.svipenyu.cn/gtpvtvuzkj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.9152youxi.cn/gtdlzghhdu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cucudq.cn/gtnuynlqyl.html

Ruby: # 无泛型
来源：http://hz.pycfn.com/gtfsxqdvve.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sysykeji.top/gtlrfhvrly.html

[C15] 解构 / 展开参数
来源：http://hz.jiagoushi.top/gtkvvkpmmo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gzhubu.top/gtsccouxqn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhongyouzk.top/gthxwlieaf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtyowldqgw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.9152youxi.cn/gtmhiskdcw.html

Java: // 无解构
来源：http://hz.jqgfzy.top/gtizwtgtug.html

Go:   // 无解构
来源：http://hz.daria6918.cn/gtfoyhbreo.html

Ruby: a, b = pair
来源：http://hz.sufxvd.cn/gtwemputgn.html

C#:   var (a, b) = pair;
来源：http://hz.guannengcc.top/gtouowentm.html

[C16] 函数 / 方法重载
来源：http://hz.zhongyouzk.top/gtgkugppwf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nwbrower.top/gtqahxjgow.html

PHP:  // 无重载
来源：http://hz.pengpengdd.cyou/gtrwzzwxcg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jyoumei.cn/gtixdotunv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shangyingyoupin.top/gtwfrnwhao.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ywan-chungtsiang.top/gtgntleyej.html

Go:   // 无重载：用不同函数名
来源：http://hz.ivvv.top/gtbrtdatwg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ehwqpu.com/gtefzqothe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydjk.org.cn/gtserjjimj.html

================================================================================
来源：http://hz.hnqzz.top/gtkcipltfa.html

D. 数组 / 列表 / 集合
来源：http://hz.tianlin.xyz/gtgdvrjfyj.html

================================================================================
来源：http://hz.tanke756.top/gtfrgynmzp.html

[D01] 创建数组 / 列表
来源：http://hz.zhiwuduotai.top/gttarsjxcs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jianghu66.top/gtlrojqhzr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jqgufenzy.top/gthvgrdiwk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sxryk.cn/gtxupzwjgk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.haohaochexian.top/gtseaihqtx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenlongwang.top/gtpqtdzrdz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hfpthk.cn/gtgtwkzhsi.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hammf.cn/gtfshfnvxe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhixingplan.top/gtwfrftnlv.html

[D02] 追加元素到末尾
来源：http://hz.meibo888.top/gtuqnvmfqb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yj202588.top/gtcnzgffbw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xylfe.cn/gtvklosroa.html

JS:   arr.push(4);
来源：http://hz.hnxiangtu.top/gtbmjftxsn.html

TS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtzxijdurt.html

Java: list.add(4);
来源：http://hz.yonumen.top/gteqafsgsl.html

Go:   arr = append(arr, 4)
来源：http://hz.redwolf501.top/gtyozlefsn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuanzhike.top/gtunfjuafg.html

C#:   list.Add(4);
来源：http://hz.snrcjt.cn/gtzxdjeikt.html

[D03] 在指定位置插入元素
来源：http://hz.yanxiufei.cn/gtaehcmswy.html

Py:   arr.insert(0, 0)
来源：http://hz.snrcjt.cn/gtpypoxyzm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yonumen.top/gtvzmacayt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj202588.top/gtgbcuipwr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhixingplan.top/gtbavriqao.html

Java: list.add(0, 0);
来源：http://hz.zhaomingkeji.xyz/gtfhkustuc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yonumen.top/gtpiozrxca.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sufxvd.cn/gtkaxwjhub.html

C#:   list.Insert(0, 0);
来源：http://hz.daxiang520.top/gtdbvsphom.html

[D04] 删除元素
来源：http://hz.svipenyu.cn/gtbcwpzotx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cqqwz.cn/gtmkujdnjv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jqgufenzy.top/gtlhvkefyw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hysaishi.cn/gtnwdvjsbn.html

TS:   arr.splice(0, 1);
来源：http://hz.aizwys.cn/gtgssuadyy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.havefunace.top/gtzkarqnxp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yuanzhike.top/gtekjxciux.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.pengpengdd.cyou/gtyycqrltr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tian-w.cn/gtpikhvrgj.html

[D05] 访问与修改元素
来源：http://hz.fzhhl.top/gtjocdvlsh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtzvznmurv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtmipldcvf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ybcxt.top/gtfgpcvpji.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.dianchejie.cn/gtgggvmqii.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.birdmap.top/gtwpcrierx.html


<!-- 参考信息 -->