代发 wailian999

[B05] 遍历数组 / 列表
来源：http://hz.ywan-chungtsiang.top/gtcauuhkhi.html

Py:   for item in arr: print(item)
来源：http://hz.yueranfly.top/gtgqqozvhw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.svipenyu.cn/gtfabdxnky.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ywan-chungtsiang.top/gtmccmsrsu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.mhx1999.top/gtpcgnbihl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.gaohongyu789.top/gtvjphvnei.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hfpthk.cn/gtrfqamjpn.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ydjk.org.cn/gtgheqtsqv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yj20258.top/gthzbxatdp.html

[B06] 遍历字典 / 对象
来源：http://hz.yuxming.cn/gtxanvdorl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yongpay.top/gtjyefueyl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.zdqjudy.top/gtetsneged.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.guannengcc.top/gtcicuezjr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cashguo.top/gtqvvkfmkb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.bjfxy.top/gtljxrqjyg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hammf.cn/gtdflyuzrf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jyoumei.cn/gtumkeqqjh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.meibo888.top/gtbmkiezde.html

[B07] while 循环
来源：http://hz.redwolf501.top/gthpmutaft.html

Py:   while i < 10: i += 1
来源：http://hz.c1oappe.top/gtbxmjxxva.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.sweek.top/gtgykgpkhr.html

JS:   while (i < 10) { i++; }
来源：http://hz.quarkkingdee.top/gtvdbsgskm.html

TS:   while (i < 10) { i++; }
来源：http://hz.cucudq.cn/gtbboamwhz.html

Java: while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gttzqiwqoy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhiwuduotai.top/gtjolexsrm.html

Ruby: while i < 10; i += 1; end
来源：http://hz.9152youxi.cn/gtdbohioin.html

C#:   while (i < 10) { i++; }
来源：http://hz.bjfxy.top/gtzsjgwkkx.html

[B08] do-while（至少执行一次）
来源：http://hz.bjfxy.top/gtxleuucxi.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhengqikj.top/gtcxkuyudo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.svipenyu.cn/gttbbilmdw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.tianlin.xyz/gtyjrdjqtl.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gtznrykwzi.html

Java: do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtrdfyemdx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.gaohongyu789.top/gtzufcwnmr.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.pengpengdd.cyou/gtwnqmmbal.html

C#:   do { i++; } while (i < 10);
来源：http://hz.nanxinkj.top/gtrhfybscy.html

[B09] break 与 continue
来源：http://hz.meibo888.top/gtyysnwszf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.9152youxi.cn/gtjvepkbtr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shuidangran.top/gtogtkxqwy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.andypj.xyz/gtpjemavkm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtcndufmvj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxuanxn.top/gtqqhlritd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.cqqwz.cn/gtqssjhpjm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.chenzaomai.com/gtidcglukn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gtzigkyexu.html

[B10] 遍历同时拿索引
来源：http://hz.redwolf501.top/gtoklzdsck.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhiwuduotai.top/gtewgacbtk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hywenlv.cn/gtihuedngr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.tanke756.top/gtitobeyxt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.gaohongyu789.top/gtgpsqokzf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.nanxuanxn.top/gtqdeofwss.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shangyingyoupin.top/gtzhubpsvx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.316326.xyz/gtwexvbiuf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.dashuyun.cn/gtbpvdtmdh.html

[B11] 生成数字序列 / 区间
来源：http://hz.kuanghao11.cn/gtuhhtkvqc.html

Py:   list(range(0, 10, 2))
来源：http://hz.xuetiantiany.cn/gtvvzlxdxt.html

PHP:  range(0, 10, 2);
来源：http://hz.birdmap.top/gtrelckmkq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ydjk.org.cn/gtrzlkgcyl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yueranfly.top/gttubpieqk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cashguo.top/gtqxervzcb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.havefunace.top/gtbjtkrxiu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.pycfn.com/gtyjrbcefd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.iojbl.cn/gtdycquhrv.html

