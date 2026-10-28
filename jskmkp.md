代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yangfankeji.com/gttfsgruab.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hywenlv.cn/gtfeokjsmd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.daxiang520.top/gtlrnjcrnw.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zhongyouzk.top/gtjjsigysm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jyoumei.cn/gtbzoojatd.html

[B06] 遍历字典 / 对象
来源：http://hz.havefunace.top/gtnxuonvps.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cucudq.cn/gtzhregvek.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hongshengwenyu.top/gtdlkicbzr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ivvv.top/gtlndiktki.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cdnleiting.top/gtlivvvsph.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gogol.net.cn/gtvqvdlsvu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shzxlz.cn/gtkagxgnad.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yanxiufei.cn/gtohzomfpi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.ydzc1.top/gtcajaubfe.html

[B07] while 循环
来源：http://hz.tanke756.top/gtrjjbiyqv.html

Py:   while i < 10: i += 1
来源：http://hz.sufxvd.cn/gtwuxohreu.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ivvv.top/gtyvpthetk.html

JS:   while (i < 10) { i++; }
来源：http://hz.yj20258888.top/gtrtuhafca.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhoulong.xyz/gtclfwhaul.html

Java: while (i < 10) { i++; }
来源：http://hz.snrcjt.cn/gtfuwpqzex.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yj20258888.top/gtwiyiktme.html

Ruby: while i < 10; i += 1; end
来源：http://hz.nanxuanxn.top/gtynouksot.html

C#:   while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtunzgsrdc.html

[B08] do-while（至少执行一次）
来源：http://hz.feifeiyinyue.top/gttfqqlihl.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jqgufenzy.top/gtofwdcsdy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.svipenyu.cn/gtcfdatiyv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gotoacloud.top/gtbazlvtby.html

TS:   do { i++; } while (i < 10);
来源：http://hz.meibo888.top/gtngmfajmk.html

Java: do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gtedhobklf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cqqwz.cn/gtyquowqno.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.havefunace.top/gtrixyhpse.html

C#:   do { i++; } while (i < 10);
来源：http://hz.guannengcc.top/gtdpiejnnu.html

[B09] break 与 continue
来源：http://hz.smart0.xyz/gtdeqepixd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shangyingyoupin.top/gtqfuxgnyj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jqgfzy.top/gtrtrfqxrs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gtxprippwc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gtkmrksfqj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtbigtsfms.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xuanzx.com/gtwyxeiraa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.mhx1999.top/gtratxvsvx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtauiytukp.html

[B10] 遍历同时拿索引
来源：http://hz.snrcjt.cn/gtzwoniyfj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hnxiangtu.top/gtvxufxdjy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xinyue.icu/gtsmnzaoxp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.fzhhl.top/gtiriwzzbd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhijiandao.cn/gtrxexrwyi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shangyingyoupin.top/gtqspgbxkp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.c1oappe.top/gtzfyypgpw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhaomingkeji.xyz/gtxyxtljra.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhoulong.xyz/gtnafsapeu.html

[B11] 生成数字序列 / 区间
来源：http://hz.wangshuangyany.cn/gtaspnpppq.html

Py:   list(range(0, 10, 2))
来源：http://hz.hysaishi.cn/gtzyinpzvu.html

PHP:  range(0, 10, 2);
来源：http://hz.ehwqpu.com/gtykhjiubu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dashuyun.cn/gttmmqilwo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shzxlz.cn/gtsjwlzyuo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.vqdsnc.cn/gtaveaxuil.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yanxiufei.cn/gtgjfqhggs.html

Ruby: (0...10).step(2).to_a
来源：http://hz.tianlin.xyz/gtuwrtbpch.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.havefunace.top/gtfmksmszv.html

[B12] 跳出多层循环
来源：http://hz.jqgufenzy.top/gtckzsebxd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ehwqpu.com/gtqntnvkra.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sxryk.cn/gtwutyfciz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fengsongda.top/gtihegasvw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.mhx1999.top/gtrbrbgdtk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.daxiang520.top/gtnmkfamcr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.316326.xyz/gtaalfwmjk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xylfe.cn/gtgijsnayy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.bjfxy.top/gttlnycdyg.html

