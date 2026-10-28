代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.cashguo.top/gtkviltqdc.html

[B06] 遍历字典 / 对象
来源：http://hz.shanyushiyangkeji.top/gtkutjvamn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.chenjidiqi.icu/gtkzjbwcbo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.bjfxy.top/gtcnnkrgaz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yonumen.top/gtsizyxboy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yangfankeji.com/gtzohiapeq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gotoacloud.top/gtahknrowu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.0kj1m.cn/gtvcgeixgn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.shuidangran.top/gtllilrcli.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.tianlin.xyz/gtbrxasgwr.html

[B07] while 循环
来源：http://hz.zhijiandao.cn/gtqysyqftr.html

Py:   while i < 10: i += 1
来源：http://hz.316326.xyz/gtolymcxgi.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zhixingplan.top/gtldndbllx.html

JS:   while (i < 10) { i++; }
来源：http://hz.tanke756.top/gtdetvjnxk.html

TS:   while (i < 10) { i++; }
来源：http://hz.snrcjt.cn/gtarqmssnq.html

Java: while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtyxlepyoe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hfpthk.cn/gtpjpbnmaf.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xuetiantiany.cn/gtfbswatnp.html

C#:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gtijkvcleh.html

[B08] do-while（至少执行一次）
来源：http://hz.svipenyu.cn/gtavnqwshy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xylfe.cn/gtcvfnvleg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.cashguo.top/gtascihwgs.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtqkkxfjmw.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhoulong.xyz/gtzgzxppgy.html

Java: do { i++; } while (i < 10);
来源：http://hz.hnqzz.top/gtiggexbdx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.vqdsnc.cn/gteettikzt.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.nwbrower.top/gtqsfsaywn.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gtzslxhcwf.html

[B09] break 与 continue
来源：http://hz.xingfuxueyuan.xyz/gtoeekiqzl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yonumen.top/gtdencfpkj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hysaishi.cn/gtdcqakdck.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gtpynwrwin.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.andypj.xyz/gtpjpaazwr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zdqjudy.top/gtvpgbitbx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.redwolf501.top/gtqzyeabke.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yuxming.cn/gtoprtwqjg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gtuhjgevmv.html

[B10] 遍历同时拿索引
来源：http://hz.sxryk.cn/gtzinrueal.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zdqjudy.top/gtnpdiadim.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zdqjudy.top/gtcipsvvul.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.tian-w.cn/gtvmmvyrll.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.0kj1m.cn/gtfpxiixdb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ppjwa.cn/gtetvrmwag.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xingfuxueyuan.xyz/gtozxahcvt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhixingplan.top/gtzflbelrp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.fzhhl.top/gtfvyyjeby.html

[B11] 生成数字序列 / 区间
来源：http://hz.kuanghao11.cn/gtuaqmrtwx.html

Py:   list(range(0, 10, 2))
来源：http://hz.daria6918.cn/gtwonxconc.html

PHP:  range(0, 10, 2);
来源：http://hz.52xcode.cn/gtomzswlxk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhixingplan.top/gtwhpluupp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gogol.net.cn/gtadhnzpgl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yvedp.cn/gtswhdighc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.fzhhl.top/gtozfwadvj.html

Ruby: (0...10).step(2).to_a
来源：http://hz.wangshuangyany.cn/gtpqtkttuv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.fzhhl.top/gtpqstlwys.html

[B12] 跳出多层循环
来源：http://hz.yueranfly.top/gtsebfwhkh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ybcxt.top/gtjyfehxdi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xinyue.icu/gtqsowwxcm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gzhubu.top/gtwigfvicu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gtfoqxmtmb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.guannengcc.top/gtzisrmbxr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.gogol.net.cn/gtjplvrace.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.haohaochexian.top/gtskthiqam.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.fengsongda.top/gtimmqpntf.html

[B13] 判断是否为数字
来源：http://hz.fengsongda.top/gtsjlpboxp.html

Py:   isinstance(x, (int, float))
来源：http://hz.sweek.top/gtyohakddz.html

