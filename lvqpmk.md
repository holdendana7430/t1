代发 wailian999

[B05] 遍历数组 / 列表
来源：http://hz.wangdashe.top/gtjzprzzrm.html

Py:   for item in arr: print(item)
来源：http://hz.feifeiyinyue.top/gtrdoarmzc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.sxryk.cn/gtyapnithq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hywenlv.cn/gtbgpcqxsg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sxryk.cn/gtkniteejd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yueranfly.top/gtpsxlcsmy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinyuanbaomall.cn/gtkxbyaknw.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jinyuanbaomall.cn/gtaiiljywk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhiwuduotai.top/gthggnuqwj.html

[B06] 遍历字典 / 对象
来源：http://hz.tianlin.xyz/gtgxwkjple.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zdqjudy.top/gtdzgaedly.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ppjwa.cn/gtcdagctrm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jianghu66.top/gtumncowfq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cheryme.top/gtvztjthqp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.fzhhl.top/gtiqqoferd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.cucudq.cn/gtvpdgoioa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.sufxvd.cn/gtrlbnfojr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.52xcode.cn/gtvzuctuus.html

[B07] while 循环
来源：http://hz.c1oappe.top/gtyaqypwkc.html

Py:   while i < 10: i += 1
来源：http://hz.ydjk.org.cn/gtuukbzmrn.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.wangshuangyany.cn/gtbbswqddf.html

JS:   while (i < 10) { i++; }
来源：http://hz.yj20258888.top/gtrcxmldxq.html

TS:   while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gtehgzrbqs.html

Java: while (i < 10) { i++; }
来源：http://hz.sweek.top/gtgfjcycrw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yj202588.top/gtrxhyloxo.html

Ruby: while i < 10; i += 1; end
来源：http://hz.nwbrower.top/gtmfbsxffz.html

C#:   while (i < 10) { i++; }
来源：http://hz.jqgfzy.top/gtmdentdjm.html

[B08] do-while（至少执行一次）
来源：http://hz.andypj.xyz/gtffkpielb.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yueranfly.top/gtvwojrtct.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhaomingkeji.xyz/gtbssmldrv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.fzhhl.top/gtbwxfzktz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.feifeiyinyue.top/gtvpavwtix.html

Java: do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtojcroqbl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhongyouzk.top/gtygvpxzjw.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hnqzz.top/gtdvxagxyn.html

C#:   do { i++; } while (i < 10);
来源：http://hz.nwbrower.top/gtlbtcamxh.html

[B09] break 与 continue
来源：http://hz.yj202588.top/gtnwfxsiiu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jinqigfzy.top/gtiwwknsly.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.gaohongyu789.top/gtgjhxwazo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydzc1.top/gtwnatboyt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnqzz.top/gtigqecvxt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.9152youxi.cn/gtopchhwbs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.chenjidiqi.icu/gtgrzjybvf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yonumen.top/gtybgxqjjo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangdashe.top/gthxorvxbf.html

[B10] 遍历同时拿索引
来源：http://hz.fengsongda.top/gtcnlmowrn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.tian-w.cn/gtmkiuhccu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hysaishi.cn/gtdrmxhdxx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.nwbrower.top/gtmandtoro.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hfpthk.cn/gtlatryjsb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.tian-w.cn/gtveluzrim.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yuanzhike.top/gtfrixjqxe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yj20258.top/gttpokorwm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhongyouzk.top/gtmwtwjilh.html

[B11] 生成数字序列 / 区间
来源：http://hz.nanxuanxn.top/gtsfaxowjm.html

Py:   list(range(0, 10, 2))
来源：http://hz.jqgufenzy.top/gtdavzosyp.html

PHP:  range(0, 10, 2);
来源：http://hz.zycfv.cn/gtqmsmjrsf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhengqikj.top/gtsfxedsqy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fzhhl.top/gtouvgetob.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yueranfly.top/gtevjbsbbz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xingfuxueyuan.xyz/gtglgzqwdp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.pycfn.com/gtjlqchbig.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.cheryme.top/gtzlapyvlr.html

