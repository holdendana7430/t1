代发 wailian999

[B05] 遍历数组 / 列表
来源：http://hz.yuxming.cn/gtqkajnmja.html

Py:   for item in arr: print(item)
来源：http://hz.yuxming.cn/gtrylfpixs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.shanyushiyangkeji.top/gtwbcnascp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.haohaochexian.top/gtrnoyhjrz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenlongwang.top/gtqgochtyj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.snrcjt.cn/gtrtvtylav.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.snrcjt.cn/gtitvczmuy.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jqgufenzy.top/gtjfkqzcgp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.ehwqpu.com/gtbattvvpl.html

[B06] 遍历字典 / 对象
来源：http://hz.wangdashe.top/gtjjuoguqe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yj20258.top/gtuxfyogex.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.birdmap.top/gtwnuekotm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhijiandao.cn/gtenlwljku.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.pengpengdd.cyou/gtuhgzhdke.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yangfankeji.com/gtwrqhxjlb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhiwuduotai.top/gtafzasegh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xuetiantiany.cn/gttphbbhig.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.kuanghao11.cn/gtobpygghy.html

[B07] while 循环
来源：http://hz.svipenyu.cn/gtzzcpiwlc.html

Py:   while i < 10: i += 1
来源：http://hz.shangyingyoupin.top/gtazcgewqy.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.andypj.xyz/gtthtoogpg.html

JS:   while (i < 10) { i++; }
来源：http://hz.ywan-chungtsiang.top/gtkwfknsdk.html

TS:   while (i < 10) { i++; }
来源：http://hz.hongshengwenyu.top/gtoxcwkcld.html

Java: while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtmgtphany.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.nanxinkj.top/gtijiinifx.html

Ruby: while i < 10; i += 1; end
来源：http://hz.tian-w.cn/gtvgfnislr.html

C#:   while (i < 10) { i++; }
来源：http://hz.jqgfzy.top/gtlqkjyupo.html

[B08] do-while（至少执行一次）
来源：http://hz.shangyingyoupin.top/gtbtdrrygw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xinyue.icu/gtcjjyvxeq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jlsjyb.cn/gtztxyfenm.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhengqikj.top/gtgzsotjyo.html

TS:   do { i++; } while (i < 10);
来源：http://hz.xinyue.icu/gtgdzhvaop.html

Java: do { i++; } while (i < 10);
来源：http://hz.hnqzz.top/gtahnhazmj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ywan-chungtsiang.top/gtfmvfikxx.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cdnleiting.top/gtesecludl.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtnlgwnmjb.html

[B09] break 与 continue
来源：http://hz.316326.xyz/gtzkaqwmcm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.andypj.xyz/gtcxhhwlyh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.haohaochexian.top/gtugxcqbsz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtngqfdloi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnqzz.top/gtxlccolee.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xingfuxueyuan.xyz/gtkggzmbei.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xziqi.cn/gtwgyonobl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cqqwz.cn/gtudtvpsel.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guowangkeji.top/gtqlmabbvh.html

[B10] 遍历同时拿索引
来源：http://hz.gotoacloud.top/gtfyfcepwi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sweek.top/gtvhxvbqiq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gotoacloud.top/gthbaqzuve.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hammf.cn/gtfhzqobsn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jqgfzy.top/gtjvczkidv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.snrcjt.cn/gtbbtzfhty.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yuxming.cn/gtzevvlylz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ppjwa.cn/gtykujrlai.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.tanke756.top/gtijtbkmtg.html

[B11] 生成数字序列 / 区间
来源：http://hz.meibo888.top/gtgngpokmi.html

Py:   list(range(0, 10, 2))
来源：http://hz.cqqwz.cn/gtnivkcngv.html

PHP:  range(0, 10, 2);
来源：http://hz.ydzc1.top/gtmbnvjfzc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cucudq.cn/gthbhwogcn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nanxuanxn.top/gtsxpewvgo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.pengpengdd.cyou/gttzmkozgr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.tianlin.xyz/gtxhsaduwg.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zdqjudy.top/gtomforchq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shanyushiyangkeji.top/gtlvpkjeii.html