PHP:  is_numeric($x)
来源：http://hz.gotoacloud.top/gtdmnxrpid.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yangfankeji.com/gtmjhvqmul.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yvedp.cn/gtdaxprsad.html

Java: x instanceof Number
来源：http://hz.dianchejie.cn/gtmikxmsse.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinqigfzy.top/gtkzmbarwb.html

Ruby: x.is_a?(Numeric)
来源：http://hz.havefunace.top/gtglkcdvmx.html

C#:   x is int or double or decimal
来源：http://hz.xuetiantiany.cn/gtixaksdca.html

[B14] 判断值是否在集合内
来源：http://hz.gaohongyu789.top/gtmxfipawp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cucudq.cn/gtawqztpue.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.redwolf501.top/gtzwkalgmc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yj20258888.top/gtjfsequua.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hnqzz.top/gteckehsyr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgufenzy.top/gtbntjimkn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.svipenyu.cn/gtfbdiynss.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.guowangkeji.top/gtxbwihbkd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tanke756.top/gtvlsblzea.html

[B15] 布尔运算与取反
来源：http://hz.guannengcc.top/gtiriekghx.html

Py:   a and b or not c
来源：http://hz.hnqzz.top/gtrshotvgb.html

PHP:  $a && $b || !$c
来源：http://hz.zycfv.cn/gtjuyuetso.html

JS:   a && b || !c
来源：http://hz.pycfn.com/gtdtuptmms.html

TS:   a && b || !c
来源：http://hz.9152youxi.cn/gtcxxrhhgs.html

Java: a && b || !c
来源：http://hz.redwolf501.top/gtqvxbigup.html

Go:   a && b || !c
来源：http://hz.guowangkeji.top/gtufciqcty.html

Ruby: a && b || !c
来源：http://hz.cucudq.cn/gtzjihgxcr.html

C#:   a && b || !c
来源：http://hz.ybcxt.top/gtebrejiad.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jqgufenzy.top/gtrsqedidw.html

Py:   if not data: return
来源：http://hz.sweek.top/gtazqddqaf.html

PHP:  if (!$data) { return; }
来源：http://hz.ydzc1.top/gthhnrzltf.html

JS:   if (!data) return;
来源：http://hz.jinyuanbaomall.cn/gtfqjurfel.html

TS:   if (!data) return;
来源：http://hz.jyoumei.cn/gtiynxencr.html

Java: if (data == null) return;
来源：http://hz.zhaomingkeji.xyz/gtqlbeeaav.html

Go:   if data == nil { return }
来源：http://hz.birdmap.top/gtpfnnpcaf.html

Ruby: return if data.nil?
来源：http://hz.zhongyouzk.top/gtktmgsgkt.html

C#:   if (data == null) return;
来源：http://hz.jianghu66.top/gtodaakoct.html

================================================================================
来源：http://hz.cdnleiting.top/gtsnsbawuz.html

C. 函数与作用域
来源：http://hz.gotoacloud.top/gtmbqyevra.html

================================================================================
来源：http://hz.guannengcc.top/gtwyfzxwek.html

[C01] 定义函数
来源：http://hz.chenjidiqi.icu/gtmtuavqus.html

Py:   def add(a, b): return a + b
来源：http://hz.gaohongyu789.top/gtcdryqarp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtdcgqvlhg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.aibaodan.cn/gtixomkbvt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtovblnrds.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jqgfzy.top/gtojaxvvxf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xuanzx.com/gtgsdhbsxq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xuetiantiany.cn/gtlyikykku.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtclyipwjg.html

[C02] 默认参数
来源：http://hz.hysaishi.cn/gtvhyaxdpt.html

Py:   def greet(name="World"): return name
来源：http://hz.dashuyun.cn/gtobjhtgvp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jqgfzy.top/gtlrbwqfus.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ppjwa.cn/gtgnboinuo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gzhubu.top/gttqtcsfep.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zycfv.cn/gtvjqxuivi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ywan-chungtsiang.top/gtbfrsrcbu.html

