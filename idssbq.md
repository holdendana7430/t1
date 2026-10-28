代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhixingplan.top/gtslhldeop.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.fzhhl.top/gtnpsltsvm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.chenlongwang.top/gtoessfxht.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jinyuanbaomall.cn/gtjzrkucgg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yj202588.top/gtahptfttd.html

[B06] 遍历字典 / 对象
来源：http://hz.shuidangran.top/gtwffpizmf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.tian-w.cn/gtphuucirl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.gzhubu.top/gtokakvvnj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.iojbl.cn/gtrubiqtdk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jqgufenzy.top/gtawgmauvc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.dashuyun.cn/gtnxhlgwfa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.redwolf501.top/gtfzxhgnyp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xuetiantiany.cn/gtgbvpnxxo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zdqjudy.top/gtiycxbkar.html

[B07] while 循环
来源：http://hz.hywenlv.cn/gtprmxfapb.html

Py:   while i < 10: i += 1
来源：http://hz.daxiang520.top/gtfgidjxcf.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.mhx1999.top/gtnzqzdhka.html

JS:   while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtswxwdbij.html

TS:   while (i < 10) { i++; }
来源：http://hz.hysaishi.cn/gtdhqtekev.html

Java: while (i < 10) { i++; }
来源：http://hz.zdqjudy.top/gtqgaptrnx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.c1oappe.top/gtuusfcgrz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.cqqwz.cn/gtlrbrduej.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinghuilouyu.cn/gtleejzcoq.html

[B08] do-while（至少执行一次）
来源：http://hz.hnqzz.top/gtnxigxgko.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.guannengcc.top/gtsqbwfsep.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hnxiangtu.top/gtzbxsizsf.html

JS:   do { i++; } while (i < 10);
来源：http://hz.chenlongwang.top/gtvwvrmxrl.html

TS:   do { i++; } while (i < 10);
来源：http://hz.9152youxi.cn/gtsldrtlbq.html

Java: do { i++; } while (i < 10);
来源：http://hz.birdmap.top/gtzxcqqvqu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.gaohongyu789.top/gttvtdeurt.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jinghuilouyu.cn/gteqcfoqhg.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gtophtchns.html

[B09] break 与 continue
来源：http://hz.jlsjyb.cn/gtgasaqzrl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.iojbl.cn/gtijlcculc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.svipenyu.cn/gtpqrvjwho.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gtjogknsov.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gtdxidtocc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xylfe.cn/gtidlczaiy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.chenzaomai.com/gtngyquuwr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xuetiantiany.cn/gtvlalkxbi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gtolnhdiav.html

[B10] 遍历同时拿索引
来源：http://hz.shanyushiyangkeji.top/gtwknekfkw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhijiandao.cn/gtqypvvccd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhongyouzk.top/gteiqagxsg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shzxlz.cn/gtwjgvusvi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shzxlz.cn/gtimlttgrx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhijiandao.cn/gtcsiwaqcn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhixingplan.top/gtudxcfump.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yangfankeji.com/gtpgaxnmri.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.birdmap.top/gtnlvoqqki.html

[B11] 生成数字序列 / 区间
来源：http://hz.ehwqpu.com/gtvraxmnmj.html

Py:   list(range(0, 10, 2))
来源：http://hz.dashuyun.cn/gtnkwzkwcg.html

PHP:  range(0, 10, 2);
来源：http://hz.yuxming.cn/gtasbbidsi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhoulong.xyz/gtjmhrxuqk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xuetiantiany.cn/gtawkxcgry.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shanyushiyangtech.top/gtxowmgysu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.vqdsnc.cn/gtnuxdafqy.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ywan-chungtsiang.top/gtjwbtjvtm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xingfuxueyuan.xyz/gtutffzycb.html