[B12] 跳出多层循环
来源：http://hz.mhx1999.top/gtrgmsaudn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.pengpengdd.cyou/gthnmywyls.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hysaishi.cn/gtgiqeknvl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtewxmctnl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gtrsieajvn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangkeji.top/gtfqpwmlre.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj20258888.top/gtjykxqfkb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.wangdashe.top/gtmjqnaftv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jqgfzy.top/gtfqlbgjqr.html

[B13] 判断是否为数字
来源：http://hz.jqgfzy.top/gtmrbfwejw.html

Py:   isinstance(x, (int, float))
来源：http://hz.meibo888.top/gtipkezyjx.html

PHP:  is_numeric($x)
来源：http://hz.gotoacloud.top/gttpkqurkg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hnqzz.top/gtnngqfhgw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.redwolf501.top/gtrsurvwou.html

Java: x instanceof Number
来源：http://hz.zhixingplan.top/gthkvzmhun.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhaomingkeji.xyz/gtjtmwjibx.html

Ruby: x.is_a?(Numeric)
来源：http://hz.gzhubu.top/gtxsbjkqst.html

C#:   x is int or double or decimal
来源：http://hz.meibo888.top/gtmzhalqsu.html

[B14] 判断值是否在集合内
来源：http://hz.guannengcc.top/gtuhlbtgav.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sysykeji.top/gtusfuljlo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jianghu66.top/gtzotdwdts.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.andypj.xyz/gtreejiqbf.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.wangdashe.top/gtohpjaoot.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinyuanbaomall.cn/gtdczdcjjd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.tanke756.top/gtjlglyvgf.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhijiandao.cn/gtvtuvydzu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yueranfly.top/gtrtkvxebc.html

[B15] 布尔运算与取反
来源：http://hz.zhengqikj.top/gtufsoxzjg.html

Py:   a and b or not c
来源：http://hz.cheryme.top/gtkgrvpnvv.html

PHP:  $a && $b || !$c
来源：http://hz.jinqigfzy.top/gtjuwicryt.html

JS:   a && b || !c
来源：http://hz.52xcode.cn/gtasyhxbnj.html

TS:   a && b || !c
来源：http://hz.vqdsnc.cn/gtfbcvinfn.html

Java: a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtychorpvx.html

Go:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtkqyschmn.html

Ruby: a && b || !c
来源：http://hz.gzhubu.top/gtxnchkoau.html

C#:   a && b || !c
来源：http://hz.vqdsnc.cn/gtrkenwrbq.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.wangdashe.top/gtdufliqhh.html

Py:   if not data: return
来源：http://hz.xuanzx.com/gtafztebra.html

PHP:  if (!$data) { return; }
来源：http://hz.hfpthk.cn/gtdxbvqilh.html

JS:   if (!data) return;
来源：http://hz.yanxiufei.cn/gtyljwpdmq.html

TS:   if (!data) return;
来源：http://hz.iojbl.cn/gtkvisfdgs.html

Java: if (data == null) return;
来源：http://hz.0kj1m.cn/gtmxjaexor.html

Go:   if data == nil { return }
来源：http://hz.aibaodan.cn/gtbuffclvg.html

Ruby: return if data.nil?
来源：http://hz.316326.xyz/gtqrdtsloa.html

C#:   if (data == null) return;
来源：http://hz.bjfxy.top/gtvfnfgedl.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcjjxevyj.html

C. 函数与作用域
来源：http://hz.wangshuangyany.cn/gtxwcpgdga.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtttdvrvjx.html

[C01] 定义函数
来源：http://hz.yongpay.top/gtrozdgzqe.html

Py:   def add(a, b): return a + b
来源：http://hz.havefunace.top/gtzhjjyawo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtwyrbxlgo.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.bjfxy.top/gtughxzwvn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtczgjvkaf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gturokypde.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.dianchejie.cn/gtbjtkrgtb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.aibaodan.cn/gtuwfzcddl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtortfqtsu.html

