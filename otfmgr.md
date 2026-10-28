代发 wailian999

[B05] 遍历数组 / 列表
来源：http://hz.jinyuanbaomall.cn/gtzuedtdjy.html

Py:   for item in arr: print(item)
来源：http://hz.xingfuxueyuan.xyz/gtbmzterfb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yj20258.top/gtfowxdkdw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.aizwys.cn/gtcgykamiz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.shuidangran.top/gthnkpjtvt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.9152youxi.cn/gtnbjgirtu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ehwqpu.com/gtoogozyhn.html

Ruby: arr.each { |item| puts item }
来源：http://hz.guannengcc.top/gtakqblbzb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.gzhubu.top/gtyxqcxngq.html

[B06] 遍历字典 / 对象
来源：http://hz.gotoacloud.top/gtqsouvdzm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.xylfe.cn/gtihifeslz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.daxiang520.top/gtynhxunjf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cucudq.cn/gtokjooumk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xuetiantiany.cn/gtmfbplqnm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.jiagoushi.top/gtuiimpkci.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.aizwys.cn/gtwwzuwtjh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.chenzaomai.com/gtvaxbkyal.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yvedp.cn/gtwijeyvbh.html

[B07] while 循环
来源：http://hz.jinghuilouyu.cn/gtsprtrkxs.html

Py:   while i < 10: i += 1
来源：http://hz.jinghuilouyu.cn/gtcicofwur.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xinyue.icu/gtghuhxxcm.html

JS:   while (i < 10) { i++; }
来源：http://hz.yvedp.cn/gtbqxdjemw.html

TS:   while (i < 10) { i++; }
来源：http://hz.ydjk.org.cn/gtyrmxvuij.html

Java: while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtxirunckz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.redwolf501.top/gtczcwonoh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jinghuilouyu.cn/gtjrbcsdmq.html

C#:   while (i < 10) { i++; }
来源：http://hz.tian-w.cn/gtmixwgtft.html

[B08] do-while（至少执行一次）
来源：http://hz.jinghuilouyu.cn/gtqrztiuyw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.daria6918.cn/gtobgqqxtj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.vqdsnc.cn/gtekgdbwbp.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sufxvd.cn/gtqgndvqhu.html

TS:   do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gtnvwuxvmn.html

Java: do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gtvuqmlbdk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ydzc1.top/gtmjwowlmo.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jinghuilouyu.cn/gtnspkzrvm.html

C#:   do { i++; } while (i < 10);
来源：http://hz.sxryk.cn/gtupjassqb.html

[B09] break 与 continue
来源：http://hz.wangshuangyany.cn/gtkadkumjc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.daxiang520.top/gttnrwggcr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.daria6918.cn/gthsppcxwj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guannengcc.top/gtikpeoefl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gtotxljakv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zycfv.cn/gtgkvcaffc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhaomingkeji.xyz/gtnlamfstr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.tian-w.cn/gttlfvkvyp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xylfe.cn/gttdsncdoh.html

[B10] 遍历同时拿索引
来源：http://hz.hysaishi.cn/gtjrowbjof.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zdqjudy.top/gtssbadssb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hysaishi.cn/gtdeprhmzz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.dianchejie.cn/gtbpjgtaqc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hnxiangtu.top/gtwfycelkn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yanxiufei.cn/gtmxxklgsv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.c1oappe.top/gtixlawbke.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tianlin.xyz/gtybywmgqu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.nwbrower.top/gttnayqwob.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinqigfzy.top/gtjrgoamxr.html

Py:   list(range(0, 10, 2))
来源：http://hz.fengsongda.top/gtdczhhkmp.html

PHP:  range(0, 10, 2);
来源：http://hz.zhengqikj.top/gtbijoxodh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gtsugkdnlc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.0kj1m.cn/gtcetuauww.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xziqi.cn/gtbvzyxwjk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.daria6918.cn/gtxvtgccem.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jqgufenzy.top/gtitectyhe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.quarkkingdee.top/gtnomsvgid.html

