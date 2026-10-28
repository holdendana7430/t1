代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj20258.top/gteghfsjvx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.sweek.top/gtulxelatk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cashguo.top/gtkjijrocw.html

Ruby: arr.each { |item| puts item }
来源：http://hz.sxryk.cn/gtlprwkrgu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.tianlin.xyz/gtvyvgrxti.html

[B06] 遍历字典 / 对象
来源：http://hz.nwbrower.top/gtehyffpaw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.quarkkingdee.top/gtqdfpynqf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.sysykeji.top/gthqlvrvhc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gaohongyu789.top/gtnjhllwuq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xziqi.cn/gtfrdrfrio.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.smart0.xyz/gtqrgsncim.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shangyingyoupin.top/gtlfvkctpl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.0kj1m.cn/gtxfbmdzgs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.xuetiantiany.cn/gtnqpwores.html

[B07] while 循环
来源：http://hz.xziqi.cn/gtdatxcuej.html

Py:   while i < 10: i += 1
来源：http://hz.cqqwz.cn/gtnzkkteaa.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.cashguo.top/gteemlmovp.html

JS:   while (i < 10) { i++; }
来源：http://hz.yj20258.top/gtvpncxdaf.html

TS:   while (i < 10) { i++; }
来源：http://hz.fengsongda.top/gtziyunpsr.html

Java: while (i < 10) { i++; }
来源：http://hz.yj20258888.top/gtewaunpwf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.havefunace.top/gtslqjkgbz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.cqqwz.cn/gtlwweozmh.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinqigufen.top/gtfcahgkxz.html

[B08] do-while（至少执行一次）
来源：http://hz.xinyue.icu/gttxjohkpr.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.sufxvd.cn/gtmafxxstj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ydjk.org.cn/gteywrxywo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gtmyajuuzm.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ydjk.org.cn/gtbhegrtpr.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhaomingkeji.xyz/gtmjkoropu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.redwolf501.top/gtqkcuopgr.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.bjfxy.top/gtzfvwdtes.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gtovscunen.html

[B09] break 与 continue
来源：http://hz.yanxiufei.cn/gtxmijzoar.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.52xcode.cn/gtrqhdogoo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhongyouzk.top/gtafgzkese.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhixingplan.top/gtmbxassqp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pengpengdd.cyou/gtidkonzgd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtzawoeqex.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yangfankeji.com/gtihlnpgdh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.chenzaomai.com/gtmgwvpbfe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jyoumei.cn/gtynfgiyoz.html

[B10] 遍历同时拿索引
来源：http://hz.hnxiangtu.top/gtewtjkdgz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.wangdashe.top/gtyxfmxegl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yj20258888.top/gtwhefqlcp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.chenzaomai.com/gtuqiuqmon.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jinghuilouyu.cn/gtxasojrcj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hammf.cn/gtvpywmdeh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hnqzz.top/gtebaouwsz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.meibo888.top/gtxvmosgax.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.wangshuangyany.cn/gttvnxhobz.html

[B11] 生成数字序列 / 区间
来源：http://hz.52xcode.cn/gthugieyzi.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenjidiqi.icu/gtxmcchcvr.html

PHP:  range(0, 10, 2);
来源：http://hz.jiagoushi.top/gtzcpufygq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xingfuxueyuan.xyz/gttcneqtez.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xuetiantiany.cn/gteydljcmv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhixingplan.top/gtlxcgeeqf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.quarkkingdee.top/gtoyfxvdfq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.havefunace.top/gtojnmetms.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.kuanghao11.cn/gtpijtbtkw.html

[B12] 跳出多层循环
来源：http://hz.shzxlz.cn/gtiqtgtkjc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.pengpengdd.cyou/gtovhvvwnp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zdqjudy.top/gtdxerxbwe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxinkj.top/gtklllwxhy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shzxlz.cn/gtiqeiqzzx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.smart0.xyz/gtidaxbsqb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hongshengwenyu.top/gtqxqlgcbf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhengqikj.top/gtxfmcmdcp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yuanzhike.top/gtfclaunpy.html