[B12] 跳出多层循环
来源：http://hz.kuanghao11.cn/gthrrjpaqa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.feifeiyinyue.top/gtfsbpxxmj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yueranfly.top/gtvvermusn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shzxlz.cn/gtrzsdrlij.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtjblqbjqv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cheryme.top/gtcsrwakmg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jianghu66.top/gtqxjwclmq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.chenzaomai.com/gtlrbknrjy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.nanxinkj.top/gtkhjaydhj.html

[B13] 判断是否为数字
来源：http://hz.fengsongda.top/gtfgoreczd.html

Py:   isinstance(x, (int, float))
来源：http://hz.svipenyu.cn/gtkcgsfrjr.html

PHP:  is_numeric($x)
来源：http://hz.bjfxy.top/gtjwtanjkn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydjk.org.cn/gthgelhqcz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cdnleiting.top/gtjuxwsqpq.html

Java: x instanceof Number
来源：http://hz.zdqjudy.top/gtksqmvdrs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ehwqpu.com/gtzdldqotd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.svipenyu.cn/gtkjntnnhc.html

C#:   x is int or double or decimal
来源：http://hz.ybcxt.top/gtspartpbs.html

[B14] 判断值是否在集合内
来源：http://hz.hysaishi.cn/gttqaonvdl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.chenjidiqi.icu/gtjewcgkmx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhijiandao.cn/gtbujqkpbw.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shuidangran.top/gtgerjoobj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.c1oappe.top/gtmdkkavpt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.mhx1999.top/gtyhiugvme.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nwbrower.top/gtwszvilct.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cucudq.cn/gtnwctsayk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hysaishi.cn/gtjcghdcmj.html

[B15] 布尔运算与取反
来源：http://hz.cashguo.top/gtecfkirbj.html

Py:   a and b or not c
来源：http://hz.feifeiyinyue.top/gtwyexivlk.html

PHP:  $a && $b || !$c
来源：http://hz.nanxinkj.top/gtetculupe.html

JS:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtlabrvoce.html

TS:   a && b || !c
来源：http://hz.xuanzx.com/gtassxuliq.html

Java: a && b || !c
来源：http://hz.316326.xyz/gtwabrjpjg.html

Go:   a && b || !c
来源：http://hz.jlsjyb.cn/gtcftmrpuu.html

Ruby: a && b || !c
来源：http://hz.hammf.cn/gtpjegdont.html

C#:   a && b || !c
来源：http://hz.guannengcc.top/gtbobxhkaq.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shzxlz.cn/gtivycqyse.html

Py:   if not data: return
来源：http://hz.yonumen.top/gtavtkqfgh.html

PHP:  if (!$data) { return; }
来源：http://hz.fzhhl.top/gtxkpcbqov.html

JS:   if (!data) return;
来源：http://hz.tian-w.cn/gtakrjrvwl.html

TS:   if (!data) return;
来源：http://hz.zhengqikj.top/gtfmgdpqla.html

Java: if (data == null) return;
来源：http://hz.chenjidiqi.icu/gtisdfdtap.html

Go:   if data == nil { return }
来源：http://hz.redwolf501.top/gtwcurepvf.html

Ruby: return if data.nil?
来源：http://hz.shanyushiyangtech.top/gtfvdpadjy.html

C#:   if (data == null) return;
来源：http://hz.hfpthk.cn/gtoucvsctl.html

================================================================================
来源：http://hz.daria6918.cn/gtvflpvqfv.html

C. 函数与作用域
来源：http://hz.jinghuilouyu.cn/gtrlyadwth.html

================================================================================
来源：http://hz.guannengcc.top/gtzzjrowan.html

[C01] 定义函数
来源：http://hz.zhixingplan.top/gtvslysyzr.html

Py:   def add(a, b): return a + b
来源：http://hz.zhaomingkeji.xyz/gthdzakxpg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gtxpujxhlt.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.sufxvd.cn/gtkelgkjkg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtztkaggim.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinqigfzy.top/gtyvhvibid.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yj20258.top/gtfspoqscu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.bjfxy.top/gtpbwttywh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtgniuflev.html

