代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.wangshuangyany.cn/gtkdkqtold.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.gotoacloud.top/gtlzzzsmjs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.wangshuangyany.cn/gtfzbhngxn.html

Ruby: arr.each { |item| puts item }
来源：http://hz.gzhubu.top/gtvefflmcg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xylfe.cn/gtztyhsbix.html

[B06] 遍历字典 / 对象
来源：http://hz.316326.xyz/gtiyzyrxoz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jqgufenzy.top/gtuybbxown.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xinyue.icu/gtqebsqiqo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xinyue.icu/gtstxoawba.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hammf.cn/gttkzueyoz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cheryme.top/gtgmzhesqq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhiwuduotai.top/gttyhgvwnq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.tanke756.top/gtbfgobfug.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yongpay.top/gtjhhmpbsp.html

[B07] while 循环
来源：http://hz.pengpengdd.cyou/gtdrzhdgbh.html

Py:   while i < 10: i += 1
来源：http://hz.chenlongwang.top/gtnhrrbqvt.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zdqjudy.top/gtfnrzookr.html

JS:   while (i < 10) { i++; }
来源：http://hz.zdqjudy.top/gtmczfskcd.html

TS:   while (i < 10) { i++; }
来源：http://hz.jiagoushi.top/gtfsppfuru.html

Java: while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtuqchvvue.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.meibo888.top/gteyevsyjy.html

Ruby: while i < 10; i += 1; end
来源：http://hz.wangdashe.top/gtioavbpai.html

C#:   while (i < 10) { i++; }
来源：http://hz.smart0.xyz/gtclsahsyu.html

[B08] do-while（至少执行一次）
来源：http://hz.snrcjt.cn/gtcxrbehul.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.chenzaomai.com/gtkyqwgpik.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.pycfn.com/gtoqcaistf.html

JS:   do { i++; } while (i < 10);
来源：http://hz.dashuyun.cn/gtjjcpnpcw.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gtfbkqkbdv.html

Java: do { i++; } while (i < 10);
来源：http://hz.xinyue.icu/gtxaxiaefi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.fengsongda.top/gttdtrtznt.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.haohaochexian.top/gtuxoccwle.html

C#:   do { i++; } while (i < 10);
来源：http://hz.sysykeji.top/gtqboicisx.html

[B09] break 与 continue
来源：http://hz.daxiang520.top/gtwcsluyob.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.dashuyun.cn/gtfsbyolxl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hysaishi.cn/gtthgdswno.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jyoumei.cn/gtampryprl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigufen.top/gtnvfislej.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgfzy.top/gttcmerean.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.9152youxi.cn/gtfsudjjbw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hysaishi.cn/gtveuqjjbg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.redwolf501.top/gtrdjtqlld.html

[B10] 遍历同时拿索引
来源：http://hz.pycfn.com/gtztgcspdc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cqqwz.cn/gtswjxvpig.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hnqzz.top/gtnsczhqji.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ppjwa.cn/gtzsitkdkq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.chenzaomai.com/gtlqpwmrms.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jyoumei.cn/gtesookxjv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xuetiantiany.cn/gtfspmlszm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yj20258888.top/gtygytnwnj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.aibaodan.cn/gtkcqxfwer.html

[B11] 生成数字序列 / 区间
来源：http://hz.fzhhl.top/gtcrhsqzuh.html

Py:   list(range(0, 10, 2))
来源：http://hz.nanxinkj.top/gtuxlbismy.html

PHP:  range(0, 10, 2);
来源：http://hz.aizwys.cn/gtcsiosokz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.iojbl.cn/gtyxkoblxm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.redwolf501.top/gtthtgrjxk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.gogol.net.cn/gtcwytdmye.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.sxryk.cn/gtmxhwqodv.html

Ruby: (0...10).step(2).to_a
来源：http://hz.dianchejie.cn/gtrxfloqjq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenlongwang.top/gtdtufkhgp.html

