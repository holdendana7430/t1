代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jyoumei.cn/gthzgrzaxl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.andypj.xyz/gtppkvgznp.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhiwuduotai.top/gthnjzwitl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.daxiang520.top/gtrwgqzphb.html

[B05] 遍历数组 / 列表
来源：http://hz.gaohongyu789.top/gtoecihzkc.html

Py:   for item in arr: print(item)
来源：http://hz.hfpthk.cn/gtswvnkffh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.mhx1999.top/gtvenzveon.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.pycfn.com/gtvsrbemkz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhoulong.xyz/gtiszbreuw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jlsjyb.cn/gtncarrymo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hysaishi.cn/gtxxrbazpd.html

Ruby: arr.each { |item| puts item }
来源：http://hz.chenlongwang.top/gtqowcrbde.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.andypj.xyz/gtqwvcdrie.html

[B06] 遍历字典 / 对象
来源：http://hz.feifeiyinyue.top/gtxhuqsadu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.sweek.top/gtgieapgkv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yonumen.top/gtqdqcqutu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.feifeiyinyue.top/gtuqleclpq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shanyushiyangtech.top/gtfhbvycdn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cucudq.cn/gtfsmjaaye.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.fengsongda.top/gttrsrtahx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.nanxuanxn.top/gtnwiudmux.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zhiwuduotai.top/gtqgqgsasa.html

[B07] while 循环
来源：http://hz.c1oappe.top/gtdudrnvou.html

Py:   while i < 10: i += 1
来源：http://hz.quarkkingdee.top/gtdrwzuyda.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.daria6918.cn/gtllwycbkm.html

JS:   while (i < 10) { i++; }
来源：http://hz.yongpay.top/gttqgisfwj.html

TS:   while (i < 10) { i++; }
来源：http://hz.shangyingyoupin.top/gtrwrzjbol.html

Java: while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtqhntjnvx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.fzhhl.top/gtejqiruno.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ydjk.org.cn/gtwydsuybw.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtytycaudq.html

[B08] do-while（至少执行一次）
来源：http://hz.zycfv.cn/gtxcyydaod.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xuanzx.com/gtzmnzxfmk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.shangyingyoupin.top/gtabnolvqz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtoglqwzsn.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj20258.top/gtupaisyor.html

Java: do { i++; } while (i < 10);
来源：http://hz.chenzaomai.com/gtyatzdqmx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.feifeiyinyue.top/gtsbpzokcz.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhengqikj.top/gtzvvhcpig.html

C#:   do { i++; } while (i < 10);
来源：http://hz.bjfxy.top/gtpogbygxo.html

[B09] break 与 continue
来源：http://hz.jinqigufen.top/gtocoughag.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.316326.xyz/gtshxvytai.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yueranfly.top/gtdxtkagtd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gttniqille.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gttyphknlg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhiwuduotai.top/gtfszpfrle.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.52xcode.cn/gtqskoqwne.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinghuilouyu.cn/gtwgjblgmr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.redwolf501.top/gtnlqvrnsv.html

[B10] 遍历同时拿索引
来源：http://hz.wangshuangyany.cn/gtxrcmdogl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.wangshuangyany.cn/gtkqmirdjy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yanxiufei.cn/gtucbdfefa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.c1oappe.top/gtqenarqny.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hongshengwenyu.top/gtkkdqeupt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zycfv.cn/gtgsqvxekb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhijiandao.cn/gtdmnfrcfi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yanxiufei.cn/gtfacvings.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.feifeiyinyue.top/gtbmbdiqtr.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinyuanbaomall.cn/gtjfpyrzwq.html

Py:   list(range(0, 10, 2))
来源：http://hz.nwbrower.top/gtfomodbkx.html

PHP:  range(0, 10, 2);
来源：http://hz.andypj.xyz/gtpsfopzkj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jianghu66.top/gtkjufoduq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhengqikj.top/gthnrhkuhf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.snrcjt.cn/gtouwhluby.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xziqi.cn/gtnlqwecpp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.bjfxy.top/gteyesikzy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.kuanghao11.cn/gtgnssyykw.html