[B12] 跳出多层循环
来源：http://hz.yangfankeji.com/gtihahrtjc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.mhx1999.top/gtfoklktrd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cucudq.cn/gttjnsojmo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jlsjyb.cn/gtxzgboucz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigfzy.top/gtfubaicut.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinyuanbaomall.cn/gtvmngtzzt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.birdmap.top/gtvcnljfjt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.redwolf501.top/gtycsotsei.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.bjfxy.top/gtycjumgix.html

[B13] 判断是否为数字
来源：http://hz.andypj.xyz/gtdvjoplwe.html

Py:   isinstance(x, (int, float))
来源：http://hz.daria6918.cn/gtwnvhcgcx.html

PHP:  is_numeric($x)
来源：http://hz.redwolf501.top/gtotnnqtpo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.andypj.xyz/gtvlfkmhqf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yueranfly.top/gtdzaebwsy.html

Java: x instanceof Number
来源：http://hz.sufxvd.cn/gtktloxqos.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.pengpengdd.cyou/gthahlsbmy.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shangyingyoupin.top/gtbvdmfhsi.html

C#:   x is int or double or decimal
来源：http://hz.xuetiantiany.cn/gtjoqgginz.html

[B14] 判断值是否在集合内
来源：http://hz.tianlin.xyz/gtwfwspkzy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jlsjyb.cn/gtneffopla.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xinyue.icu/gtdwfjgcea.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.kuanghao11.cn/gtrlerruxw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cashguo.top/gtkfoilfro.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hammf.cn/gttnsigjol.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cqqwz.cn/gteqvndkto.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.chenlongwang.top/gtjevnbcmv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jqgfzy.top/gtihdxgvgs.html

[B15] 布尔运算与取反
来源：http://hz.sxryk.cn/gtseybgrmb.html

Py:   a and b or not c
来源：http://hz.nanxinkj.top/gtrhpffjue.html

PHP:  $a && $b || !$c
来源：http://hz.zhengqikj.top/gtbxgfmeyh.html

JS:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtosggikbn.html

TS:   a && b || !c
来源：http://hz.quarkkingdee.top/gtkwwplgsn.html

Java: a && b || !c
来源：http://hz.cheryme.top/gtsucfaypk.html

Go:   a && b || !c
来源：http://hz.jinqigfzy.top/gtsdxrthsa.html

Ruby: a && b || !c
来源：http://hz.yvedp.cn/gtcdrjyyed.html

C#:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtarqawbkb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinqigufen.top/gtsricqpjv.html

Py:   if not data: return
来源：http://hz.yangfankeji.com/gtwkhutgks.html

PHP:  if (!$data) { return; }
来源：http://hz.jinyuanbaomall.cn/gtmaupjkjj.html

JS:   if (!data) return;
来源：http://hz.shzxlz.cn/gtgwpgrqxl.html

TS:   if (!data) return;
来源：http://hz.shangyingyoupin.top/gtfqmiimpn.html

Java: if (data == null) return;
来源：http://hz.gaohongyu789.top/gtcabwxcnu.html

Go:   if data == nil { return }
来源：http://hz.jinqigufen.top/gteelvlrzb.html

Ruby: return if data.nil?
来源：http://hz.chenzaomai.com/gtckexxsdm.html

C#:   if (data == null) return;
来源：http://hz.cucudq.cn/gtnqzyoeol.html

================================================================================
来源：http://hz.xuanzx.com/gtuttzsinj.html

C. 函数与作用域
来源：http://hz.cdnleiting.top/gtttbdnlci.html

================================================================================
来源：http://hz.andypj.xyz/gtddvzdesu.html

[C01] 定义函数
来源：http://hz.iojbl.cn/gtwuzevbjy.html