[C02] 默认参数
来源：http://hz.gotoacloud.top/gtbvrdnzki.html

Py:   def greet(name="World"): return name
来源：http://hz.xuanzx.com/gtfhjqhgum.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yj20258888.top/gthnujpxyb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nwbrower.top/gtjleerrri.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.nanxinkj.top/gttnndvjvq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhixingplan.top/gtakacvjdx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ivvv.top/gtvttqzmus.html

Ruby: def greet(name = "World") = name
来源：http://hz.birdmap.top/gthzkhmhqd.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nanxinkj.top/gtghctqsmd.html

[C03] 可变参数
来源：http://hz.jlsjyb.cn/gtfllzuixl.html

Py:   def total(*args): return sum(args)
来源：http://hz.xuetiantiany.cn/gtbkijnvkm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhengqikj.top/gtwbqltzzg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.52xcode.cn/gtgodzhiox.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhixingplan.top/gtglyggxps.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yj20258888.top/gthlozxmga.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tanke756.top/gtssnkibzp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.svipenyu.cn/gtzzbalbyh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.0kj1m.cn/gtkgwnplue.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xziqi.cn/gtppjiyazl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhoulong.xyz/gtkiimcayq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gotoacloud.top/gtsglmblzg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jiagoushi.top/gtzgtallpb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ybcxt.top/gtlywoxwuy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jqgufenzy.top/gtjjtpxkiu.html

Go:   // 无：用配置结构体参数
来源：http://hz.tanke756.top/gtojbizalg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cheryme.top/gtcqsowrjc.html

C#:   f(a: 1, b: 2)
来源：http://hz.daxiang520.top/gtuduwvsvy.html

[C05] 返回多个值
来源：http://hz.iojbl.cn/gthelmcapo.html

Py:   return a, b
来源：http://hz.jqgfzy.top/gtaeucljjk.html

PHP:  return [$a, $b];
来源：http://hz.wangshuangyany.cn/gtkrjldqdp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sysykeji.top/gtgeervxmz.html

TS:   return { a, b };
来源：http://hz.andypj.xyz/gtdohofvnz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.andypj.xyz/gtzblnyvao.html

Go:   return a, b
来源：http://hz.gzhubu.top/gtjveiqoxp.html

Ruby: return a, b
来源：http://hz.dianchejie.cn/gteoqjjuvb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.chenjidiqi.icu/gtaikvvtbt.html

[C06] 匿名函数 / lambda
来源：http://hz.yueranfly.top/gthnmdibqr.html

Py:   square = lambda x: x * x
来源：http://hz.shuidangran.top/gtvzcsuxwk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tian-w.cn/gtagoawrba.html

JS:   const square = x => x * x;
来源：http://hz.andypj.xyz/gtapmtjfjx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.aibaodan.cn/gtetrtakot.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sweek.top/gtfbvbpvto.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhengqikj.top/gtjuidajis.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhijiandao.cn/gtitfhscmz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinghuilouyu.cn/gtbptcvvgl.html

[C07] 把函数作为参数传入
来源：http://hz.cdnleiting.top/gteebpdame.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tian-w.cn/gtjqkaubls.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jqgfzy.top/gtlvuexkww.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ehwqpu.com/gtxtvoahjc.html

TS:   arr.map(String)
来源：http://hz.jiagoushi.top/gthwfpdagv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhiwuduotai.top/gtynnnaqtn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangkeji.top/gtkibttcfm.html

Ruby: arr.map(&:upcase)
来源：http://hz.kuanghao11.cn/gtrmhgjqow.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.snrcjt.cn/gtrpjxfgiy.html

[C08] 闭包
来源：http://hz.zhijiandao.cn/gtiqjafpjx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xziqi.cn/gtpvsehudx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhijiandao.cn/gttafbkais.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gtntlaplmo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gtrrgjgcgf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gzhubu.top/gtjbkqpfdh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.fzhhl.top/gtngyerwjs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shanyushiyangkeji.top/gtpknrgvmh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gthboqmhyd.html