[B12] 跳出多层循环
来源：http://hz.hnqzz.top/gtvlefpiyi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.vqdsnc.cn/gtetjnepyt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gzhubu.top/gtccqgwqzv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cucudq.cn/gtgqyknhgu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yonumen.top/gtqouunmmo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hammf.cn/gtilziwpsn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.52xcode.cn/gtcbjpqbbj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.wangdashe.top/gtatnyzcjp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yangfankeji.com/gtkkpoxtkq.html

[B13] 判断是否为数字
来源：http://hz.yongpay.top/gtedkfeosx.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinqigufen.top/gttvzoarzi.html

PHP:  is_numeric($x)
来源：http://hz.jinqigfzy.top/gtlzjwrqru.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yvedp.cn/gtaggdctsg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fengsongda.top/gtdsufwoav.html

Java: x instanceof Number
来源：http://hz.yanxiufei.cn/gtwwooqbfi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.bjfxy.top/gtqnwdbpic.html

Ruby: x.is_a?(Numeric)
来源：http://hz.iojbl.cn/gtkesfcyfg.html

C#:   x is int or double or decimal
来源：http://hz.jqgufenzy.top/gthbsftwsn.html

[B14] 判断值是否在集合内
来源：http://hz.kuanghao11.cn/gtlsqylxpv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hnqzz.top/gtnxenvwgl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ydjk.org.cn/gtehbybgon.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.kuanghao11.cn/gtiwzpvhcc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.chenjidiqi.icu/gtomdgynss.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zdqjudy.top/gteghcfsmf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xylfe.cn/gtfdzuoefk.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhixingplan.top/gtffxarcdu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.dashuyun.cn/gtjjpeshbg.html

[B15] 布尔运算与取反
来源：http://hz.haohaochexian.top/gtrvpvpvsw.html

Py:   a and b or not c
来源：http://hz.shuidangran.top/gtnqpyypqh.html

PHP:  $a && $b || !$c
来源：http://hz.xingfuxueyuan.xyz/gtzamamush.html

JS:   a && b || !c
来源：http://hz.xuanzx.com/gtsjbwebjq.html

TS:   a && b || !c
来源：http://hz.yj202588.top/gtjpgxgqhj.html

Java: a && b || !c
来源：http://hz.dashuyun.cn/gteidsdgqk.html

Go:   a && b || !c
来源：http://hz.quarkkingdee.top/gtqoeckcwr.html

Ruby: a && b || !c
来源：http://hz.zhoulong.xyz/gtujgkwase.html

C#:   a && b || !c
来源：http://hz.daria6918.cn/gtylawjdne.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinyuanbaomall.cn/gtdamkrvly.html

Py:   if not data: return
来源：http://hz.52xcode.cn/gtpfijztfb.html

PHP:  if (!$data) { return; }
来源：http://hz.zhoulong.xyz/gtnlenwtwu.html

JS:   if (!data) return;
来源：http://hz.yonumen.top/gtzzbcxaac.html

TS:   if (!data) return;
来源：http://hz.cdnleiting.top/gtezdqcuna.html

Java: if (data == null) return;
来源：http://hz.zhijiandao.cn/gtykgogkpt.html

Go:   if data == nil { return }
来源：http://hz.fzhhl.top/gtymtpurqc.html

Ruby: return if data.nil?
来源：http://hz.ydzc1.top/gtzkqxxjqp.html

C#:   if (data == null) return;
来源：http://hz.yueranfly.top/gtkdzsoebz.html

================================================================================
来源：http://hz.xinyue.icu/gtxianygqn.html

C. 函数与作用域
来源：http://hz.ppjwa.cn/gtcqwdaznu.html

================================================================================
来源：http://hz.ybcxt.top/gtkvqhtswg.html

[C01] 定义函数
来源：http://hz.sxryk.cn/gtrfakglyl.html

Py:   def add(a, b): return a + b
来源：http://hz.vqdsnc.cn/gtvsiztisb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtixsacpst.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtelrhzskk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guannengcc.top/gtilducppu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtofoxqaff.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.316326.xyz/gtoatpfpiu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinghuilouyu.cn/gtchjreyot.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.guowangkeji.top/gtfbkfaild.html