[B13] 判断是否为数字
来源：http://hz.guannengcc.top/gtkvhzffaq.html

Py:   isinstance(x, (int, float))
来源：http://hz.nwbrower.top/gtnefxqrpr.html

PHP:  is_numeric($x)
来源：http://hz.fengsongda.top/gtthauttsj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hywenlv.cn/gtyvxprupn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yvedp.cn/gtvjigyiir.html

Java: x instanceof Number
来源：http://hz.redwolf501.top/gtjwzgoqty.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.316326.xyz/gtikvhpezu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yueranfly.top/gttmradbgj.html

C#:   x is int or double or decimal
来源：http://hz.wangshuangyany.cn/gtbjkozqsr.html

[B14] 判断值是否在集合内
来源：http://hz.aibaodan.cn/gtdbbenasp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.fengsongda.top/gtrcccowkz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.9152youxi.cn/gtwsqwdqyt.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.guowangkeji.top/gtkvgrljgp.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zycfv.cn/gtyolsamdu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ppjwa.cn/gthrpuystu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ehwqpu.com/gtszsxnbmz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hywenlv.cn/gttolcmzpb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sweek.top/gtnijhqbdw.html

[B15] 布尔运算与取反
来源：http://hz.nwbrower.top/gtcxdlphut.html

Py:   a and b or not c
来源：http://hz.yonumen.top/gtipskropo.html

PHP:  $a && $b || !$c
来源：http://hz.pycfn.com/gtbbnllnmq.html

JS:   a && b || !c
来源：http://hz.sxryk.cn/gtvwhqnagk.html

TS:   a && b || !c
来源：http://hz.dashuyun.cn/gtbhijhrnv.html

Java: a && b || !c
来源：http://hz.yj20258.top/gtrsnnmvru.html

Go:   a && b || !c
来源：http://hz.yvedp.cn/gtfnpodnhi.html

Ruby: a && b || !c
来源：http://hz.hfpthk.cn/gtffxhchbw.html

C#:   a && b || !c
来源：http://hz.yvedp.cn/gtsucrdxmc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tanke756.top/gtaaeywwdy.html

Py:   if not data: return
来源：http://hz.cheryme.top/gtqgxrzhxj.html

PHP:  if (!$data) { return; }
来源：http://hz.hysaishi.cn/gtuamlghbp.html

JS:   if (!data) return;
来源：http://hz.sweek.top/gtzevzlube.html

TS:   if (!data) return;
来源：http://hz.jinyuanbaomall.cn/gtparuztwo.html

Java: if (data == null) return;
来源：http://hz.redwolf501.top/gtrypqehqn.html

Go:   if data == nil { return }
来源：http://hz.feifeiyinyue.top/gtsopgbwfb.html

Ruby: return if data.nil?
来源：http://hz.jinqigufen.top/gtmviglifi.html

C#:   if (data == null) return;
来源：http://hz.yuanzhike.top/gtpqjdjhti.html

================================================================================
来源：http://hz.mhx1999.top/gthczhokcw.html

C. 函数与作用域
来源：http://hz.sysykeji.top/gtiztritct.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtycvouxyl.html

[C01] 定义函数
来源：http://hz.cheryme.top/gtdrerbfea.html

Py:   def add(a, b): return a + b
来源：http://hz.hongshengwenyu.top/gtjcustyhv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sweek.top/gtsdwycopn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenlongwang.top/gtkdxndzmj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.316326.xyz/gttyuqzmnh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tianlin.xyz/gtrxhyezju.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shanyushiyangtech.top/gtaikjbopd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenzaomai.com/gtikgpnkew.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtifuplmmx.html

[C02] 默认参数
来源：http://hz.yj20258.top/gtazuwudll.html