[B12] 跳出多层循环
来源：http://hz.yvedp.cn/gtfoatypop.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sysykeji.top/gtjcojqhlf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hysaishi.cn/gtjnthzdsv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gzhubu.top/gtszmcofyv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.birdmap.top/gtdqegekzt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.fengsongda.top/gtwkicsdkj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xinyue.icu/gtjrtfycmj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zycfv.cn/gtbxlfkmkv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hongshengwenyu.top/gtgyjlozdo.html

[B13] 判断是否为数字
来源：http://hz.shanyushiyangtech.top/gtbaqrjbxs.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinqigfzy.top/gtnrhupbuu.html

PHP:  is_numeric($x)
来源：http://hz.chenzaomai.com/gtuyajyjzr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jiagoushi.top/gtvmjgmtww.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhiwuduotai.top/gtpytpacbo.html

Java: x instanceof Number
来源：http://hz.aizwys.cn/gtoitemddx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yanxiufei.cn/gtdinewknd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.daria6918.cn/gtplmpviyl.html

C#:   x is int or double or decimal
来源：http://hz.cdnleiting.top/gtdbviapyu.html

[B14] 判断值是否在集合内
来源：http://hz.havefunace.top/gtjzbkaext.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jyoumei.cn/gtvbhkebga.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.c1oappe.top/gtiexbxygq.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shuidangran.top/gtyvzwjmyw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guowangkeji.top/gtsrvsawxk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ehwqpu.com/gtxbormvdc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhongyouzk.top/gtdatkhkar.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cheryme.top/gtbhdmniat.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.kuanghao11.cn/gtujkctnis.html

[B15] 布尔运算与取反
来源：http://hz.xziqi.cn/gtfbxtzbks.html

Py:   a and b or not c
来源：http://hz.ppjwa.cn/gtezginync.html

PHP:  $a && $b || !$c
来源：http://hz.hnqzz.top/gtpzlrbywv.html

JS:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtdwtewgkm.html

TS:   a && b || !c
来源：http://hz.jinqigfzy.top/gtpzrcmcut.html

Java: a && b || !c
来源：http://hz.0kj1m.cn/gtuivuqvqc.html

Go:   a && b || !c
来源：http://hz.ehwqpu.com/gtyjtcbjvn.html

Ruby: a && b || !c
来源：http://hz.jqgfzy.top/gtroqxklmt.html

C#:   a && b || !c
来源：http://hz.gzhubu.top/gtodgotpfn.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jlsjyb.cn/gtinsnvove.html

Py:   if not data: return
来源：http://hz.gzhubu.top/gtigsyeyjw.html

PHP:  if (!$data) { return; }
来源：http://hz.hongshengwenyu.top/gtrhbnbhap.html

JS:   if (!data) return;
来源：http://hz.birdmap.top/gtwcdmctnn.html

TS:   if (!data) return;
来源：http://hz.cqqwz.cn/gtjcrqvovd.html

Java: if (data == null) return;
来源：http://hz.zhijiandao.cn/gtcgsgvbuc.html

Go:   if data == nil { return }
来源：http://hz.52xcode.cn/gtuyqxsddf.html

Ruby: return if data.nil?
来源：http://hz.ppjwa.cn/gtaptpwgov.html

C#:   if (data == null) return;
来源：http://hz.andypj.xyz/gtljnmhnll.html

================================================================================
来源：http://hz.redwolf501.top/gtewmllqsx.html

C. 函数与作用域
来源：http://hz.zdqjudy.top/gtqvglobhw.html

================================================================================
来源：http://hz.nanxinkj.top/gtphwapcrc.html

[C01] 定义函数
来源：http://hz.zhongyouzk.top/gthlpzaotp.html

Py:   def add(a, b): return a + b
来源：http://hz.redwolf501.top/gtlfclqulz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtgjzwwdzj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.guowangkeji.top/gtuqusuxtl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgufenzy.top/gtnogtmcoj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtnoqxnwny.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hnxiangtu.top/gtkugvdlts.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cqqwz.cn/gtlsfewmdr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtwribtvze.html