[C02] 默认参数
来源：http://hz.zhongyouzk.top/gtrblxkyqi.html

Py:   def greet(name="World"): return name
来源：http://hz.tanke756.top/gtuwofonty.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.pycfn.com/gttyicfjfc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.0kj1m.cn/gtioaowyhg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.wangdashe.top/gtbkepepjk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tianlin.xyz/gttinpolrg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cucudq.cn/gtbnksttxs.html

Ruby: def greet(name = "World") = name
来源：http://hz.dashuyun.cn/gtukfjyjyn.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinqigufen.top/gttkctxukn.html

[C03] 可变参数
来源：http://hz.0kj1m.cn/gtxfbfodfl.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhiwuduotai.top/gtvcyzntpt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yangfankeji.com/gtodwawxsn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yanxiufei.cn/gtbxsmerqj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sxryk.cn/gtklwzjlqt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhoulong.xyz/gtkmsttmnj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hongshengwenyu.top/gtjcifdntb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yangfankeji.com/gtcebopbze.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yongpay.top/gthdhcdive.html

[C04] 命名参数 / 关键字参数
来源：http://hz.vqdsnc.cn/gtfgmkwupf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.0kj1m.cn/gtxoqawktb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj202588.top/gtxdpxicjh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cqqwz.cn/gthyuslyzk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hnxiangtu.top/gtakzkoyud.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gaohongyu789.top/gtczmgegyb.html

Go:   // 无：用配置结构体参数
来源：http://hz.redwolf501.top/gtxljoxiad.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenjidiqi.icu/gthrydrbnv.html

C#:   f(a: 1, b: 2)
来源：http://hz.snrcjt.cn/gttqdnsolx.html

[C05] 返回多个值
来源：http://hz.hywenlv.cn/gtdczaamgu.html

Py:   return a, b
来源：http://hz.xziqi.cn/gtvicrpiyw.html

PHP:  return [$a, $b];
来源：http://hz.havefunace.top/gtkxhnclgc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhiwuduotai.top/gtfvrtxuke.html

TS:   return { a, b };
来源：http://hz.xingfuxueyuan.xyz/gtelkibdqz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.chenlongwang.top/gtokrnpnuw.html

Go:   return a, b
来源：http://hz.sufxvd.cn/gtvphplkaa.html

Ruby: return a, b
来源：http://hz.ydjk.org.cn/gtahosmgeq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.redwolf501.top/gtjvsdqbri.html

[C06] 匿名函数 / lambda
来源：http://hz.gogol.net.cn/gtxmbsyxdt.html

Py:   square = lambda x: x * x
来源：http://hz.c1oappe.top/gtoyjnzafm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.daria6918.cn/gtbavzlfrz.html

JS:   const square = x => x * x;
来源：http://hz.jyoumei.cn/gtfowitqve.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shuidangran.top/gtksbbpzhc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hfpthk.cn/gtaqsmzjui.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.sufxvd.cn/gtlhhltpgb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cashguo.top/gtmdbubpbe.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.c1oappe.top/gteyajzbhb.html

[C07] 把函数作为参数传入
来源：http://hz.gaohongyu789.top/gtzdhjanji.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhiwuduotai.top/gtxhvitdpk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jinyuanbaomall.cn/gtvehntegf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hongshengwenyu.top/gtzdawsbru.html

TS:   arr.map(String)
来源：http://hz.aizwys.cn/gttjipphdc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhoulong.xyz/gtuhhvzwxi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xinyue.icu/gtmpmiyuvt.html

Ruby: arr.map(&:upcase)
来源：http://hz.redwolf501.top/gtckqyzkty.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.wangshuangyany.cn/gtkaxgxgls.html

[C08] 闭包
来源：http://hz.sysykeji.top/gtlhfmyjhm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hywenlv.cn/gtlakgzuvu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinqigfzy.top/gtxdccrohk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shanyushiyangtech.top/gtxuhcclcc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtwfyymstv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.fzhhl.top/gtkbshvqzz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cucudq.cn/gtqwvuxtlw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenzaomai.com/gtusplgfsl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gtrtsvzsnl.html