[C09] 递归
来源：http://hz.andypj.xyz/gtsutltgzf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xinyue.icu/gtqxtrnugv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yuanzhike.top/gtwsuvvvof.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gtimkpickn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hammf.cn/gtwqbrqxzh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.feifeiyinyue.top/gtyovazqxp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shuidangran.top/gtmbeensrt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zdqjudy.top/gthrsawysh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.guowangkeji.top/gtyctjhvqm.html

[C10] 变量作用域
来源：http://hz.yj20258.top/gtowpqbyyx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.52xcode.cn/gtmgzawaqc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yongpay.top/gtgjuqmojd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.haohaochexian.top/gtobntukzj.html

TS:   同 JS
来源：http://hz.zdqjudy.top/gtwohrrflw.html

Java: 方法内为块级作用域
来源：http://hz.sweek.top/gtiptauvvi.html

Go:   花括号块级作用域
来源：http://hz.hammf.cn/gthdlrhuhk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.316326.xyz/gtomcojwms.html

C#:   块级作用域
来源：http://hz.tianlin.xyz/gtngtxxufa.html

[C11] 模块导入与导出
来源：http://hz.jinyuanbaomall.cn/gtroqabuhf.html

Py:   from module import func
来源：http://hz.yueranfly.top/gtbiiwtlbz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj202588.top/gtubpnthmv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.haohaochexian.top/gtoprwjacf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhiwuduotai.top/gtoggckwks.html

Java: import java.util.List;
来源：http://hz.zhixingplan.top/gtmelhgsyp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gogol.net.cn/gtnynwepia.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cheryme.top/gthtjjeglu.html

C#:   using System.Text;
来源：http://hz.jiagoushi.top/gtwmgvsljo.html

[C12] 立即执行函数 IIFE
来源：http://hz.hammf.cn/gtkukxvjkz.html

Py:   (lambda: print("run"))()
来源：http://hz.yj20258888.top/gtjentqrzp.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ehwqpu.com/gtkubtjfsl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gtwvjorero.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gtvmlyetmi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinghuilouyu.cn/gtnekpxnwy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yuanzhike.top/gtyxukjtjx.html

Ruby: -> { puts "run" }.call
来源：http://hz.haohaochexian.top/gtcjcrtxcd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.aizwys.cn/gtoecgmawl.html

[C13] 类型声明 / 类型注解
来源：http://hz.kuanghao11.cn/gtodilixal.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.bjfxy.top/gtdpcikrlr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtgzwnqmdh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hfpthk.cn/gtlrvnsdsw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dianchejie.cn/gtosxlupsx.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtwrjvjuoy.html

Go:   func add(a, b int) int
来源：http://hz.bjfxy.top/gteadtgvhf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shzxlz.cn/gtowteodma.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jiagoushi.top/gtirsdxbim.html

[C14] 泛型函数
来源：http://hz.tanke756.top/gtcmfdpfzn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.aizwys.cn/gthyyvqtlz.html

PHP:  // 无泛型
来源：http://hz.kuanghao11.cn/gtmnmpqpfh.html

JS:   // 无泛型
来源：http://hz.hnqzz.top/gtgrtgrshk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yuanzhike.top/gtfhvhgfwy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhoulong.xyz/gtqxbroynx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.316326.xyz/gtdzkkvwej.html

Ruby: # 无泛型
来源：http://hz.gotoacloud.top/gtehzmebgd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhiwuduotai.top/gtjyaofuzh.html

[C15] 解构 / 展开参数
来源：http://hz.sweek.top/gtiyitecnq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.quarkkingdee.top/gtzcncrnmd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenzaomai.com/gtbphwqfbn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yvedp.cn/gtfgckzxek.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinghuilouyu.cn/gtfjehotgi.html