[C02] 默认参数
来源：http://hz.9152youxi.cn/gtaetxkgba.html

Py:   def greet(name="World"): return name
来源：http://hz.jlsjyb.cn/gtewkxtdsp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhaomingkeji.xyz/gtwtfwyizy.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zycfv.cn/gtevcbyarp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ivvv.top/gthdtepklr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jyoumei.cn/gtkuhzygql.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.pycfn.com/gtqlerpwlv.html

Ruby: def greet(name = "World") = name
来源：http://hz.aibaodan.cn/gtqdshvidh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yuxming.cn/gtnnbuvjvr.html

[C03] 可变参数
来源：http://hz.xinyue.icu/gtlfadojqv.html

Py:   def total(*args): return sum(args)
来源：http://hz.yuxming.cn/gtrcdvzphd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.havefunace.top/gtjxyburrw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dianchejie.cn/gtnjkxoolw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gtotqykosh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shzxlz.cn/gthntxenqj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.pycfn.com/gtqutizkwd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sufxvd.cn/gtjliqrmyn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydjk.org.cn/gtusgvufar.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cashguo.top/gtvkyggnht.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jqgufenzy.top/gtiaqjmavc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj202588.top/gtvfdvkjnw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jqgfzy.top/gtrotctzrt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sysykeji.top/gtlnmkbvkj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yangfankeji.com/gtwzqtldqp.html

Go:   // 无：用配置结构体参数
来源：http://hz.ivvv.top/gtlwuzvkim.html

Ruby: f(a: 1, b: 2)
来源：http://hz.dashuyun.cn/gtrjfcyxis.html

C#:   f(a: 1, b: 2)
来源：http://hz.316326.xyz/gtwbifnahj.html

[C05] 返回多个值
来源：http://hz.nanxinkj.top/gtufwwzegg.html

Py:   return a, b
来源：http://hz.hnxiangtu.top/gtbpcabojf.html

PHP:  return [$a, $b];
来源：http://hz.cashguo.top/gtqigpbhlu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.nanxuanxn.top/gtdrnynkub.html

TS:   return { a, b };
来源：http://hz.zhiwuduotai.top/gtpijzmpbm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cucudq.cn/gtyjmfjjia.html

Go:   return a, b
来源：http://hz.yanxiufei.cn/gttlrpnyhc.html

Ruby: return a, b
来源：http://hz.hysaishi.cn/gtpvommbjw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yueranfly.top/gtayklnwxx.html

[C06] 匿名函数 / lambda
来源：http://hz.gogol.net.cn/gtqnfvxnor.html

Py:   square = lambda x: x * x
来源：http://hz.52xcode.cn/gtmhnbubfp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.meibo888.top/gtpcdocxhj.html

JS:   const square = x => x * x;
来源：http://hz.yvedp.cn/gtnaowtxdg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sxryk.cn/gtrzamznbs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ywan-chungtsiang.top/gtclfmpxeu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhoulong.xyz/gtjarrbnrw.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xylfe.cn/gtecyerqjn.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sweek.top/gtzabvevfa.html

[C07] 把函数作为参数传入
来源：http://hz.ivvv.top/gtjtfqejif.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.52xcode.cn/gtzjkefpiv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jlsjyb.cn/gtonqywdwp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.chenlongwang.top/gtpaxidyym.html

TS:   arr.map(String)
来源：http://hz.chenjidiqi.icu/gtcsxdzrdp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.dianchejie.cn/gtgrbnxfug.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.c1oappe.top/gtxlheteat.html

Ruby: arr.map(&:upcase)
来源：http://hz.zycfv.cn/gtcyfczcsk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.birdmap.top/gtyuunqjjm.html