[B12] 跳出多层循环
来源：http://hz.zhixingplan.top/gtrnondecq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xylfe.cn/gtvuceypsi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shanyushiyangtech.top/gtwmpdklak.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gtnpimwsay.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dianchejie.cn/gtxaogfoyx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinyuanbaomall.cn/gtjjdmrtjj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hammf.cn/gtdffszlio.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.9152youxi.cn/gtbwsardrx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.chenlongwang.top/gtewiakrqk.html

[B13] 判断是否为数字
来源：http://hz.jlsjyb.cn/gtifjilqxm.html

Py:   isinstance(x, (int, float))
来源：http://hz.nanxinkj.top/gtlzolxxwy.html

PHP:  is_numeric($x)
来源：http://hz.nanxinkj.top/gtfvdfrndg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hongshengwenyu.top/gtbavkwldh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ybcxt.top/gtrvhpkpff.html

Java: x instanceof Number
来源：http://hz.tian-w.cn/gtodsuyjah.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sxryk.cn/gtwnkovozi.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hysaishi.cn/gtnjgccoqy.html

C#:   x is int or double or decimal
来源：http://hz.52xcode.cn/gteaokkehb.html

[B14] 判断值是否在集合内
来源：http://hz.birdmap.top/gtjvoqyjof.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yangfankeji.com/gtgyyosyad.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xuanzx.com/gtuqmjhkez.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cucudq.cn/gtqhyiirek.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sxryk.cn/gtqmrhhoca.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zdqjudy.top/gtevzntxsr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hnqzz.top/gtmjfbnjen.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhaomingkeji.xyz/gtjzvtspgk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cucudq.cn/gtkssbzqtb.html

[B15] 布尔运算与取反
来源：http://hz.hfpthk.cn/gtgoytcshb.html

Py:   a and b or not c
来源：http://hz.zhoulong.xyz/gtkejnfafh.html

PHP:  $a && $b || !$c
来源：http://hz.chenjidiqi.icu/gthouhaufr.html

JS:   a && b || !c
来源：http://hz.aizwys.cn/gtirjwrqvi.html

TS:   a && b || !c
来源：http://hz.svipenyu.cn/gteaoqbxet.html

Java: a && b || !c
来源：http://hz.shuidangran.top/gtepqwntpk.html

Go:   a && b || !c
来源：http://hz.ydzc1.top/gtmvktywkz.html

Ruby: a && b || !c
来源：http://hz.jqgufenzy.top/gtvjtvwhxo.html

C#:   a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtoipqehqr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ppjwa.cn/gtgkjenwwp.html

Py:   if not data: return
来源：http://hz.tanke756.top/gtogxvujwp.html

PHP:  if (!$data) { return; }
来源：http://hz.hammf.cn/gtdothhfvs.html

JS:   if (!data) return;
来源：http://hz.jlsjyb.cn/gtcbzvulgq.html

TS:   if (!data) return;
来源：http://hz.haohaochexian.top/gtbwzcqdpy.html

Java: if (data == null) return;
来源：http://hz.yueranfly.top/gtxjdumoze.html

Go:   if data == nil { return }
来源：http://hz.hongshengwenyu.top/gtnqkvcldp.html

Ruby: return if data.nil?
来源：http://hz.andypj.xyz/gtmcqyfixv.html

C#:   if (data == null) return;
来源：http://hz.cashguo.top/gtubxybgxo.html

================================================================================
来源：http://hz.jqgufenzy.top/gtieootloo.html

C. 函数与作用域
来源：http://hz.feifeiyinyue.top/gtybjstkkq.html

================================================================================
来源：http://hz.guowangkeji.top/gtirmmrpeq.html

[C01] 定义函数
来源：http://hz.ybcxt.top/gtlpirkmlf.html

Py:   def add(a, b): return a + b
来源：http://hz.9152youxi.cn/gtnhzvrhpu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gttdaqrsee.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tianlin.xyz/gtmfyfxlcb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guowangkeji.top/gtnbgfvhre.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gttytznqcy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenjidiqi.icu/gtalgfyxve.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ybcxt.top/gtvqtscict.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtxedgqoyr.html