Py:   def greet(name="World"): return name
来源：http://hz.kuanghao11.cn/gtdalvknbe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yuanzhike.top/gtkuvncyfq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jianghu66.top/gtjmjbyjxo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.shanyushiyangkeji.top/gtkmdwqylh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.52xcode.cn/gtqatycjou.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj202588.top/gtadbmakwn.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhaomingkeji.xyz/gtcvbehglx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jqgufenzy.top/gtbagnudjg.html

[C03] 可变参数
来源：http://hz.gaohongyu789.top/gttjcekxso.html

Py:   def total(*args): return sum(args)
来源：http://hz.jiagoushi.top/gtopphgnsv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shanyushiyangkeji.top/gtelmqedrb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenlongwang.top/gthvejsaca.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhongyouzk.top/gtvmqojtap.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhengqikj.top/gtpsorfprp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jqgfzy.top/gtsunadewg.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shanyushiyangkeji.top/gthdtojnln.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.aibaodan.cn/gtjpdaqxuw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cucudq.cn/gtpcakhues.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shangyingyoupin.top/gtfzmkwaqi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.andypj.xyz/gtbznxrubb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinyuanbaomall.cn/gtmumvigtr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.tian-w.cn/gtuuwbcqcu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.smart0.xyz/gtiacvetuy.html

Go:   // 无：用配置结构体参数
来源：http://hz.nanxinkj.top/gtaasmxznb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gttuoqqaqr.html

C#:   f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtielklats.html

[C05] 返回多个值
来源：http://hz.yangfankeji.com/gtobvgfwgz.html

Py:   return a, b
来源：http://hz.yangfankeji.com/gtwdpmmxqm.html

PHP:  return [$a, $b];
来源：http://hz.yj202588.top/gtiqrbqbld.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yongpay.top/gtwrsnfhsv.html

TS:   return { a, b };
来源：http://hz.jianghu66.top/gtluxofxtl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hnqzz.top/gtlchyvfpe.html

Go:   return a, b
来源：http://hz.jlsjyb.cn/gtqahvpprj.html

Ruby: return a, b
来源：http://hz.gaohongyu789.top/gtanezlbxi.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jyoumei.cn/gtokefnfwr.html

[C06] 匿名函数 / lambda
来源：http://hz.tanke756.top/gtqblwspub.html

Py:   square = lambda x: x * x
来源：http://hz.dashuyun.cn/gthkftecge.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.iojbl.cn/gtzwpdrnfo.html

JS:   const square = x => x * x;
来源：http://hz.shanyushiyangkeji.top/gtyfvjmldi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.316326.xyz/gthrxownsh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yvedp.cn/gtzsislbzs.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.sysykeji.top/gtkvcbueza.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yuxming.cn/gteolcesqy.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinyuanbaomall.cn/gtbtamdikd.html

[C07] 把函数作为参数传入
来源：http://hz.gotoacloud.top/gtjjdfcnww.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.52xcode.cn/gtysussoiz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zycfv.cn/gtwmanfqpn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dashuyun.cn/gterelkwjd.html

TS:   arr.map(String)
来源：http://hz.snrcjt.cn/gtndwcejex.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nanxuanxn.top/gtikuofoce.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xinyue.icu/gthvlmxhsp.html

Ruby: arr.map(&:upcase)
来源：http://hz.ywan-chungtsiang.top/gtiijmxxgz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jyoumei.cn/gtneuaxfdd.html

[C08] 闭包
来源：http://hz.bjfxy.top/gticgrmnnx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.guowangkeji.top/gtohysjwkk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.havefunace.top/gtkfxzdtts.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jiagoushi.top/gtmhxrwlyh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.smart0.xyz/gtxezuxreb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sufxvd.cn/gtnsweslyr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.wangdashe.top/gtoexroxgd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yuanzhike.top/gtnhzehxia.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtcnpysuyb.html