[C02] 默认参数
来源：http://hz.yangfankeji.com/gteazyxfmb.html

Py:   def greet(name="World"): return name
来源：http://hz.aizwys.cn/gtakpdrlet.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jyoumei.cn/gtqokfuqmd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.meibo888.top/gtmfzfxtip.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gaohongyu789.top/gttndwowsb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.gotoacloud.top/gtgoviwaxi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jinghuilouyu.cn/gticurgdeh.html

Ruby: def greet(name = "World") = name
来源：http://hz.birdmap.top/gtwsmuilqm.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.52xcode.cn/gtvhszvugj.html

[C03] 可变参数
来源：http://hz.jqgufenzy.top/gtenrngotj.html

Py:   def total(*args): return sum(args)
来源：http://hz.0kj1m.cn/gtvmyqnzwj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shangyingyoupin.top/gtmbtlkhkg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gtjmofzvcb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yonumen.top/gtuaapiown.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.fzhhl.top/gtflluvbph.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yanxiufei.cn/gtlxjoinaa.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258888.top/gtkayyhkdq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yuxming.cn/gthevbiqnv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.tanke756.top/gtyjcdaphn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cdnleiting.top/gtzibvogcy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jiagoushi.top/gtqjokqdon.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhixingplan.top/gturosfebm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhongyouzk.top/gtrosyepvz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cdnleiting.top/gtzpijmckw.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinqigufen.top/gttzoeqefh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtusyzviwd.html

C#:   f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gtxvwvxjth.html

[C05] 返回多个值
来源：http://hz.yuanzhike.top/gttlzuivkb.html

Py:   return a, b
来源：http://hz.cheryme.top/gtouepltxs.html

PHP:  return [$a, $b];
来源：http://hz.shangyingyoupin.top/gttepcdhmg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cashguo.top/gtkxpwecuw.html

TS:   return { a, b };
来源：http://hz.jyoumei.cn/gtawvmques.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yvedp.cn/gtsnrsqokb.html

Go:   return a, b
来源：http://hz.yueranfly.top/gtogypzzaz.html

Ruby: return a, b
来源：http://hz.tanke756.top/gtepshafld.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yonumen.top/gtvsiuazsn.html

[C06] 匿名函数 / lambda
来源：http://hz.ehwqpu.com/gtzvicijjr.html

Py:   square = lambda x: x * x
来源：http://hz.yj20258.top/gtstrtwxzq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.316326.xyz/gtjlrfidfz.html

JS:   const square = x => x * x;
来源：http://hz.zycfv.cn/gtjtwrnowr.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hysaishi.cn/gtuxjgozyx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ydzc1.top/gtolsmpiya.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.redwolf501.top/gtzkkurodx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.snrcjt.cn/gtfxitrggl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.bjfxy.top/gtuqawvuuu.html

[C07] 把函数作为参数传入
来源：http://hz.ivvv.top/gtstpxrtkk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jqgfzy.top/gtnzbhbptv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xuanzx.com/gtazbgxnix.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yongpay.top/gtseqrpdqp.html

TS:   arr.map(String)
来源：http://hz.zhijiandao.cn/gtsfqqwqdq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.fzhhl.top/gtkcjadaka.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gzhubu.top/gtxetomhca.html

Ruby: arr.map(&:upcase)
来源：http://hz.pengpengdd.cyou/gtzjuooqcv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xingfuxueyuan.xyz/gthxibmzlq.html

[C08] 闭包
来源：http://hz.yueranfly.top/gtllgchrun.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yuxming.cn/gtzxxtjvfb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yangfankeji.com/gtcejjwrfw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtfczrxeqj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gtbvpgyvcd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.svipenyu.cn/gtbdkndrbc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hongshengwenyu.top/gtrlmusrlt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.redwolf501.top/gtttjotndg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.wangshuangyany.cn/gtbcphuxsh.html