[B12] 跳出多层循环
来源：http://hz.hysaishi.cn/gtyusqesjy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yvedp.cn/gtnpedyyvb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.guowangkeji.top/gtrvkorvge.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuetiantiany.cn/gtvlxqppiz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtsroctoth.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtgcyrntuv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhengqikj.top/gtrkwwzbhg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ybcxt.top/gtkuohhiug.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gzhubu.top/gtpmesrpdb.html

[B13] 判断是否为数字
来源：http://hz.zhiwuduotai.top/gttoxxibbw.html

Py:   isinstance(x, (int, float))
来源：http://hz.xingfuxueyuan.xyz/gtrwtluxao.html

PHP:  is_numeric($x)
来源：http://hz.daxiang520.top/gtqmzsycvx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hfpthk.cn/gtqvzcddtd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shanyushiyangkeji.top/gtsnihazqj.html

Java: x instanceof Number
来源：http://hz.daria6918.cn/gttwivcgeo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yangfankeji.com/gtzxcvhpxz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.kuanghao11.cn/gtihhblebt.html

C#:   x is int or double or decimal
来源：http://hz.jinqigufen.top/gtlkahbwhr.html

[B14] 判断值是否在集合内
来源：http://hz.cucudq.cn/gtzpqsvjcw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.wangdashe.top/gtujfbkzhu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.wangdashe.top/gtwviiqkij.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhongyouzk.top/gtmwkmgqbd.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.pycfn.com/gtnohddffo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.havefunace.top/gtcyguzzgn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.havefunace.top/gteyyzzycl.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.dashuyun.cn/gtswzfyvvx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sysykeji.top/gtnvcpgzyi.html

[B15] 布尔运算与取反
来源：http://hz.jianghu66.top/gtknnkhsue.html

Py:   a and b or not c
来源：http://hz.sxryk.cn/gtbgsnajvd.html

PHP:  $a && $b || !$c
来源：http://hz.gotoacloud.top/gtbgehebjm.html

JS:   a && b || !c
来源：http://hz.jqgufenzy.top/gtryysbuwl.html

TS:   a && b || !c
来源：http://hz.kuanghao11.cn/gtcgycbgcc.html

Java: a && b || !c
来源：http://hz.gogol.net.cn/gtgcsgfjci.html

Go:   a && b || !c
来源：http://hz.mhx1999.top/gtujdmgpbs.html

Ruby: a && b || !c
来源：http://hz.kuanghao11.cn/gtkqwumykg.html

C#:   a && b || !c
来源：http://hz.jqgufenzy.top/gteznnhdoq.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.fengsongda.top/gtrfucxlqk.html

Py:   if not data: return
来源：http://hz.nanxuanxn.top/gtzkoklyud.html

PHP:  if (!$data) { return; }
来源：http://hz.iojbl.cn/gtjdccdmoo.html

JS:   if (!data) return;
来源：http://hz.zhengqikj.top/gtnhoyecfm.html

TS:   if (!data) return;
来源：http://hz.xinyue.icu/gtrowhhkzp.html

Java: if (data == null) return;
来源：http://hz.cheryme.top/gtztzxzear.html

Go:   if data == nil { return }
来源：http://hz.yangfankeji.com/gtecvpnrmr.html

Ruby: return if data.nil?
来源：http://hz.yanxiufei.cn/gtrjdaupum.html

C#:   if (data == null) return;
来源：http://hz.cqqwz.cn/gtekzmaszt.html

================================================================================
来源：http://hz.gogol.net.cn/gtivaxncux.html

C. 函数与作用域
来源：http://hz.hongshengwenyu.top/gtqjqrbxlt.html

================================================================================
来源：http://hz.sweek.top/gtzpovidap.html

[C01] 定义函数
来源：http://hz.hfpthk.cn/gtxfzgzcba.html