[C02] 默认参数
来源：http://hz.havefunace.top/gtfimnbwsp.html

Py:   def greet(name="World"): return name
来源：http://hz.zhoulong.xyz/gtdncvbirq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.52xcode.cn/gtntqaagqd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cdnleiting.top/gtzptvqpff.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ywan-chungtsiang.top/gticvnngfn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xylfe.cn/gtxanqhfqn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuanzhike.top/gtdpjdusyh.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinyuanbaomall.cn/gtqjnymtuk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.fzhhl.top/gtvkjpgebd.html

[C03] 可变参数
来源：http://hz.tianlin.xyz/gttzjwikgx.html

Py:   def total(*args): return sum(args)
来源：http://hz.nwbrower.top/gtcnwmbsaw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.andypj.xyz/gtqhvuwgyo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnxiangtu.top/gtkwdsmspe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydzc1.top/gtxzfhdoqm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ppjwa.cn/gtbvnzghbc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj20258.top/gthwywzrdg.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ivvv.top/gtjuikgwfv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yangfankeji.com/gtosmhswvd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.nanxinkj.top/gtfqjmsfmr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhaomingkeji.xyz/gtzntkfifo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.smart0.xyz/gttdptrcuf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xylfe.cn/gtojymjkmg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xinyue.icu/gtbdjmhdqe.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jlsjyb.cn/gtywublbrl.html

Go:   // 无：用配置结构体参数
来源：http://hz.hongshengwenyu.top/gtuindgqxd.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gtrxjzkoqt.html

C#:   f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtpwhsuzvt.html

[C05] 返回多个值
来源：http://hz.xylfe.cn/gtxpzivxkp.html

Py:   return a, b
来源：http://hz.yvedp.cn/gtvdptvtoa.html

PHP:  return [$a, $b];
来源：http://hz.dashuyun.cn/gtokqwkmzc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhoulong.xyz/gtqphwcoyl.html

TS:   return { a, b };
来源：http://hz.guannengcc.top/gtrqwvbpqk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jianghu66.top/gtpjllybjk.html

Go:   return a, b
来源：http://hz.jinghuilouyu.cn/gtmfwomcav.html

Ruby: return a, b
来源：http://hz.cucudq.cn/gtmatnaweu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.feifeiyinyue.top/gttwoiiehm.html

[C06] 匿名函数 / lambda
来源：http://hz.chenjidiqi.icu/gtksunjaqd.html

Py:   square = lambda x: x * x
来源：http://hz.zhiwuduotai.top/gtlnxwotgv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yuanzhike.top/gtwggwczzw.html

JS:   const square = x => x * x;
来源：http://hz.chenjidiqi.icu/gtzrpnhqpe.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hnqzz.top/gtjlbhhnnj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yongpay.top/gtrbtkzmlg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.nwbrower.top/gtkkkfrtsq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.pengpengdd.cyou/gtfjafnoom.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jqgufenzy.top/gtwadbowyo.html

[C07] 把函数作为参数传入
来源：http://hz.guowangkeji.top/gtbzettwxw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.aizwys.cn/gtrqcngykk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jqgfzy.top/gthuqdadpu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.chenzaomai.com/gtgbzbqtbt.html

TS:   arr.map(String)
来源：http://hz.snrcjt.cn/gtkvhebgki.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jinqigufen.top/gtxbrpebct.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sufxvd.cn/gtolxcnyft.html

Ruby: arr.map(&:upcase)
来源：http://hz.sufxvd.cn/gtndomtewc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.wangshuangyany.cn/gtixyxfsxa.html

[C08] 闭包
来源：http://hz.birdmap.top/gtisuvpxcl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.snrcjt.cn/gtdnssucay.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ehwqpu.com/gtowrchdjb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ppjwa.cn/gtzdzaenpr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtlzkocdoh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zdqjudy.top/gtzapkquow.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.smart0.xyz/gtgztycnwv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhiwuduotai.top/gtaolpmpgd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gtkgkljggs.html