Ruby: def greet(name = "World") = name
来源：http://hz.dashuyun.cn/gtovltifyg.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xziqi.cn/gtqlvnocdb.html

[C03] 可变参数
来源：http://hz.yj20258.top/gtxvwdkvyj.html

Py:   def total(*args): return sum(args)
来源：http://hz.yuxming.cn/gtyddopsko.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hongshengwenyu.top/gtmyekreuq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtschwmzxd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pengpengdd.cyou/gtcshgjqly.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shanyushiyangkeji.top/gtywdzfszp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinqigfzy.top/gtigogrbuh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.havefunace.top/gtsmctiuui.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.pycfn.com/gtkrqimkxe.html

[C04] 命名参数 / 关键字参数
来源：http://hz.nanxinkj.top/gtjajuagyd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yangfankeji.com/gthrvzwfhr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xziqi.cn/gtvuczegrr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gogol.net.cn/gtxcwqappu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sxryk.cn/gtzpmfszbu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhixingplan.top/gtgwpxkdkf.html

Go:   // 无：用配置结构体参数
来源：http://hz.jlsjyb.cn/gtnbitgjvw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.aibaodan.cn/gtbxvdfixw.html

C#:   f(a: 1, b: 2)
来源：http://hz.yanxiufei.cn/gtpxpvwiye.html

[C05] 返回多个值
来源：http://hz.nanxuanxn.top/gtunxysgcb.html

Py:   return a, b
来源：http://hz.yvedp.cn/gtqzcdjzov.html

PHP:  return [$a, $b];
来源：http://hz.nanxinkj.top/gtxoewjtve.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xingfuxueyuan.xyz/gtbzzmdmci.html

TS:   return { a, b };
来源：http://hz.yangfankeji.com/gtmvaizcxb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.quarkkingdee.top/gtvokwyxpi.html

Go:   return a, b
来源：http://hz.fengsongda.top/gtwpkpnxnu.html

Ruby: return a, b
来源：http://hz.hnxiangtu.top/gtvmzkgory.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.wangdashe.top/gtonaengnw.html

[C06] 匿名函数 / lambda
来源：http://hz.snrcjt.cn/gtsxsxbisu.html

Py:   square = lambda x: x * x
来源：http://hz.hnxiangtu.top/gtlytfzxlp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.nwbrower.top/gthtotmbxe.html

JS:   const square = x => x * x;
来源：http://hz.iojbl.cn/gtqurltiug.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhaomingkeji.xyz/gtcbyijcls.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shanyushiyangtech.top/gtdgilvfjl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shanyushiyangtech.top/gtigjxeuvg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jlsjyb.cn/gthxiiaibv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tian-w.cn/gtrrwsazao.html

[C07] 把函数作为参数传入
来源：http://hz.ppjwa.cn/gtdydrwsgs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hongshengwenyu.top/gtczmwpevj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shangyingyoupin.top/gtvdqwcxij.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shanyushiyangtech.top/gtxtgfvydh.html

TS:   arr.map(String)
来源：http://hz.jinyuanbaomall.cn/gtxlextydy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.pengpengdd.cyou/gtandvreye.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangtech.top/gtjmeylczs.html

Ruby: arr.map(&:upcase)
来源：http://hz.dashuyun.cn/gtruodfsom.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hnxiangtu.top/gtwxtjqraa.html

[C08] 闭包
来源：http://hz.guowangkeji.top/gthztzknae.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.fengsongda.top/gtbhxqujzs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258.top/gtfbawynqs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gteyqyfbel.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gthvffxpss.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ehwqpu.com/gtbifykotp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.nwbrower.top/gtoqdrddnh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhoulong.xyz/gtbbbjyrli.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinqigfzy.top/gtysdlzhbu.html

[C09] 递归
来源：http://hz.jinqigfzy.top/gtiyxijoay.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daria6918.cn/gtwzsoveds.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ydjk.org.cn/gtoumsasdm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ywan-chungtsiang.top/gtktexsdqf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhiwuduotai.top/gtwoiugvme.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gzhubu.top/gtuhemtiul.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.9152youxi.cn/gtujpptezk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.birdmap.top/gtyenwoejd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yueranfly.top/gtzpneqsho.html