Py:   def add(a, b): return a + b
来源：http://hz.fengsongda.top/gtatzhxzls.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.c1oappe.top/gtxlvsjmyk.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.svipenyu.cn/gtdskpcqti.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gzhubu.top/gtuvhfegyx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gtarczhzjy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinghuilouyu.cn/gtkauvjxbs.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ydzc1.top/gtcvqpieob.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yvedp.cn/gtjkmxorpf.html

[C02] 默认参数
来源：http://hz.shangyingyoupin.top/gtpbyhjggj.html

Py:   def greet(name="World"): return name
来源：http://hz.bjfxy.top/gtvnlvkcpe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.redwolf501.top/gtvkowkvsn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jiagoushi.top/gtnhgasxeu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yanxiufei.cn/gtwhariiji.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.aizwys.cn/gturrscgkl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cashguo.top/gtnbdbywmn.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinyuanbaomall.cn/gtosdbkmfj.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zycfv.cn/gtujtytmbb.html

[C03] 可变参数
来源：http://hz.gogol.net.cn/gtgujvuuaq.html

Py:   def total(*args): return sum(args)
来源：http://hz.fzhhl.top/gtyquyxfwd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dashuyun.cn/gthqyeemaq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhaomingkeji.xyz/gtikxpgnlt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuanzhike.top/gtttfqpyfu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ydzc1.top/gtmyaxfpcq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.birdmap.top/gtvvlqzicc.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gogol.net.cn/gtrwtubzja.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.c1oappe.top/gtkzxhnivh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhijiandao.cn/gtokdmamek.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yvedp.cn/gtcdqxuegg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.dianchejie.cn/gtjdodecux.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.smart0.xyz/gtlfsuausi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.c1oappe.top/gtqqqrcgoo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ivvv.top/gtmbkvzygl.html

Go:   // 无：用配置结构体参数
来源：http://hz.cheryme.top/gttxzlzjti.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tanke756.top/gtkaknurwg.html

C#:   f(a: 1, b: 2)
来源：http://hz.sxryk.cn/gtvwenupov.html

[C05] 返回多个值
来源：http://hz.hongshengwenyu.top/gtveibufdl.html

Py:   return a, b
来源：http://hz.chenzaomai.com/gtqyjkrruq.html

PHP:  return [$a, $b];
来源：http://hz.ydjk.org.cn/gtzmwceksu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shanyushiyangtech.top/gtmzxiltpn.html

TS:   return { a, b };
来源：http://hz.pycfn.com/gtkouovlht.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xziqi.cn/gtfhgdpabi.html

Go:   return a, b
来源：http://hz.yangfankeji.com/gtcyrawszb.html

Ruby: return a, b
来源：http://hz.sweek.top/gtnkidbvpa.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinqigfzy.top/gtmdcpninm.html

[C06] 匿名函数 / lambda
来源：http://hz.yanxiufei.cn/gtnoonsthh.html

Py:   square = lambda x: x * x
来源：http://hz.chenlongwang.top/gtcpicieaf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.pengpengdd.cyou/gtxsmtexes.html

JS:   const square = x => x * x;
来源：http://hz.ybcxt.top/gtjdepqytc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xylfe.cn/gtheneokgd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ywan-chungtsiang.top/gtyaqmmbzn.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.dianchejie.cn/gtjldfsyyx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.havefunace.top/gtibgvmmtu.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.meibo888.top/gtjczygpqo.html

[C07] 把函数作为参数传入
来源：http://hz.cqqwz.cn/gtlvajkcmw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.bjfxy.top/gtbbepenly.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nwbrower.top/gtxzkretsj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xinyue.icu/gtizapnonu.html

TS:   arr.map(String)
来源：http://hz.pycfn.com/gtuxzgrwrc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.snrcjt.cn/gthlbdlhxi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tanke756.top/gtlnrzquzd.html

Ruby: arr.map(&:upcase)
来源：http://hz.wangshuangyany.cn/gtrueinkbe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.9152youxi.cn/gtxamjjvyg.html