[B13] 判断是否为数字
来源：http://hz.aizwys.cn/gtfnsfxibq.html

Py:   isinstance(x, (int, float))
来源：http://hz.xuanzx.com/gtjhozmxdy.html

PHP:  is_numeric($x)
来源：http://hz.daxiang520.top/gtmzehluca.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dianchejie.cn/gtpwycufwq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jyoumei.cn/gtaoxkdrop.html

Java: x instanceof Number
来源：http://hz.kuanghao11.cn/gtrrwpcxgn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.tanke756.top/gtrxyfxcrz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.cqqwz.cn/gtpiicwjfm.html

C#:   x is int or double or decimal
来源：http://hz.birdmap.top/gtsrclnfha.html

[B14] 判断值是否在集合内
来源：http://hz.xinyue.icu/gtqiwkbtoe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jiagoushi.top/gtsfbosvzc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shzxlz.cn/gtihkloicx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ehwqpu.com/gtubxjdbjh.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.52xcode.cn/gtpkocoozh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.guannengcc.top/gtsnmcypec.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.316326.xyz/gtnxgkreiw.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.andypj.xyz/gthdtpvjbn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hfpthk.cn/gtlswhvvse.html

[B15] 布尔运算与取反
来源：http://hz.jiagoushi.top/gtxuwinbxt.html

Py:   a and b or not c
来源：http://hz.zhiwuduotai.top/gtoujkmycf.html

PHP:  $a && $b || !$c
来源：http://hz.fzhhl.top/gtofcintmi.html

JS:   a && b || !c
来源：http://hz.ydzc1.top/gtzazvpzlx.html

TS:   a && b || !c
来源：http://hz.svipenyu.cn/gtwllmbtsg.html

Java: a && b || !c
来源：http://hz.0kj1m.cn/gtpwphfnhu.html

Go:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtxuzcfyvb.html

Ruby: a && b || !c
来源：http://hz.zycfv.cn/gtwyfnrlxh.html

C#:   a && b || !c
来源：http://hz.pycfn.com/gtgrududwn.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.chenjidiqi.icu/gtzkpqfawd.html

Py:   if not data: return
来源：http://hz.xuanzx.com/gtrsakoqgb.html

PHP:  if (!$data) { return; }
来源：http://hz.cdnleiting.top/gtrrgislie.html

JS:   if (!data) return;
来源：http://hz.aizwys.cn/gttfcapany.html

TS:   if (!data) return;
来源：http://hz.52xcode.cn/gtlaucrezy.html

Java: if (data == null) return;
来源：http://hz.dashuyun.cn/gtkbetoowf.html

Go:   if data == nil { return }
来源：http://hz.wangdashe.top/gtyhgknfzl.html

Ruby: return if data.nil?
来源：http://hz.hysaishi.cn/gtlofnnbnu.html

C#:   if (data == null) return;
来源：http://hz.meibo888.top/gtppuyyyqb.html

================================================================================
来源：http://hz.svipenyu.cn/gtdzjxsoha.html

C. 函数与作用域
来源：http://hz.birdmap.top/gtsvcctikf.html

================================================================================
来源：http://hz.nwbrower.top/gtllcsatys.html

[C01] 定义函数
来源：http://hz.bjfxy.top/gtfihhuiyk.html

Py:   def add(a, b): return a + b
来源：http://hz.ywan-chungtsiang.top/gtcjurdoiw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gtwyjarjgk.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tianlin.xyz/gtxhikhdpz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtrokzsiwu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtfqpdukwc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yj202588.top/gtfwopwvkn.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yonumen.top/gttqhosyya.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gtpsqpkkwp.html

[C02] 默认参数
来源：http://hz.ybcxt.top/gtqvugvhds.html