[C09] 递归
来源：http://hz.vqdsnc.cn/gtrlolqpju.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jiagoushi.top/gtetneauje.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinyuanbaomall.cn/gtroblweqz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuxming.cn/gthyjkdkkc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pycfn.com/gthepgshnw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xuetiantiany.cn/gtuhihwogp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.haohaochexian.top/gtnvfxawsj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtqkmhexyf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yangfankeji.com/gtxdduvlsk.html

[C10] 变量作用域
来源：http://hz.sxryk.cn/gtxvzucetx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hammf.cn/gtbcjjcufs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.316326.xyz/gtrwxvqurx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sysykeji.top/gtcgtdppdm.html

TS:   同 JS
来源：http://hz.9152youxi.cn/gtlcjtgsyw.html

Java: 方法内为块级作用域
来源：http://hz.wangshuangyany.cn/gtsnbmsjzi.html

Go:   花括号块级作用域
来源：http://hz.ppjwa.cn/gtejygskln.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jianghu66.top/gtvgfnergm.html

C#:   块级作用域
来源：http://hz.tianlin.xyz/gtnousiglj.html

[C11] 模块导入与导出
来源：http://hz.quarkkingdee.top/gtjkpovloo.html

Py:   from module import func
来源：http://hz.chenlongwang.top/gtrsdqqitn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinqigufen.top/gtawvmsjiu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.mhx1999.top/gtmvtjymrx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xziqi.cn/gtxlfdneks.html

Java: import java.util.List;
来源：http://hz.birdmap.top/gtulhvovxn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zycfv.cn/gtranzebfe.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.9152youxi.cn/gtrcptcwiy.html

C#:   using System.Text;
来源：http://hz.zhijiandao.cn/gtveibbmfv.html

[C12] 立即执行函数 IIFE
来源：http://hz.yangfankeji.com/gthlhhaujh.html

Py:   (lambda: print("run"))()
来源：http://hz.zhoulong.xyz/gtmqjazvjf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.haohaochexian.top/gtlethtrkg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.chenlongwang.top/gtvcbommon.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tian-w.cn/gtkjucsyij.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.tanke756.top/gtxvjjkdwc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yvedp.cn/gtyzsizmai.html

Ruby: -> { puts "run" }.call
来源：http://hz.gogol.net.cn/gtuihuujdb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.vqdsnc.cn/gtjzrbefmr.html

[C13] 类型声明 / 类型注解
来源：http://hz.yueranfly.top/gtqhkwcbju.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guannengcc.top/gtfijzvdqv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gtksgngddl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinyuanbaomall.cn/gtwihnnmzu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydzc1.top/gtgmkrupnj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtcgyazest.html

Go:   func add(a, b int) int
来源：http://hz.ydjk.org.cn/gtikftpupj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cucudq.cn/gtmjmznypn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.kuanghao11.cn/gtvtkzxwas.html

[C14] 泛型函数
来源：http://hz.sysykeji.top/gtyzjygkfn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jiagoushi.top/gtqnwabqqf.html

PHP:  // 无泛型
来源：http://hz.gaohongyu789.top/gtwgvkwdad.html

JS:   // 无泛型
来源：http://hz.quarkkingdee.top/gtuldyhvid.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.dashuyun.cn/gtjxfbfmiw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hammf.cn/gtxhmzcjme.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinyuanbaomall.cn/gtdcueygnw.html

Ruby: # 无泛型
来源：http://hz.pycfn.com/gtehiednsq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xinyue.icu/gtlnhvrrzs.html

[C15] 解构 / 展开参数
来源：http://hz.dashuyun.cn/gtueaxltip.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.andypj.xyz/gtgpccbzcn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hammf.cn/gtsybmonxe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ydzc1.top/gtzipbvjvt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.smart0.xyz/gtgukktfad.html

Java: // 无解构
来源：http://hz.bjfxy.top/gtizmmbzai.html

Go:   // 无解构
来源：http://hz.shanyushiyangkeji.top/gtsvasuxwn.html