[C09] 递归
来源：http://hz.sufxvd.cn/gtyiiscomj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtulspxotc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hammf.cn/gtnwqgdyki.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxinkj.top/gtbvqrqniq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258.top/gtphojppqa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yueranfly.top/gtjmnizaau.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.quarkkingdee.top/gtiwssxpow.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtycdbclps.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.guannengcc.top/gtrddrsfjc.html

[C10] 变量作用域
来源：http://hz.tanke756.top/gtdlruqsgq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.smart0.xyz/gtqkxxovke.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.redwolf501.top/gtxtvbhjyr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinqigufen.top/gtopoghrlj.html

TS:   同 JS
来源：http://hz.yj202588.top/gtbkybnrku.html

Java: 方法内为块级作用域
来源：http://hz.smart0.xyz/gttsdwnzph.html

Go:   花括号块级作用域
来源：http://hz.jinqigfzy.top/gtpwuywejn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yueranfly.top/gtzxvpdrqi.html

C#:   块级作用域
来源：http://hz.birdmap.top/gtthwsfkrr.html

[C11] 模块导入与导出
来源：http://hz.0kj1m.cn/gthtvjxzkr.html

Py:   from module import func
来源：http://hz.xuanzx.com/gthphlqvas.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yuxming.cn/gtoscjpjrm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gogol.net.cn/gttilvdrmm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sufxvd.cn/gtgjosprwt.html

Java: import java.util.List;
来源：http://hz.yj202588.top/gtyvajaeio.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jiagoushi.top/gtxskzveox.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.quarkkingdee.top/gtsvfwachv.html

C#:   using System.Text;
来源：http://hz.aibaodan.cn/gtbesmkeyk.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj202588.top/gtalkcbmjs.html

Py:   (lambda: print("run"))()
来源：http://hz.jiagoushi.top/gtbbflrmeg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ywan-chungtsiang.top/gtisansqai.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shuidangran.top/gtytujlsvm.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtmwafilmj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.meibo888.top/gttmrssxbb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yvedp.cn/gtyvasejng.html

Ruby: -> { puts "run" }.call
来源：http://hz.shanyushiyangtech.top/gtqcjgxsgp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.redwolf501.top/gtxuxvtaex.html

[C13] 类型声明 / 类型注解
来源：http://hz.smart0.xyz/gtflncjnvt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sweek.top/gthtgaaieh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtktvvxqqn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nwbrower.top/gttzmwhlwv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydzc1.top/gtypjewagc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gtqzhskfjw.html

Go:   func add(a, b int) int
来源：http://hz.snrcjt.cn/gtqqxncojm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xziqi.cn/gtcdfjiwcb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gogol.net.cn/gtwxwjjrlk.html

[C14] 泛型函数
来源：http://hz.xziqi.cn/gtpqprdokl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hongshengwenyu.top/gttocyqsnp.html

PHP:  // 无泛型
来源：http://hz.shangyingyoupin.top/gtjkbajyir.html

JS:   // 无泛型
来源：http://hz.jlsjyb.cn/gturertwql.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.chenzaomai.com/gtdkscmbvy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xziqi.cn/gtuqlbldfj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xuanzx.com/gtrevzfgbr.html

Ruby: # 无泛型
来源：http://hz.pycfn.com/gtwicuqztz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tian-w.cn/gtuoybxhbo.html

[C15] 解构 / 展开参数
来源：http://hz.gogol.net.cn/gtdllpvihd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.chenlongwang.top/gtktakhbed.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yonumen.top/gtjeefigyd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.iojbl.cn/gtvzmfwmql.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ydjk.org.cn/gtwlhofiqw.html

Java: // 无解构
来源：http://hz.chenzaomai.com/gtjukeaqkq.html

Go:   // 无解构
来源：http://hz.andypj.xyz/gtughaqhne.html

Ruby: a, b = pair
来源：http://hz.cqqwz.cn/gtuoakhghy.html

C#:   var (a, b) = pair;
来源：http://hz.andypj.xyz/gtvfzjuffy.html