Py:   def greet(name="World"): return name
来源：http://hz.zhaomingkeji.xyz/gtrdawnrtd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.bjfxy.top/gtathnkrwl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.vqdsnc.cn/gtaqphzkhj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.tian-w.cn/gtxxsfvcqb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ydzc1.top/gtmxrfmiyo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.nanxinkj.top/gtruhlfwcp.html

Ruby: def greet(name = "World") = name
来源：http://hz.xingfuxueyuan.xyz/gtgdhcugcv.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.0kj1m.cn/gtfyuedqvg.html

[C03] 可变参数
来源：http://hz.shanyushiyangtech.top/gtpafjqxtb.html

Py:   def total(*args): return sum(args)
来源：http://hz.ywan-chungtsiang.top/gtrnauvehh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.aibaodan.cn/gtoncnzrur.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangkeji.top/gtgyxhsfui.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenjidiqi.icu/gtfupzcegr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dianchejie.cn/gthogouywe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj20258888.top/gtpibdrvuc.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.mhx1999.top/gtpzbcnjpq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.tianlin.xyz/gtlyhwcvsf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gzhubu.top/gtzfkvdicu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ywan-chungtsiang.top/gtoghjmxdx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jlsjyb.cn/gtudobfngz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yuxming.cn/gtflcbooyx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yongpay.top/gtjtmqiehz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.wangshuangyany.cn/gtmfuxaieh.html

Go:   // 无：用配置结构体参数
来源：http://hz.cheryme.top/gtsjvugvjp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.meibo888.top/gttgoaalmz.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhongyouzk.top/gtngvifbkv.html

[C05] 返回多个值
来源：http://hz.wangdashe.top/gtnocybwjk.html

Py:   return a, b
来源：http://hz.shzxlz.cn/gtjeuoeent.html

PHP:  return [$a, $b];
来源：http://hz.yueranfly.top/gtxrohkzud.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tanke756.top/gtucyuayjy.html

TS:   return { a, b };
来源：http://hz.jinqigufen.top/gtanmaufxa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.52xcode.cn/gtbyjzrifa.html

Go:   return a, b
来源：http://hz.andypj.xyz/gtczhuuhif.html

Ruby: return a, b
来源：http://hz.aibaodan.cn/gtsnfjryfl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinqigufen.top/gttoqptiwp.html

[C06] 匿名函数 / lambda
来源：http://hz.snrcjt.cn/gtmprdvbfi.html

Py:   square = lambda x: x * x
来源：http://hz.smart0.xyz/gtzbjcjzur.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.feifeiyinyue.top/gtqcalmqcg.html

JS:   const square = x => x * x;
来源：http://hz.xingfuxueyuan.xyz/gthdfnokjv.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yonumen.top/gtllmxeqcz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ivvv.top/gtmkyzavyt.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.dianchejie.cn/gttfhnzonu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.bjfxy.top/gtnfxsalkv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dashuyun.cn/gtsacolcdk.html

[C07] 把函数作为参数传入
来源：http://hz.cucudq.cn/gtldzmnzcx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shanyushiyangtech.top/gtxtjrlpxf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jianghu66.top/gtbonekcxg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.bjfxy.top/gtldylkqbl.html

TS:   arr.map(String)
来源：http://hz.pengpengdd.cyou/gtjhtmzrcg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xinyue.icu/gtbezypdql.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ydjk.org.cn/gtlefpcoyh.html

Ruby: arr.map(&:upcase)
来源：http://hz.chenzaomai.com/gtvmizwcja.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xziqi.cn/gteyilufqj.html

[C08] 闭包
来源：http://hz.mhx1999.top/gtsjimwpkz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ywan-chungtsiang.top/gtpjwpfhof.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj202588.top/gtljrpnzsn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenjidiqi.icu/gteaywboxi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtdrppaxvw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.guannengcc.top/gtdprtwukx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shanyushiyangtech.top/gtsdeuafaq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shzxlz.cn/gtwjbacprx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtznyakweg.html