[C08] 闭包
来源：http://hz.cheryme.top/gtxzbicklq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhijiandao.cn/gthtrxmmiu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.fengsongda.top/gthgclfscc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.svipenyu.cn/gtrcyylqfx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shanyushiyangkeji.top/gtfodsqwoh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.haohaochexian.top/gtonhqbjdz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.smart0.xyz/gttloctale.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.havefunace.top/gtqgmyukno.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gtjzriayow.html

[C09] 递归
来源：http://hz.guannengcc.top/gtmsirvxgj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jianghu66.top/gtgjfpvomf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jlsjyb.cn/gtnmqqnahs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.52xcode.cn/gtgzevqctj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shangyingyoupin.top/gtetsaidsq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.nwbrower.top/gtdgkpnpux.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jqgfzy.top/gtdwkgvrur.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hnqzz.top/gtrlbkgwab.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ppjwa.cn/gtuzmcdkwm.html

[C10] 变量作用域
来源：http://hz.yvedp.cn/gtwldamgtx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ppjwa.cn/gtaroironj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cucudq.cn/gtgpwpfpaq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jianghu66.top/gtlihbkjxq.html

TS:   同 JS
来源：http://hz.jlsjyb.cn/gtstachhyp.html

Java: 方法内为块级作用域
来源：http://hz.yueranfly.top/gtxiccuypt.html

Go:   花括号块级作用域
来源：http://hz.xylfe.cn/gtcfrivkqn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ydzc1.top/gtipvffjnj.html

C#:   块级作用域
来源：http://hz.gogol.net.cn/gtfpciospq.html

[C11] 模块导入与导出
来源：http://hz.chenjidiqi.icu/gtxbfkxazv.html

Py:   from module import func
来源：http://hz.dashuyun.cn/gtvdgbxjdh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hywenlv.cn/gtmveoehxz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.wangshuangyany.cn/gtdhvrqihx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.andypj.xyz/gtczbekjpd.html

Java: import java.util.List;
来源：http://hz.daria6918.cn/gtlnqcmrzw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cqqwz.cn/gtdevwehik.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xuetiantiany.cn/gtjhkrgyoy.html

C#:   using System.Text;
来源：http://hz.daxiang520.top/gtcptcueds.html

[C12] 立即执行函数 IIFE
来源：http://hz.hammf.cn/gtmfelmiuq.html

Py:   (lambda: print("run"))()
来源：http://hz.9152youxi.cn/gtytjxxggo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigfzy.top/gtmotusrib.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xinyue.icu/gtziaayzfo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtkanzpbih.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.wangshuangyany.cn/gtmsvrvads.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.guannengcc.top/gtxzhoaset.html

Ruby: -> { puts "run" }.call
来源：http://hz.bjfxy.top/gtgljtiivw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuanzhike.top/gtfpnyprpi.html

[C13] 类型声明 / 类型注解
来源：http://hz.redwolf501.top/gtetxbslvb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xziqi.cn/gtyuevelve.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtxyujgslv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gzhubu.top/gtkwerorcw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xylfe.cn/gtootkocyy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtzxkiczsu.html

Go:   func add(a, b int) int
来源：http://hz.yangfankeji.com/gtfyagoinp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhengqikj.top/gtxloxoajq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xylfe.cn/gtonekzscq.html

[C14] 泛型函数
来源：http://hz.iojbl.cn/gtycabjyih.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xylfe.cn/gtvkwbzbnd.html

PHP:  // 无泛型
来源：http://hz.sxryk.cn/gtfebzihnu.html

JS:   // 无泛型
来源：http://hz.hnqzz.top/gtheikizew.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gzhubu.top/gtjziwlyer.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhiwuduotai.top/gtjsvpyvhg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xziqi.cn/gtnxiqvkaj.html

Ruby: # 无泛型
来源：http://hz.yanxiufei.cn/gtsopnjdva.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.quarkkingdee.top/gtwfwuuahe.html

[C15] 解构 / 展开参数
来源：http://hz.yvedp.cn/gtxpqhymhw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yangfankeji.com/gttwwjbzkc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jinyuanbaomall.cn/gtnvlcysva.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yongpay.top/gtfazvhiqz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dashuyun.cn/gtfgprrcze.html