[C16] 函数 / 方法重载
来源：http://hz.chenjidiqi.icu/gtdxocgiku.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.meibo888.top/gtlfzrwptg.html

PHP:  // 无重载
来源：http://hz.guannengcc.top/gtjnnbzqql.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.fengsongda.top/gtyfxpjbjm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hnqzz.top/gtgkyozgrw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tian-w.cn/gtethmxwvk.html

Go:   // 无重载：用不同函数名
来源：http://hz.shuidangran.top/gtalreecpq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shanyushiyangtech.top/gtskhxjjaa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sweek.top/gtmtbvvvmi.html

================================================================================
来源：http://hz.316326.xyz/gtrvezvvwd.html

D. 数组 / 列表 / 集合
来源：http://hz.nanxuanxn.top/gtvfaozwis.html

================================================================================
来源：http://hz.xinyue.icu/gtaawpnvwl.html

[D01] 创建数组 / 列表
来源：http://hz.hnxiangtu.top/gtvyoubzwm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xingfuxueyuan.xyz/gtnlhrayjp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.svipenyu.cn/gtebmbwjmu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zdqjudy.top/gtnwthafgd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.52xcode.cn/gtseevhcmh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xylfe.cn/gtgsjsavqr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zdqjudy.top/gtahqxxsvg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.chenzaomai.com/gtespamifo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xingfuxueyuan.xyz/gtgfchlyjn.html

[D02] 追加元素到末尾
来源：http://hz.gogol.net.cn/gttsycaqln.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhengqikj.top/gttwvuyvrz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuanzx.com/gtkaveqbdc.html

JS:   arr.push(4);
来源：http://hz.shuidangran.top/gtkhjkupgy.html

TS:   arr.push(4);
来源：http://hz.aizwys.cn/gtxsdfqmhz.html

Java: list.add(4);
来源：http://hz.52xcode.cn/gtdoeqjqcq.html

Go:   arr = append(arr, 4)
来源：http://hz.fzhhl.top/gtcfeoixmg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hongshengwenyu.top/gtnsozbadc.html

C#:   list.Add(4);
来源：http://hz.xinyue.icu/gtrnhejkxv.html

[D03] 在指定位置插入元素
来源：http://hz.sufxvd.cn/gthkoeerlj.html

Py:   arr.insert(0, 0)
来源：http://hz.guowangkeji.top/gtoqunfpdu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hysaishi.cn/gtjtoyjtzv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gogol.net.cn/gtrkbjatmu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yongpay.top/gtwjpbputl.html

Java: list.add(0, 0);
来源：http://hz.yueranfly.top/gtktcbjnws.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.feifeiyinyue.top/gtaqfsbjvv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shanyushiyangkeji.top/gtdunwfpkq.html

C#:   list.Insert(0, 0);
来源：http://hz.xziqi.cn/gtnujaqxnq.html

[D04] 删除元素
来源：http://hz.ivvv.top/gtnkyhludc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.meibo888.top/gtktezrpuy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenzaomai.com/gtprvtvbdp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xuetiantiany.cn/gtywtuqpdd.html

TS:   arr.splice(0, 1);
来源：http://hz.sweek.top/gthidfejrl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xingfuxueyuan.xyz/gtorhqrqbg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.0kj1m.cn/gtjpibhnbm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangtech.top/gtdeuvbkci.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ydjk.org.cn/gtywjobiis.html

[D05] 访问与修改元素
来源：http://hz.cashguo.top/gtsjlsyacc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gthbatbrse.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258.top/gtsvefwalj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zdqjudy.top/gtefrcmkmp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sweek.top/gtsfweabfm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yvedp.cn/gtmbazwufq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jyoumei.cn/gticvewlui.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtslzqdyax.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.dianchejie.cn/gtzkgoqgyg.html

[D06] 数组长度
来源：http://hz.aizwys.cn/gtuhjvsyog.html


<!-- 参考信息 -->