[C09] 递归
来源：http://hz.yonumen.top/gttppkiiwx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.dianchejie.cn/gtbvzvtthw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gaohongyu789.top/gtsathmshk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gzhubu.top/gtaatcstfj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tanke756.top/gtudndodeo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jinyuanbaomall.cn/gtjscgrqgu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.andypj.xyz/gtjrqdtrfg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinyuanbaomall.cn/gtabumimee.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yueranfly.top/gtzurufgfa.html

[C10] 变量作用域
来源：http://hz.hongshengwenyu.top/gtucuxsfvk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj202588.top/gtyczggcqs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sxryk.cn/gtcqtdzcuu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.bjfxy.top/gtgubydusf.html

TS:   同 JS
来源：http://hz.feifeiyinyue.top/gtxubmakir.html

Java: 方法内为块级作用域
来源：http://hz.mhx1999.top/gtvyhoryhk.html

Go:   花括号块级作用域
来源：http://hz.xuetiantiany.cn/gtgbtkivtl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jqgufenzy.top/gtefizhkxd.html

C#:   块级作用域
来源：http://hz.shanyushiyangkeji.top/gtqtyhxcfq.html

[C11] 模块导入与导出
来源：http://hz.dianchejie.cn/gtvpbnpvdm.html

Py:   from module import func
来源：http://hz.andypj.xyz/gttxwrnukp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.pycfn.com/gtvnnimdqu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ivvv.top/gtylioaolo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.vqdsnc.cn/gtdlrnwoen.html

Java: import java.util.List;
来源：http://hz.aizwys.cn/gtbeztupsz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xinyue.icu/gtedtmsqsu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.andypj.xyz/gtulypqovp.html

C#:   using System.Text;
来源：http://hz.birdmap.top/gtyfsxwpdk.html

[C12] 立即执行函数 IIFE
来源：http://hz.0kj1m.cn/gtfwcegbqr.html

Py:   (lambda: print("run"))()
来源：http://hz.havefunace.top/gtrfqgrrld.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhoulong.xyz/gtqzjzdfcm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jyoumei.cn/gtifvtroyj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.meibo888.top/gtohpvisph.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinqigfzy.top/gtxshsajed.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jianghu66.top/gthykpjsbn.html

Ruby: -> { puts "run" }.call
来源：http://hz.jiagoushi.top/gtgqsbeoau.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.chenjidiqi.icu/gtnjyyoapw.html

[C13] 类型声明 / 类型注解
来源：http://hz.pycfn.com/gtuedfoztf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jianghu66.top/gtfuengtzq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.0kj1m.cn/gtjjgoibqa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jqgufenzy.top/gtyrzmuope.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtezrmxmhl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gttjyocklx.html

Go:   func add(a, b int) int
来源：http://hz.vqdsnc.cn/gtxbchdtbh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yj20258.top/gtaxrjtnah.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hammf.cn/gtgbyfmspc.html

[C14] 泛型函数
来源：http://hz.chenjidiqi.icu/gtaufmqodg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gogol.net.cn/gtwlwytfyo.html

PHP:  // 无泛型
来源：http://hz.yuxming.cn/gtpgclenqc.html

JS:   // 无泛型
来源：http://hz.cashguo.top/gtjxhvadud.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yuanzhike.top/gtqqxbsmfg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shzxlz.cn/gtqocmfsbj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.haohaochexian.top/gthzqgesbh.html

Ruby: # 无泛型
来源：http://hz.birdmap.top/gtkexpnloe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.dianchejie.cn/gtyqxckwnk.html

[C15] 解构 / 展开参数
来源：http://hz.yangfankeji.com/gtyjcvvvrv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tian-w.cn/gtrskqewrl.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ydjk.org.cn/gtoldkyuww.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.aibaodan.cn/gtgsyqcxzb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tian-w.cn/gtndopmsgy.html

Java: // 无解构
来源：http://hz.fengsongda.top/gtzzdkjoyc.html

Go:   // 无解构
来源：http://hz.sysykeji.top/gtmidctnhf.html

Ruby: a, b = pair
来源：http://hz.jianghu66.top/gtniksmxic.html