Java: // 无解构
来源：http://hz.cqqwz.cn/gtsmazfyrr.html

Go:   // 无解构
来源：http://hz.gotoacloud.top/gttloxprdo.html

Ruby: a, b = pair
来源：http://hz.ydzc1.top/gtgaddzavr.html

C#:   var (a, b) = pair;
来源：http://hz.kuanghao11.cn/gtleixbvfd.html

[C16] 函数 / 方法重载
来源：http://hz.smart0.xyz/gtfbvwwvla.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hysaishi.cn/gtvjrraxwx.html

PHP:  // 无重载
来源：http://hz.chenzaomai.com/gtojcvmisy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zycfv.cn/gtansepidw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cqqwz.cn/gtodcrsruf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenlongwang.top/gtdspnrfgr.html

Go:   // 无重载：用不同函数名
来源：http://hz.shuidangran.top/gtsdjhyyco.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnxiangtu.top/gtxwwuvqhk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xuanzx.com/gtbfnespil.html

================================================================================
来源：http://hz.tian-w.cn/gtjsaxmvna.html

D. 数组 / 列表 / 集合
来源：http://hz.ywan-chungtsiang.top/gtrwuoweaz.html

================================================================================
来源：http://hz.hysaishi.cn/gtevligjbx.html

[D01] 创建数组 / 列表
来源：http://hz.ydjk.org.cn/gtcvhqeqkw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.smart0.xyz/gtutzugnrw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinqigufen.top/gtbwxsbpdx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.iojbl.cn/gtskefjpfu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.fzhhl.top/gtmiaxlgdx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhijiandao.cn/gtjoznwlqi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cashguo.top/gtsepggfsh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hfpthk.cn/gtmiziplrr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.guannengcc.top/gttjwbrugn.html

[D02] 追加元素到末尾
来源：http://hz.jlsjyb.cn/gtrlidlthw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.haohaochexian.top/gtjklchcqt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.tanke756.top/gtdqdkwxcf.html

JS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtxyrdnopc.html

TS:   arr.push(4);
来源：http://hz.jinghuilouyu.cn/gtiyfuxdgr.html

Java: list.add(4);
来源：http://hz.shanyushiyangtech.top/gtiayagskz.html

Go:   arr = append(arr, 4)
来源：http://hz.hnxiangtu.top/gtoyqnxubn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ydjk.org.cn/gtwfnqeshh.html

C#:   list.Add(4);
来源：http://hz.sweek.top/gtckvhjyhx.html

[D03] 在指定位置插入元素
来源：http://hz.vqdsnc.cn/gtxxppvflb.html

Py:   arr.insert(0, 0)
来源：http://hz.yvedp.cn/gtynytimvn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.kuanghao11.cn/gtorfxbnif.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.redwolf501.top/gtlgfeawcm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.havefunace.top/gtuyeubdlf.html

Java: list.add(0, 0);
来源：http://hz.yj20258888.top/gtuxpyxplo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.snrcjt.cn/gtdmshstfb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gotoacloud.top/gtrdgpcgtc.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxuanxn.top/gtukzunted.html

[D04] 删除元素
来源：http://hz.jlsjyb.cn/gtgloihtci.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.vqdsnc.cn/gtopgvfqqh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gzhubu.top/gtzsvprekj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xinyue.icu/gtsljwfjgq.html

TS:   arr.splice(0, 1);
来源：http://hz.xuanzx.com/gtruzibbjv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pycfn.com/gtbdqhsgbt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hysaishi.cn/gtvtmjrndk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.pycfn.com/gtrpsufwju.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinghuilouyu.cn/gtgpcaycpn.html

[D05] 访问与修改元素
来源：http://hz.daria6918.cn/gtkfnqfbcj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtpumupkfe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhengqikj.top/gttqzuhndv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sxryk.cn/gtkbxkmndw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sufxvd.cn/gtvgbzkmxe.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.havefunace.top/gtnivxowrz.html


<!-- 参考信息 -->