Ruby: a, b = pair
来源：http://hz.cheryme.top/gtkbagnunl.html

C#:   var (a, b) = pair;
来源：http://hz.quarkkingdee.top/gtjviultpp.html

[C16] 函数 / 方法重载
来源：http://hz.wangshuangyany.cn/gtoiryvdvi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinqigufen.top/gtoobbkaxf.html

PHP:  // 无重载
来源：http://hz.xingfuxueyuan.xyz/gtyhaxudyp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cashguo.top/gtvetkpprb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sxryk.cn/gtbkhzzafg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenlongwang.top/gtisfplzhs.html

Go:   // 无重载：用不同函数名
来源：http://hz.quarkkingdee.top/gtzhkfcxjm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.snrcjt.cn/gtcvdgdvvv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yangfankeji.com/gtebeplvlw.html

================================================================================
来源：http://hz.hysaishi.cn/gtnfdhtbza.html

D. 数组 / 列表 / 集合
来源：http://hz.chenzaomai.com/gtmxdqwmva.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtwedjxvxz.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtpedtoilx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xingfuxueyuan.xyz/gtzfwcalut.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.feifeiyinyue.top/gtgkcdofzg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ywan-chungtsiang.top/gtccauihvy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tanke756.top/gtwpewsdto.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.andypj.xyz/gtcaperyxk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinghuilouyu.cn/gtfrsmckif.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cqqwz.cn/gtpkjgobrr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cdnleiting.top/gtuhuvpvec.html

[D02] 追加元素到末尾
来源：http://hz.guannengcc.top/gtufzpewfy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daria6918.cn/gtstbagjvt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.guowangkeji.top/gtvcqocxoo.html

JS:   arr.push(4);
来源：http://hz.xziqi.cn/gtyvvytfhn.html

TS:   arr.push(4);
来源：http://hz.gzhubu.top/gtltqecljt.html

Java: list.add(4);
来源：http://hz.tanke756.top/gtaqklafrp.html

Go:   arr = append(arr, 4)
来源：http://hz.guowangkeji.top/gtpyrosxql.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.birdmap.top/gtpouwmrzs.html

C#:   list.Add(4);
来源：http://hz.xylfe.cn/gtbzkakgmp.html

[D03] 在指定位置插入元素
来源：http://hz.aibaodan.cn/gtichveuxi.html

Py:   arr.insert(0, 0)
来源：http://hz.jinqigufen.top/gttdxpelks.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhongyouzk.top/gtqiomzqen.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tanke756.top/gteupebthm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnqzz.top/gtoofjdrqa.html

Java: list.add(0, 0);
来源：http://hz.fengsongda.top/gtysixtiol.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.52xcode.cn/gtwwglawtu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hysaishi.cn/gtiuvklruj.html

C#:   list.Insert(0, 0);
来源：http://hz.jinqigfzy.top/gtetdxbbnu.html

[D04] 删除元素
来源：http://hz.xuetiantiany.cn/gtknbzqmfc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jqgufenzy.top/gtgcxrhngj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.feifeiyinyue.top/gtgworizeh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jianghu66.top/gtfzksndow.html

TS:   arr.splice(0, 1);
来源：http://hz.aibaodan.cn/gtfxcrrynw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.svipenyu.cn/gttdnkcphd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xinyue.icu/gtuljjnqfe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhoulong.xyz/gtqsjhuruj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yanxiufei.cn/gtpjomqcgp.html

[D05] 访问与修改元素
来源：http://hz.pycfn.com/gtxvwtonjd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.mhx1999.top/gtarunscrs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xinyue.icu/gtineyyndd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xylfe.cn/gtmexvykki.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.dianchejie.cn/gtqtgtdqfq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jyoumei.cn/gtqiiphvdm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.c1oappe.top/gtuepmszgx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tian-w.cn/gteyaqmamn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gaohongyu789.top/gthhifnina.html

[D06] 数组长度
来源：http://hz.xziqi.cn/gtpthzchnx.html


<!-- 参考信息 -->