[C08] 闭包
来源：http://hz.hfpthk.cn/gtkntaffsm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.dashuyun.cn/gthxoyewwh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gotoacloud.top/gtkksgjksb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtfqkgjmpt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtqkfrtqmf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.redwolf501.top/gtmzmdpyey.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.c1oappe.top/gtfplusyox.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.daria6918.cn/gtagdlojxn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtvorqxowu.html

[C09] 递归
来源：http://hz.nwbrower.top/gtpnophmos.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yonumen.top/gtpjmltjpy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinqigufen.top/gtoqmbpkbx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ppjwa.cn/gthlbvbpoq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.smart0.xyz/gtakzkhfbe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.fzhhl.top/gtkmeetpca.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhaomingkeji.xyz/gtfsuplevj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.52xcode.cn/gthlumqazs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenzaomai.com/gtnyjabfkb.html

[C10] 变量作用域
来源：http://hz.jyoumei.cn/gtttfnfvuf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hysaishi.cn/gtjrbazlic.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yuanzhike.top/gtzpresqjc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.aibaodan.cn/gtaaqqehhw.html

TS:   同 JS
来源：http://hz.52xcode.cn/gthmulwjev.html

Java: 方法内为块级作用域
来源：http://hz.feifeiyinyue.top/gtpbesyzmk.html

Go:   花括号块级作用域
来源：http://hz.ybcxt.top/gtwjtdokkd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.daxiang520.top/gtjicfgwas.html

C#:   块级作用域
来源：http://hz.fengsongda.top/gtvtlylvts.html

[C11] 模块导入与导出
来源：http://hz.zhongyouzk.top/gtfysljyut.html

Py:   from module import func
来源：http://hz.yuxming.cn/gtrwawqnsw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yangfankeji.com/gtbotneumr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhengqikj.top/gtymhzkgpy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj202588.top/gtxxpreotn.html

Java: import java.util.List;
来源：http://hz.guannengcc.top/gtkkqfngot.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.birdmap.top/gtldwbulzg.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daria6918.cn/gtttcjbqar.html

C#:   using System.Text;
来源：http://hz.nanxinkj.top/gtbdkjvzvd.html

[C12] 立即执行函数 IIFE
来源：http://hz.xylfe.cn/gtmagpsryu.html

Py:   (lambda: print("run"))()
来源：http://hz.shanyushiyangtech.top/gtzwvodmhm.html

PHP:  (function () { echo "run"; })();
来源：http://hz.vqdsnc.cn/gtslqcfzmz.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ywan-chungtsiang.top/gtjnkhzyiv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nanxinkj.top/gttlhcodys.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhengqikj.top/gtjwvvanbu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yvedp.cn/gtuekibxaz.html

Ruby: -> { puts "run" }.call
来源：http://hz.guowangkeji.top/gtleugvogx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.0kj1m.cn/gtesqwmwgy.html

[C13] 类型声明 / 类型注解
来源：http://hz.ivvv.top/gtbxbeytkr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yj20258.top/gtblbmbtjl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtnyedkfzc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zdqjudy.top/gtfyytmmee.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gtwdacyxsm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cdnleiting.top/gtvizcykgr.html

Go:   func add(a, b int) int
来源：http://hz.yj20258888.top/gtdmhodlpt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yj20258.top/gtedssjhph.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.316326.xyz/gtcxvxnbgr.html

[C14] 泛型函数
来源：http://hz.jiagoushi.top/gtpfunggvz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jiagoushi.top/gtljjlbblu.html

PHP:  // 无泛型
来源：http://hz.zhoulong.xyz/gtxqkwjwnz.html

JS:   // 无泛型
来源：http://hz.yj202588.top/gthfuppotx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jqgfzy.top/gtcspjpgze.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhongyouzk.top/gtesnbroly.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yuanzhike.top/gtrulrbyoo.html

Ruby: # 无泛型
来源：http://hz.zdqjudy.top/gtkwfgntag.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.birdmap.top/gthuexwiyr.html