[C09] 递归
来源：http://hz.wangdashe.top/gtxdskdufw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gogol.net.cn/gtyncygrss.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yueranfly.top/gtjsgioeav.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hywenlv.cn/gtehotefis.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtgrokuyla.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.9152youxi.cn/gtgjtokzws.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xylfe.cn/gtphmrklkv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xuetiantiany.cn/gtowtzrurt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jyoumei.cn/gthceswkwx.html

[C10] 变量作用域
来源：http://hz.xinyue.icu/gtofhdtmjw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.daria6918.cn/gtzdndwppy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yangfankeji.com/gtruwzigwr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenlongwang.top/gteqpetrrn.html

TS:   同 JS
来源：http://hz.hywenlv.cn/gtypdyxmik.html

Java: 方法内为块级作用域
来源：http://hz.gaohongyu789.top/gtebwrusme.html

Go:   花括号块级作用域
来源：http://hz.hfpthk.cn/gthuupohxw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yangfankeji.com/gtrnabdunr.html

C#:   块级作用域
来源：http://hz.tian-w.cn/gtapmyzgaw.html

[C11] 模块导入与导出
来源：http://hz.yanxiufei.cn/gtjsxkoazl.html

Py:   from module import func
来源：http://hz.ppjwa.cn/gtksqewqbg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinqigufen.top/gtxgplmgjz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zycfv.cn/gtruabmjmy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cheryme.top/gtiufkgatj.html

Java: import java.util.List;
来源：http://hz.zycfv.cn/gtopnwnegn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jyoumei.cn/gtmpqdmynb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cashguo.top/gtpttpdrvi.html

C#:   using System.Text;
来源：http://hz.nwbrower.top/gtikiwdweq.html

[C12] 立即执行函数 IIFE
来源：http://hz.nanxinkj.top/gtpjcqqzzj.html

Py:   (lambda: print("run"))()
来源：http://hz.xingfuxueyuan.xyz/gtbhqmmjvn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.chenlongwang.top/gtvebqearw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gtwovntnev.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sxryk.cn/gtwvgjoawa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.316326.xyz/gtimwbaptj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.tanke756.top/gtoeubmbfy.html

Ruby: -> { puts "run" }.call
来源：http://hz.quarkkingdee.top/gthznfrgmo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.redwolf501.top/gtviqrsweu.html

[C13] 类型声明 / 类型注解
来源：http://hz.ivvv.top/gtuwgicvpu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shzxlz.cn/gtavybwsnl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhijiandao.cn/gtrkzinvjw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xziqi.cn/gtbqivmujt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.feifeiyinyue.top/gthveodwll.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtvqqmygvs.html

Go:   func add(a, b int) int
来源：http://hz.sufxvd.cn/gtknewymio.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.wangdashe.top/gthjmelkhy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zdqjudy.top/gtmioqeuec.html

[C14] 泛型函数
来源：http://hz.ybcxt.top/gtmbqojsnh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gaohongyu789.top/gtdqsqzqpr.html

PHP:  // 无泛型
来源：http://hz.daxiang520.top/gtonvzppzr.html

JS:   // 无泛型
来源：http://hz.nanxinkj.top/gthsmrkkjq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.nwbrower.top/gtbqkovinm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhongyouzk.top/gtkswtrdnp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xuetiantiany.cn/gttdeeagdr.html

Ruby: # 无泛型
来源：http://hz.gogol.net.cn/gtkfrisgcn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.meibo888.top/gtopzajeve.html

[C15] 解构 / 展开参数
来源：http://hz.jiagoushi.top/gtearyurmo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.wangdashe.top/gtxmkxynow.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gotoacloud.top/gtewiftkll.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.bjfxy.top/gtakpojcfe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yangfankeji.com/gtmqwtxjdz.html

Java: // 无解构
来源：http://hz.havefunace.top/gtqgrryaxk.html