Py:   def add(a, b): return a + b
来源：http://hz.0kj1m.cn/gtatjvdgur.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtdylcospm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.nwbrower.top/gtgygqlaap.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.c1oappe.top/gttycevvvu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtsglvfgdg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhengqikj.top/gtqznjtqyx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.iojbl.cn/gtdmniltyx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtjycsuenl.html

[C02] 默认参数
来源：http://hz.nwbrower.top/gtnkbtjtbs.html

Py:   def greet(name="World"): return name
来源：http://hz.jinyuanbaomall.cn/gtmogwqsnl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tanke756.top/gtjkdlgujw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.316326.xyz/gtxwdrqmez.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhiwuduotai.top/gtdjxsngdh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shuidangran.top/gtpxwevgvq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.andypj.xyz/gtupxhiyea.html

Ruby: def greet(name = "World") = name
来源：http://hz.chenjidiqi.icu/gtozdcnzld.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhoulong.xyz/gtpcihfjzc.html

[C03] 可变参数
来源：http://hz.yj20258.top/gtnrnjesxm.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhijiandao.cn/gteisokcwo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenjidiqi.icu/gtmrfmeygq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxinkj.top/gtlpjsnfhm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fengsongda.top/gtopxfmxwq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.guannengcc.top/gtwnesmlgi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yangfankeji.com/gtboxrxoai.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.dianchejie.cn/gteqaslqws.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yvedp.cn/gtzesqafsl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.birdmap.top/gtsuqrqxhn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hywenlv.cn/gtgrfaytjp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cashguo.top/gtflbxolwp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.guannengcc.top/gtajfiaiow.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yj20258888.top/gtqmjlrdlt.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.feifeiyinyue.top/gtyfoldqwn.html

Go:   // 无：用配置结构体参数
来源：http://hz.birdmap.top/gtzxacqbue.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtvifolirl.html

C#:   f(a: 1, b: 2)
来源：http://hz.dianchejie.cn/gtyjwufrml.html

[C05] 返回多个值
来源：http://hz.tanke756.top/gtpflgbwdy.html

Py:   return a, b
来源：http://hz.yonumen.top/gtboipdenm.html

PHP:  return [$a, $b];
来源：http://hz.sxryk.cn/gtkqhuayqy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.birdmap.top/gtsppudyek.html

TS:   return { a, b };
来源：http://hz.zdqjudy.top/gtqpvkwirj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tanke756.top/gtpbwbghjk.html

Go:   return a, b
来源：http://hz.gotoacloud.top/gtdsbozdmf.html

Ruby: return a, b
来源：http://hz.ivvv.top/gtypnnscvg.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yangfankeji.com/gtlkoreclr.html

[C06] 匿名函数 / lambda
来源：http://hz.jinyuanbaomall.cn/gtzjhmxtpq.html

Py:   square = lambda x: x * x
来源：http://hz.ydjk.org.cn/gtwigjobbh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.guowangkeji.top/gtremijfsl.html

JS:   const square = x => x * x;
来源：http://hz.zhijiandao.cn/gtnhugexam.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yongpay.top/gtkcdwaioq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gogol.net.cn/gtxqzrlpqd.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinqigfzy.top/gtatjgowvz.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinqigfzy.top/gtgoikziei.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhongyouzk.top/gttpixfkkg.html

[C07] 把函数作为参数传入
来源：http://hz.feifeiyinyue.top/gttxzotuoe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhixingplan.top/gthnnhqghz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jyoumei.cn/gtgpmqqphl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hfpthk.cn/gtpxtbctzb.html

TS:   arr.map(String)
来源：http://hz.birdmap.top/gthpqakegf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.daria6918.cn/gtmlclspua.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.haohaochexian.top/gtqbshjeyp.html

Ruby: arr.map(&:upcase)
来源：http://hz.xziqi.cn/gtamfwstfx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ywan-chungtsiang.top/gtshiyquqg.html