[C09] 递归
来源：http://hz.nwbrower.top/gtzfijivba.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ybcxt.top/gtcvmomvie.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.c1oappe.top/gtywuhmsjr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cheryme.top/gtvqbmdudw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnxiangtu.top/gtmjbjkewm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.wangdashe.top/gtdanfbwkz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenlongwang.top/gtlfjfqdfr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.birdmap.top/gtovguzfvu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.pycfn.com/gtzrlxdgpe.html

[C10] 变量作用域
来源：http://hz.yj20258.top/gtneudzhmq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.bjfxy.top/gtdoalkyer.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shanyushiyangtech.top/gteklrmhva.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydjk.org.cn/gtylfhpeju.html

TS:   同 JS
来源：http://hz.ydjk.org.cn/gtzvvuguwd.html

Java: 方法内为块级作用域
来源：http://hz.jianghu66.top/gtfufwdlyo.html

Go:   花括号块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtgvrlqzyh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.kuanghao11.cn/gtoaihlmau.html

C#:   块级作用域
来源：http://hz.yj20258.top/gtwsfkizgz.html

[C11] 模块导入与导出
来源：http://hz.zycfv.cn/gtzggseaij.html

Py:   from module import func
来源：http://hz.pycfn.com/gtmyerfnck.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.wangshuangyany.cn/gtzqulmhsw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yuanzhike.top/gtbqkogzwe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.vqdsnc.cn/gtvxausxsm.html

Java: import java.util.List;
来源：http://hz.zhijiandao.cn/gtstecqxfc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.andypj.xyz/gtheyyvrvl.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daxiang520.top/gtmzgkvfvp.html

C#:   using System.Text;
来源：http://hz.xylfe.cn/gtsznuuznr.html

[C12] 立即执行函数 IIFE
来源：http://hz.hnxiangtu.top/gtgnklnhic.html

Py:   (lambda: print("run"))()
来源：http://hz.yj20258888.top/gtheussrlv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jiagoushi.top/gttybpfxsa.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ybcxt.top/gtqdtnvpki.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xuetiantiany.cn/gtxcyygopl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ydzc1.top/gtvcbookvi.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhoulong.xyz/gtxulvmfes.html

Ruby: -> { puts "run" }.call
来源：http://hz.yangfankeji.com/gtfjhahhxt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.fengsongda.top/gtmhbmgjow.html

[C13] 类型声明 / 类型注解
来源：http://hz.shanyushiyangtech.top/gtrdpuddsl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shzxlz.cn/gtgtjtawkr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtmbtulpih.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.vqdsnc.cn/gtijqhdgut.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhijiandao.cn/gtzohyvxik.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shuidangran.top/gtjbskjdmg.html

Go:   func add(a, b int) int
来源：http://hz.svipenyu.cn/gtojykvltc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuanzhike.top/gtnjsuxtco.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhiwuduotai.top/gttniypzhe.html

[C14] 泛型函数
来源：http://hz.nanxuanxn.top/gtjqvhduev.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ywan-chungtsiang.top/gtgslqubkl.html

PHP:  // 无泛型
来源：http://hz.0kj1m.cn/gtafvwtwzc.html

JS:   // 无泛型
来源：http://hz.yongpay.top/gtklbdkmnn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xuanzx.com/gtvgbmjppk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.quarkkingdee.top/gttbcfmlba.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hnqzz.top/gtjjhaszef.html

Ruby: # 无泛型
来源：http://hz.andypj.xyz/gtirfgscet.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhongyouzk.top/gtozaiogis.html

[C15] 解构 / 展开参数
来源：http://hz.iojbl.cn/gtjjvbcvsp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hywenlv.cn/gtllghghjp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhoulong.xyz/gtwhjfttdr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nwbrower.top/gtbeshiefx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gotoacloud.top/gtwpghreyl.html

Java: // 无解构
来源：http://hz.shzxlz.cn/gtjxltufzz.html

Go:   // 无解构
来源：http://hz.xylfe.cn/gtbuqqghru.html

Ruby: a, b = pair
来源：http://hz.fzhhl.top/gtbievludg.html