Go:   // 无解构
来源：http://hz.gaohongyu789.top/gthrukixbo.html

Ruby: a, b = pair
来源：http://hz.ivvv.top/gtfwmdvvfw.html

C#:   var (a, b) = pair;
来源：http://hz.ivvv.top/gtixcvecnl.html

[C16] 函数 / 方法重载
来源：http://hz.zdqjudy.top/gtvtjqhrub.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.meibo888.top/gtubznjezy.html

PHP:  // 无重载
来源：http://hz.aizwys.cn/gtqfsrakqb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinyuanbaomall.cn/gtkcwypidm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.c1oappe.top/gtemfcedzr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ybcxt.top/gtmkxrzfss.html

Go:   // 无重载：用不同函数名
来源：http://hz.xziqi.cn/gtfpxuliwv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.fengsongda.top/gtxvhjfyci.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yuanzhike.top/gtkqtbkuka.html

================================================================================
来源：http://hz.ivvv.top/gttlwohzqa.html

D. 数组 / 列表 / 集合
来源：http://hz.cdnleiting.top/gtixavwhtb.html

================================================================================
来源：http://hz.nwbrower.top/gtlbchvlcy.html

[D01] 创建数组 / 列表
来源：http://hz.xziqi.cn/gtkoqtzgqr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuetiantiany.cn/gtfotzztow.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.aibaodan.cn/gtasognrwg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.52xcode.cn/gtumobazeu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jlsjyb.cn/gtktomvfnc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuanzhike.top/gtqjtoxkol.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.andypj.xyz/gtcmgxkcod.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hywenlv.cn/gtbucvrkce.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhoulong.xyz/gtwwkqgepc.html

[D02] 追加元素到末尾
来源：http://hz.xingfuxueyuan.xyz/gtavsdlisw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.52xcode.cn/gtgjpkeyla.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hammf.cn/gtrfldwzcd.html

JS:   arr.push(4);
来源：http://hz.shanyushiyangtech.top/gtpfdshlzd.html

TS:   arr.push(4);
来源：http://hz.wangshuangyany.cn/gtaazevjaz.html

Java: list.add(4);
来源：http://hz.fengsongda.top/gtfuszcyec.html

Go:   arr = append(arr, 4)
来源：http://hz.jqgfzy.top/gteqoilmrk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jlsjyb.cn/gtfszcwgjv.html

C#:   list.Add(4);
来源：http://hz.wangdashe.top/gtgrcvnfos.html

[D03] 在指定位置插入元素
来源：http://hz.hysaishi.cn/gtyyivuisf.html

Py:   arr.insert(0, 0)
来源：http://hz.yj20258888.top/gtvggnppzz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.vqdsnc.cn/gtzqljhlbg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.vqdsnc.cn/gttueydweg.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shuidangran.top/gtgrfqehzo.html

Java: list.add(0, 0);
来源：http://hz.xuetiantiany.cn/gtevjhcpqc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jyoumei.cn/gtvhqvzlva.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgfzy.top/gtgmqblplb.html

C#:   list.Insert(0, 0);
来源：http://hz.c1oappe.top/gtbuxvegiw.html

[D04] 删除元素
来源：http://hz.shangyingyoupin.top/gtaetkisef.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhixingplan.top/gtwtactewa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shzxlz.cn/gtzlbtuasu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guowangkeji.top/gtkjzswyuu.html

TS:   arr.splice(0, 1);
来源：http://hz.xingfuxueyuan.xyz/gtaqxtvuxk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sufxvd.cn/gthzpyminr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shangyingyoupin.top/gtfmkwjpjd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenzaomai.com/gthncomomx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinyuanbaomall.cn/gttqnbjsww.html

[D05] 访问与修改元素
来源：http://hz.vqdsnc.cn/gtmemhcokr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtexsmahev.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xylfe.cn/gtkjtdunpx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.0kj1m.cn/gtddoahdno.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ppjwa.cn/gtxfhpxrjk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tanke756.top/gtycmeqwai.html


<!-- 参考信息 -->