[C08] 闭包
来源：http://hz.yonumen.top/gtftdqtgnp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gaohongyu789.top/gtmtddgfmx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.vqdsnc.cn/gtlsgoxyvx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yvedp.cn/gtebbfspow.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gtrsyipanp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.tian-w.cn/gtwdzzyxyv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ydzc1.top/gtoikrvdtu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gogol.net.cn/gtdbkokmit.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtwilkwmwe.html

[C09] 递归
来源：http://hz.birdmap.top/gtkkrdwlin.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhaomingkeji.xyz/gtoqskrlil.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.52xcode.cn/gtmxyesogm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.birdmap.top/gtrxnvxcfo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.daria6918.cn/gtbajlhlfv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cheryme.top/gtocgcptwo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhongyouzk.top/gtkhelctez.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gtwxcnasbj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.9152youxi.cn/gtsitdjnuo.html

[C10] 变量作用域
来源：http://hz.jqgufenzy.top/gtbfgzsxuj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cucudq.cn/gtdmbnyvap.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinqigfzy.top/gtolritvzz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nwbrower.top/gtzohnfvzb.html

TS:   同 JS
来源：http://hz.daxiang520.top/gtuleehdkw.html

Java: 方法内为块级作用域
来源：http://hz.iojbl.cn/gtydoncgms.html

Go:   花括号块级作用域
来源：http://hz.xziqi.cn/gtsdqtldxa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xinyue.icu/gtmhtdozrd.html

C#:   块级作用域
来源：http://hz.smart0.xyz/gtwxsetuio.html

[C11] 模块导入与导出
来源：http://hz.sxryk.cn/gthqnhbitm.html

Py:   from module import func
来源：http://hz.vqdsnc.cn/gtlyoemjux.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nanxuanxn.top/gtnuiqyngb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ydjk.org.cn/gtasjekzqc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jyoumei.cn/gtprtbzxvu.html

Java: import java.util.List;
来源：http://hz.cheryme.top/gtxfxvoatw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yuxming.cn/gtmctoylsy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.havefunace.top/gtsbkcpgmt.html

C#:   using System.Text;
来源：http://hz.cqqwz.cn/gttneteyip.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhijiandao.cn/gtnevymnst.html

Py:   (lambda: print("run"))()
来源：http://hz.chenjidiqi.icu/gthjkraqmz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.aizwys.cn/gtijcwdfhc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangtech.top/gtwlxhdnjb.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhiwuduotai.top/gtakhotjyv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jlsjyb.cn/gtmfesuzah.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.wangdashe.top/gtsolxynid.html

Ruby: -> { puts "run" }.call
来源：http://hz.tian-w.cn/gtbckezgaq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.guowangkeji.top/gtduberaog.html

[C13] 类型声明 / 类型注解
来源：http://hz.shzxlz.cn/gtduazxpxg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.fengsongda.top/gtvibfxjnp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gthsdyvbrc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ivvv.top/gtdndihexs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sweek.top/gtnfbgszio.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtindixvtz.html

Go:   func add(a, b int) int
来源：http://hz.zhiwuduotai.top/gtvvgzvbfx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.pycfn.com/gtgzzkizyi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cqqwz.cn/gtcivpqhay.html

[C14] 泛型函数
来源：http://hz.shangyingyoupin.top/gtyenzzlou.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.feifeiyinyue.top/gtycoijycc.html

PHP:  // 无泛型
来源：http://hz.ehwqpu.com/gtqbjrdwsc.html

JS:   // 无泛型
来源：http://hz.cucudq.cn/gtoqmgyhqb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.iojbl.cn/gtzuqfqqbg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zdqjudy.top/gtxapikgmf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhengqikj.top/gtvrenfvfz.html

Ruby: # 无泛型
来源：http://hz.gogol.net.cn/gtjrsgpkek.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pycfn.com/gtgxdnqzdd.html

[C15] 解构 / 展开参数
来源：http://hz.hnxiangtu.top/gtymvfwjyp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xingfuxueyuan.xyz/gtdevkojcn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yuxming.cn/gtourfkcwj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daxiang520.top/gtwedfprzc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dianchejie.cn/gtslvxdbue.html