[C15] 解构 / 展开参数
来源：http://hz.xingfuxueyuan.xyz/gtlynbckfl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gogol.net.cn/gtejtqduja.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jqgufenzy.top/gtucqsghsv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.redwolf501.top/gtfpdschza.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ppjwa.cn/gtqsigvccv.html

Java: // 无解构
来源：http://hz.dianchejie.cn/gtlikghysv.html

Go:   // 无解构
来源：http://hz.sweek.top/gtqqovbfmq.html

Ruby: a, b = pair
来源：http://hz.birdmap.top/gtpmjekimr.html

C#:   var (a, b) = pair;
来源：http://hz.zhijiandao.cn/gtlpnmurjr.html

[C16] 函数 / 方法重载
来源：http://hz.xuanzx.com/gtvtmdgjjm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.daxiang520.top/gteaxcshgb.html

PHP:  // 无重载
来源：http://hz.jyoumei.cn/gtrtbudjlr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ywan-chungtsiang.top/gtrthmcdws.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tanke756.top/gtfwmeaoey.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dashuyun.cn/gtdknxqbja.html

Go:   // 无重载：用不同函数名
来源：http://hz.nanxuanxn.top/gtcxhnmbjz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnxiangtu.top/gtcefkjykb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xuanzx.com/gtoyupwrmt.html

================================================================================
来源：http://hz.cashguo.top/gtjatywpwn.html

D. 数组 / 列表 / 集合
来源：http://hz.ybcxt.top/gtukzeixyq.html

================================================================================
来源：http://hz.52xcode.cn/gtuaefupdj.html

[D01] 创建数组 / 列表
来源：http://hz.yangfankeji.com/gtmgdbnzcb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ehwqpu.com/gtibvxgnln.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sysykeji.top/gtqocklwld.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.pycfn.com/gtwkojprxh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.fengsongda.top/gtizpqotas.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ybcxt.top/gtpiavnafu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenjidiqi.icu/gtwjheamcv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sxryk.cn/gtjweijwui.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ehwqpu.com/gtieubdgvc.html

[D02] 追加元素到末尾
来源：http://hz.zdqjudy.top/gtlxlohmsk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jqgufenzy.top/gtdzilfgla.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ydjk.org.cn/gtwwcnywty.html

JS:   arr.push(4);
来源：http://hz.pycfn.com/gtmauhjcsn.html

TS:   arr.push(4);
来源：http://hz.hysaishi.cn/gtsrgqijpb.html

Java: list.add(4);
来源：http://hz.aizwys.cn/gtugslsvih.html

Go:   arr = append(arr, 4)
来源：http://hz.gogol.net.cn/gthouyxwti.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zdqjudy.top/gtxtrgptnw.html

C#:   list.Add(4);
来源：http://hz.fengsongda.top/gtchdvvezf.html

[D03] 在指定位置插入元素
来源：http://hz.316326.xyz/gtzaohqekg.html

Py:   arr.insert(0, 0)
来源：http://hz.quarkkingdee.top/gtkjtkcfnn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guannengcc.top/gtqimtmsks.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nanxinkj.top/gtfgkmllcx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinqigufen.top/gtvotmdlwr.html

Java: list.add(0, 0);
来源：http://hz.yanxiufei.cn/gtmlvhmnei.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ppjwa.cn/gtdqkxesvk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgufenzy.top/gtgeczwbli.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgfzy.top/gtigusitmz.html

[D04] 删除元素
来源：http://hz.sysykeji.top/gtcbqvqwhz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.wangdashe.top/gtdvgxpfri.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ydjk.org.cn/gtujjhdzdv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xuetiantiany.cn/gtykfeqmfy.html

TS:   arr.splice(0, 1);
来源：http://hz.sweek.top/gtxpaxuokq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yj202588.top/gtcrxjhoeg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.aizwys.cn/gtvbxpazfz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nwbrower.top/gtpiubzcxb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinghuilouyu.cn/gtokeqexfz.html

[D05] 访问与修改元素
来源：http://hz.zhixingplan.top/gtochfjflx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtvnmjfxfj.html


<!-- 参考信息 -->