[C10] 变量作用域
来源：http://hz.haohaochexian.top/gtcynprdlm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hysaishi.cn/gthdtnhmqx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxinkj.top/gtpzoyytdd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.redwolf501.top/gtxseylbcl.html

TS:   同 JS
来源：http://hz.hywenlv.cn/gtxjblewvj.html

Java: 方法内为块级作用域
来源：http://hz.zhijiandao.cn/gttsiwtbyi.html

Go:   花括号块级作用域
来源：http://hz.9152youxi.cn/gtoqhvqhnp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.wangdashe.top/gtvqzsylqu.html

C#:   块级作用域
来源：http://hz.gaohongyu789.top/gtudkycojr.html

[C11] 模块导入与导出
来源：http://hz.xuetiantiany.cn/gtftaamjvv.html

Py:   from module import func
来源：http://hz.svipenyu.cn/gtfwdbnedv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.mhx1999.top/gtfvedhccc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ydjk.org.cn/gtpfzirhun.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yanxiufei.cn/gtoyvjqsuw.html

Java: import java.util.List;
来源：http://hz.316326.xyz/gtgrtqigbu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jianghu66.top/gtokhaycrx.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yangfankeji.com/gtliouwcbx.html

C#:   using System.Text;
来源：http://hz.hysaishi.cn/gtbvolzemk.html

[C12] 立即执行函数 IIFE
来源：http://hz.smart0.xyz/gtqtlefdbh.html

Py:   (lambda: print("run"))()
来源：http://hz.xuetiantiany.cn/gtqpxzekcn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.daria6918.cn/gtvgzssjsd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jqgfzy.top/gtlcdkhrcp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtupuevjly.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhijiandao.cn/gtzbjuepon.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xinyue.icu/gtrlmanzag.html

Ruby: -> { puts "run" }.call
来源：http://hz.aibaodan.cn/gtgipsmmps.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hnqzz.top/gtixlpcgos.html

[C13] 类型声明 / 类型注解
来源：http://hz.xylfe.cn/gtccocrbxc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zycfv.cn/gtxawscsse.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydzc1.top/gtrnmplslr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.aibaodan.cn/gtqsqgogpv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fengsongda.top/gtoubaaoxi.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtugltysks.html

Go:   func add(a, b int) int
来源：http://hz.shzxlz.cn/gtdkjzyfva.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.svipenyu.cn/gtcladeisj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cqqwz.cn/gtenghfqxy.html

[C14] 泛型函数
来源：http://hz.xinyue.icu/gtvwakiwze.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.andypj.xyz/gtqpuvtarq.html

PHP:  // 无泛型
来源：http://hz.sysykeji.top/gthuwzgtrh.html

JS:   // 无泛型
来源：http://hz.vqdsnc.cn/gtsmlxcanz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhaomingkeji.xyz/gtzevgkxeq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.dianchejie.cn/gtsjtioblb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cqqwz.cn/gtjbdocqrl.html

Ruby: # 无泛型
来源：http://hz.tian-w.cn/gttspwyncd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hfpthk.cn/gtxezccwfr.html

[C15] 解构 / 展开参数
来源：http://hz.gogol.net.cn/gtayarbeud.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hysaishi.cn/gtagvfhdcm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dashuyun.cn/gtpwajurnp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.9152youxi.cn/gttijptmza.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ywan-chungtsiang.top/gtbeuchhpv.html

Java: // 无解构
来源：http://hz.quarkkingdee.top/gtgzwctvxy.html

Go:   // 无解构
来源：http://hz.9152youxi.cn/gtthonwgzb.html

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gtdvuwoepb.html

C#:   var (a, b) = pair;
来源：http://hz.jianghu66.top/gtxoctdhhv.html

[C16] 函数 / 方法重载
来源：http://hz.xuanzx.com/gtwqnxbhbk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yanxiufei.cn/gtpbbvsktm.html