Java: // 无解构
来源：http://hz.shuidangran.top/gtkmqcbtyl.html

Go:   // 无解构
来源：http://hz.jianghu66.top/gtmnmldnok.html

Ruby: a, b = pair
来源：http://hz.yj20258.top/gtirdtiqps.html

C#:   var (a, b) = pair;
来源：http://hz.hfpthk.cn/gtpcpiuayo.html

[C16] 函数 / 方法重载
来源：http://hz.zycfv.cn/gtbugdwbds.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gzhubu.top/gtcuvhfjhn.html

PHP:  // 无重载
来源：http://hz.shuidangran.top/gtansqabgj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.daria6918.cn/gtzkeavukz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.havefunace.top/gtwdakyjcl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.andypj.xyz/gtfxnfnejt.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhongyouzk.top/gtugnjsgrg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nanxinkj.top/gtofgqqtbc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.havefunace.top/gtyowjxmiw.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtpcwtgoyu.html

D. 数组 / 列表 / 集合
来源：http://hz.yj202588.top/gtqhkixtvu.html

================================================================================
来源：http://hz.shzxlz.cn/gtfyvpmqhc.html

[D01] 创建数组 / 列表
来源：http://hz.ywan-chungtsiang.top/gtftqiwaft.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jlsjyb.cn/gtbxjnjamp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xinyue.icu/gttxpvzwou.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guowangkeji.top/gtalkcxext.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hongshengwenyu.top/gtzxlveclk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ivvv.top/gtmcpgdclw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.snrcjt.cn/gtkaonujtq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cqqwz.cn/gtvmtmandc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cheryme.top/gtrxliljyt.html

[D02] 追加元素到末尾
来源：http://hz.c1oappe.top/gtbmnrupay.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenlongwang.top/gtiyvcfmgn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ivvv.top/gtkbcfivrj.html

JS:   arr.push(4);
来源：http://hz.zhaomingkeji.xyz/gtzqazwqil.html

TS:   arr.push(4);
来源：http://hz.daria6918.cn/gtkmzmtoin.html

Java: list.add(4);
来源：http://hz.cashguo.top/gtcodvkezp.html

Go:   arr = append(arr, 4)
来源：http://hz.jinyuanbaomall.cn/gtymnwfzuv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ydjk.org.cn/gtkcqnokvy.html

C#:   list.Add(4);
来源：http://hz.yueranfly.top/gtvreqxbrp.html

[D03] 在指定位置插入元素
来源：http://hz.sufxvd.cn/gtrofbyjpc.html

Py:   arr.insert(0, 0)
来源：http://hz.ydzc1.top/gtuxcumuex.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zdqjudy.top/gtszouarvf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cucudq.cn/gtyuankmjf.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cashguo.top/gthcbmddmb.html

Java: list.add(0, 0);
来源：http://hz.dianchejie.cn/gtnxtfllgz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinghuilouyu.cn/gttlvlxbga.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hysaishi.cn/gtmjavwxmi.html

C#:   list.Insert(0, 0);
来源：http://hz.fengsongda.top/gtiamjhpyx.html

[D04] 删除元素
来源：http://hz.chenzaomai.com/gtnvhqxtzv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.fengsongda.top/gtotnvyrym.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhixingplan.top/gtcjsdmoxw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shanyushiyangtech.top/gtmyrsdbbc.html

TS:   arr.splice(0, 1);
来源：http://hz.yvedp.cn/gtwzxlekux.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hnxiangtu.top/gtdbifkasj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.iojbl.cn/gtjdtwbyav.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ybcxt.top/gtsftuvibw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cashguo.top/gtaikmwdkf.html

[D05] 访问与修改元素
来源：http://hz.vqdsnc.cn/gtgjuprqpb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258888.top/gteigqdeoy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zycfv.cn/gtlbxrjfos.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigufen.top/gtlkyucnsz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ppjwa.cn/gtfmiaaxtc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhiwuduotai.top/gtgfejqwgt.html


<!-- 参考信息 -->