C#:   var (a, b) = pair;
来源：http://hz.tian-w.cn/gtilcjkmod.html

[C16] 函数 / 方法重载
来源：http://hz.jinyuanbaomall.cn/gteqggznwr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xuetiantiany.cn/gtiyapgtof.html

PHP:  // 无重载
来源：http://hz.zhaomingkeji.xyz/gtppfwhbpm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jianghu66.top/gtvmueydnw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hywenlv.cn/gtcbvbhpeo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ehwqpu.com/gtacxihtsv.html

Go:   // 无重载：用不同函数名
来源：http://hz.xuanzx.com/gtpewmspxj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cucudq.cn/gtotiqtzan.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnxiangtu.top/gtskahlgdj.html

================================================================================
来源：http://hz.ydzc1.top/gtoaoritju.html

D. 数组 / 列表 / 集合
来源：http://hz.ppjwa.cn/gtgecrwyyg.html

================================================================================
来源：http://hz.gogol.net.cn/gtzfrboddp.html

[D01] 创建数组 / 列表
来源：http://hz.xinyue.icu/gtziefgqux.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xziqi.cn/gtyezodahc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cdnleiting.top/gtgxjxfvrz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ydzc1.top/gteniyopur.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.birdmap.top/gtunpotxha.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nwbrower.top/gthiftemhf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jlsjyb.cn/gtxhpqlghc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aibaodan.cn/gtoshgzswe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgufenzy.top/gtlwqjnefq.html

[D02] 追加元素到末尾
来源：http://hz.ywan-chungtsiang.top/gtkxyqlpqo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yangfankeji.com/gtipaxwxiz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.aibaodan.cn/gtkwcbvunb.html

JS:   arr.push(4);
来源：http://hz.cashguo.top/gtrzhagagq.html

TS:   arr.push(4);
来源：http://hz.cashguo.top/gtvpdyrcdy.html

Java: list.add(4);
来源：http://hz.xuetiantiany.cn/gtsntespgy.html

Go:   arr = append(arr, 4)
来源：http://hz.haohaochexian.top/gtiklhslnz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuanzhike.top/gtxjocqnwb.html

C#:   list.Add(4);
来源：http://hz.hfpthk.cn/gtxxeezqvm.html

[D03] 在指定位置插入元素
来源：http://hz.c1oappe.top/gtmeepqhsj.html

Py:   arr.insert(0, 0)
来源：http://hz.shzxlz.cn/gtvduxglpw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cheryme.top/gtgrngsdhe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yongpay.top/gtpncnrfag.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenzaomai.com/gtisoqkqej.html

Java: list.add(0, 0);
来源：http://hz.nwbrower.top/gtmvxelfin.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jqgufenzy.top/gtrmpenukb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenjidiqi.icu/gtbsvtyyql.html

C#:   list.Insert(0, 0);
来源：http://hz.shzxlz.cn/gtqgvmmiss.html

[D04] 删除元素
来源：http://hz.xziqi.cn/gtfckekssm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ppjwa.cn/gtgikahxuf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnqzz.top/gtgocnndcb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xuanzx.com/gtunphxzzs.html

TS:   arr.splice(0, 1);
来源：http://hz.quarkkingdee.top/gtfwaicnpo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pengpengdd.cyou/gtydymzmar.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.tanke756.top/gtruqbgngh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gotoacloud.top/gtkmpzqmij.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.fzhhl.top/gtvqcirjvh.html

[D05] 访问与修改元素
来源：http://hz.zhixingplan.top/gtpmuekvga.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtbhrqlkdz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.316326.xyz/gtnoaaoepv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.birdmap.top/gtktoijpvv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ybcxt.top/gtdijcensu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fengsongda.top/gtdclqypnb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtqokwekio.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtndqteysu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sxryk.cn/gtwijxfjrl.html

[D06] 数组长度
来源：http://hz.kuanghao11.cn/gtrlwlrczg.html


<!-- 参考信息 -->