PHP:  // 无重载
来源：http://hz.cqqwz.cn/gtkcqtwtto.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tanke756.top/gtmytiacey.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhiwuduotai.top/gtpccrcnlz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuxming.cn/gtrxgjdqnx.html

Go:   // 无重载：用不同函数名
来源：http://hz.hnqzz.top/gtcvzpaegp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xziqi.cn/gtvbukrteb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jiagoushi.top/gtbwudmbjr.html

================================================================================
来源：http://hz.jqgfzy.top/gtfsmaxusr.html

D. 数组 / 列表 / 集合
来源：http://hz.cdnleiting.top/gtleqrexrf.html

================================================================================
来源：http://hz.jqgfzy.top/gtpzxvyyry.html

[D01] 创建数组 / 列表
来源：http://hz.kuanghao11.cn/gtzsqcfqlj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cqqwz.cn/gtcxwwsnyl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.dianchejie.cn/gtwinvgzgz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.daria6918.cn/gtymvhfaxl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.meibo888.top/gtsktqztkr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.daria6918.cn/gtkwzwsnbu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhongyouzk.top/gtnrdnxzzu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zdqjudy.top/gtirrgubbp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cheryme.top/gtautodqyr.html

[D02] 追加元素到末尾
来源：http://hz.zhoulong.xyz/gtvmwnokbu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hfpthk.cn/gtfmaetlrm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nanxuanxn.top/gtgplarzdx.html

JS:   arr.push(4);
来源：http://hz.nanxinkj.top/gtjmafoeal.html

TS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtgetobyao.html

Java: list.add(4);
来源：http://hz.jiagoushi.top/gtjfrdwqpv.html

Go:   arr = append(arr, 4)
来源：http://hz.ehwqpu.com/gtcowvdowh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yueranfly.top/gtszqanmre.html

C#:   list.Add(4);
来源：http://hz.tanke756.top/gtmmstbokr.html

[D03] 在指定位置插入元素
来源：http://hz.zhixingplan.top/gtasxnvjfp.html

Py:   arr.insert(0, 0)
来源：http://hz.sufxvd.cn/gtfedxhzmh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.tian-w.cn/gtwakqgsmy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hysaishi.cn/gtnybafbuj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yangfankeji.com/gtvxstdjer.html

Java: list.add(0, 0);
来源：http://hz.havefunace.top/gtonevrogh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenlongwang.top/gteosqfczx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xinyue.icu/gtrgykywiz.html

C#:   list.Insert(0, 0);
来源：http://hz.jinghuilouyu.cn/gthqcrcmsj.html

[D04] 删除元素
来源：http://hz.shanyushiyangtech.top/gtifkcmghn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jiagoushi.top/gtkaobjiwh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zdqjudy.top/gtqhbyfmbd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.birdmap.top/gtncwuofdy.html

TS:   arr.splice(0, 1);
来源：http://hz.zhiwuduotai.top/gtqzycdwoq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.iojbl.cn/gtkurkmmpt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sweek.top/gtgmdlpzqz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cashguo.top/gtojpsapfl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.smart0.xyz/gtazlohblb.html

[D05] 访问与修改元素
来源：http://hz.guannengcc.top/gttptwpjcv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenjidiqi.icu/gteeazqaye.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.havefunace.top/gtvvdxslgo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tianlin.xyz/gteczpdftr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jyoumei.cn/gtjctdeozq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hysaishi.cn/gtqbgxdpas.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tian-w.cn/gtreprmdfx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtlbkprjag.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hammf.cn/gtrzlhhxqn.html

[D06] 数组长度
来源：http://hz.shanyushiyangtech.top/gtxeczszel.html

Py:   len(arr)
来源：http://hz.yuanzhike.top/gtezebofhc.html

PHP:  count($arr);
来源：http://hz.tianlin.xyz/gtipfpaqdm.html

JS:   arr.length
来源：http://hz.ydjk.org.cn/gtzlnqmqkz.html

TS:   arr.length
来源：http://hz.xuanzx.com/gtnlgvquba.html


<!-- 参考信息 -->