C#:   var (a, b) = pair;
来源：http://hz.gzhubu.top/gtylfbvgvg.html

[C16] 函数 / 方法重载
来源：http://hz.yueranfly.top/gtlbvzzqnh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.dianchejie.cn/gtugqnwpri.html

PHP:  // 无重载
来源：http://hz.guowangkeji.top/gtivltfnth.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhoulong.xyz/gtpjusneak.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinghuilouyu.cn/gtsonewfst.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pycfn.com/gtttexxnws.html

Go:   // 无重载：用不同函数名
来源：http://hz.hywenlv.cn/gtdzaqkbnz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yj202588.top/gtrybscrfc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.52xcode.cn/gttwxdiciq.html

================================================================================
来源：http://hz.zycfv.cn/gtvvxsjirh.html

D. 数组 / 列表 / 集合
来源：http://hz.xuanzx.com/gtwhgbpxdv.html

================================================================================
来源：http://hz.wangdashe.top/gtqpizxjmh.html

[D01] 创建数组 / 列表
来源：http://hz.yonumen.top/gtkbmofgna.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.nwbrower.top/gtfvsutegw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.dashuyun.cn/gtmwaxklye.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yangfankeji.com/gttzytcgri.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.chenlongwang.top/gthuluwmll.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aizwys.cn/gtorermfzs.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenzaomai.com/gtdjhimkck.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cdnleiting.top/gtfkguhhgw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yonumen.top/gtaudapeed.html

[D02] 追加元素到末尾
来源：http://hz.tianlin.xyz/gtxzindmim.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xingfuxueyuan.xyz/gtckkxkznh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhoulong.xyz/gtvpuezvif.html

JS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtgjqkxxai.html

TS:   arr.push(4);
来源：http://hz.ivvv.top/gtydmwnnme.html

Java: list.add(4);
来源：http://hz.jinqigufen.top/gtdempdhju.html

Go:   arr = append(arr, 4)
来源：http://hz.gaohongyu789.top/gtrxeviaeg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinghuilouyu.cn/gtissebwkj.html

C#:   list.Add(4);
来源：http://hz.ywan-chungtsiang.top/gtxvvxqgpt.html

[D03] 在指定位置插入元素
来源：http://hz.jinghuilouyu.cn/gtnbtoltpi.html

Py:   arr.insert(0, 0)
来源：http://hz.ybcxt.top/gtwrjxrtiu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ybcxt.top/gtdmfmabcp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.dianchejie.cn/gtgjrkempo.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sufxvd.cn/gtoxudptpn.html

Java: list.add(0, 0);
来源：http://hz.sufxvd.cn/gthvfoawkl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yonumen.top/gtibmgmbtq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.snrcjt.cn/gtjztbamqt.html

C#:   list.Insert(0, 0);
来源：http://hz.jinqigfzy.top/gtpyfckjee.html

[D04] 删除元素
来源：http://hz.zhaomingkeji.xyz/gthnaurbjb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhixingplan.top/gtqnycliuv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenlongwang.top/gtzeoxtywk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.quarkkingdee.top/gtsdoiejnb.html

TS:   arr.splice(0, 1);
来源：http://hz.zhixingplan.top/gtzmgtdlez.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.bjfxy.top/gtqgilmruu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yueranfly.top/gtbymkuaqg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenjidiqi.icu/gtgwgnwvbp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnqzz.top/gtdnqejufy.html

[D05] 访问与修改元素
来源：http://hz.ybcxt.top/gtvytwmszi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pengpengdd.cyou/gtwjfxygbk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nanxuanxn.top/gtwhqupeni.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtxyyfrzts.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.iojbl.cn/gthxhtstrd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aibaodan.cn/gtmtypjuli.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sysykeji.top/gtztxgsvop.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtkktlmpua.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sweek.top/gtpmulntjh.html

[D06] 数组长度
来源：http://hz.zhixingplan.top/gtrhigbcmx.html


<!-- 参考信息 -->