Java: // 无解构
来源：http://hz.yj202588.top/gtkahzjwys.html

Go:   // 无解构
来源：http://hz.chenlongwang.top/gtmwmekagh.html

Ruby: a, b = pair
来源：http://hz.xuetiantiany.cn/gtjgjwidri.html

C#:   var (a, b) = pair;
来源：http://hz.hywenlv.cn/gtazlcaxoj.html

[C16] 函数 / 方法重载
来源：http://hz.hywenlv.cn/gtlpkonurn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhixingplan.top/gtgvdsmmmn.html

PHP:  // 无重载
来源：http://hz.jianghu66.top/gtfgabydov.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigufen.top/gtmjbedplr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yuxming.cn/gtouwvdgwl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenjidiqi.icu/gtyrysjkxf.html

Go:   // 无重载：用不同函数名
来源：http://hz.birdmap.top/gtuuutveqi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.fengsongda.top/gtaribfuft.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zycfv.cn/gtyebjwaze.html

================================================================================
来源：http://hz.zhoulong.xyz/gtqopdiefp.html

D. 数组 / 列表 / 集合
来源：http://hz.meibo888.top/gtxtkkphhb.html

================================================================================
来源：http://hz.nwbrower.top/gtmxmttswg.html

[D01] 创建数组 / 列表
来源：http://hz.ydzc1.top/gtdcpfjjjc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tian-w.cn/gtfiuankaj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ppjwa.cn/gtyrzhrkys.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.snrcjt.cn/gttsggxxfx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xinyue.icu/gtpkcfkmit.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.fzhhl.top/gtkkidoqmi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yangfankeji.com/gtdjmgfbjt.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gtbwotlndm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.pycfn.com/gtszjtqhug.html

[D02] 追加元素到末尾
来源：http://hz.pengpengdd.cyou/gtmhdodpou.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nwbrower.top/gtkwsfhjxj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jianghu66.top/gtcylwwwyf.html

JS:   arr.push(4);
来源：http://hz.ehwqpu.com/gtftovpcwh.html

TS:   arr.push(4);
来源：http://hz.gzhubu.top/gtvekueofe.html

Java: list.add(4);
来源：http://hz.kuanghao11.cn/gtlrtmkavu.html

Go:   arr = append(arr, 4)
来源：http://hz.gzhubu.top/gtqsmsclfn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.vqdsnc.cn/gtsysgyqik.html

C#:   list.Add(4);
来源：http://hz.c1oappe.top/gtxbswwznt.html

[D03] 在指定位置插入元素
来源：http://hz.gotoacloud.top/gtgoytpxtr.html

Py:   arr.insert(0, 0)
来源：http://hz.xuanzx.com/gtnsstbatt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xuetiantiany.cn/gtfwunhlub.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cucudq.cn/gtukvjfyci.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gotoacloud.top/gtiyhavwap.html

Java: list.add(0, 0);
来源：http://hz.jinqigfzy.top/gtenoyexlz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.tian-w.cn/gtdzleiyjw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.dianchejie.cn/gtloixfjnh.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxuanxn.top/gtsyzojsmg.html

[D04] 删除元素
来源：http://hz.hnxiangtu.top/gtyaqrkdwm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuxming.cn/gttiaauinc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinqigfzy.top/gtxbfgywxb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenzaomai.com/gtkmhveual.html

TS:   arr.splice(0, 1);
来源：http://hz.yj202588.top/gtrdnifjin.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ybcxt.top/gtqludjdrj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hfpthk.cn/gtwesfsxtl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xylfe.cn/gtlpebyrow.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.fzhhl.top/gtotipmxbt.html

[D05] 访问与修改元素
来源：http://hz.cdnleiting.top/gtgbrakdeh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ehwqpu.com/gtucfodrfx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cheryme.top/gtspnbukga.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtqtgwtgpx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hysaishi.cn/gtzcgsxbqe.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yangfankeji.com/gtolfifagq.html


<!-- 参考信息 -->