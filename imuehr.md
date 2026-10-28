代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.cdnleiting.top/gtxuvewzjh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.gaohongyu789.top/gtglzaoliu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.xuetiantiany.cn/gtnymynyrl.html

Ruby: arr.each { |item| puts item }
来源：http://hz.andypj.xyz/gtismawfin.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.cashguo.top/gthqsibrbx.html

[B06] 遍历字典 / 对象
来源：http://hz.shangyingyoupin.top/gtuxyjxeco.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.xingfuxueyuan.xyz/gtklgvnxzq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.316326.xyz/gtycsfpzas.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gotoacloud.top/gtdvzhzrbi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jqgfzy.top/gtyemyiwzf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gaohongyu789.top/gtgjkszzoe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.pycfn.com/gtqylwqqws.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ydzc1.top/gtaiqyehdw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.daria6918.cn/gtwbzetctc.html

[B07] while 循环
来源：http://hz.cdnleiting.top/gtrrdnyuzn.html

Py:   while i < 10: i += 1
来源：http://hz.hywenlv.cn/gtiojopqob.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jqgufenzy.top/gtjwtaqkcl.html

JS:   while (i < 10) { i++; }
来源：http://hz.c1oappe.top/gtycabtolq.html

TS:   while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtjxefsfgl.html

Java: while (i < 10) { i++; }
来源：http://hz.iojbl.cn/gtzaqbpokc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.shanyushiyangkeji.top/gtqnlrtvgb.html

Ruby: while i < 10; i += 1; end
来源：http://hz.svipenyu.cn/gtywijmgof.html

C#:   while (i < 10) { i++; }
来源：http://hz.vqdsnc.cn/gtdljuvcfg.html

[B08] do-while（至少执行一次）
来源：http://hz.cdnleiting.top/gtkdvulptf.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.aibaodan.cn/gtjmqcasui.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.sysykeji.top/gtdykoesjb.html

JS:   do { i++; } while (i < 10);
来源：http://hz.svipenyu.cn/gtmvqorsmn.html

TS:   do { i++; } while (i < 10);
来源：http://hz.fzhhl.top/gtimrekkyy.html

Java: do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gthsdeuuck.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yuxming.cn/gtgxjbrfgl.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.52xcode.cn/gtuunptffv.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yuanzhike.top/gtpcgykhnl.html

[B09] break 与 continue
来源：http://hz.ppjwa.cn/gtzwzfjdfo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.iojbl.cn/gttnyvwxwc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cheryme.top/gtcteiweye.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtzpqsauto.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cdnleiting.top/gthgekojyn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yvedp.cn/gtrpogtaap.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.mhx1999.top/gtlgydqakr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.daria6918.cn/gtsvioijen.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtkzqrouzw.html

[B10] 遍历同时拿索引
来源：http://hz.guannengcc.top/gtaaoufbic.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shzxlz.cn/gtzadvppdg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.shuidangran.top/gtzcsxrcuo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.0kj1m.cn/gtmyvklrpk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shanyushiyangtech.top/gtmgqyxarg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.nanxinkj.top/gtexmxsvqt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.sysykeji.top/gttgyiwiee.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.chenlongwang.top/gtljgmdjio.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhiwuduotai.top/gtvdwcqwhq.html

[B11] 生成数字序列 / 区间
来源：http://hz.yvedp.cn/gthzcjfeyt.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhengqikj.top/gthjawbytp.html

PHP:  range(0, 10, 2);
来源：http://hz.chenlongwang.top/gttxvcwfxy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gotoacloud.top/gtffrxacxr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.bjfxy.top/gttfjxfynw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ydzc1.top/gtbezxaxby.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.nwbrower.top/gtemcefubl.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhiwuduotai.top/gtafaglrco.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.nanxinkj.top/gtcisoyduk.html

[B12] 跳出多层循环
来源：http://hz.jinyuanbaomall.cn/gtsiomzzyj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zdqjudy.top/gtqrjdqcfz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ywan-chungtsiang.top/gtlksofvgh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xingfuxueyuan.xyz/gtibxusdql.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hongshengwenyu.top/gtfghfvqxe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yanxiufei.cn/gtqtytgxfh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yueranfly.top/gtuvobpkpy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.feifeiyinyue.top/gtozqosqya.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.c1oappe.top/gtljycnilf.html

[B13] 判断是否为数字
来源：http://hz.zhengqikj.top/gtqxfuflsg.html

Py:   isinstance(x, (int, float))
来源：http://hz.gaohongyu789.top/gtwulhwkoa.html

PHP:  is_numeric($x)
来源：http://hz.zhengqikj.top/gtjnfpejbz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hammf.cn/gtcjcmlcyg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jiagoushi.top/gtndtntnxx.html

Java: x instanceof Number
来源：http://hz.nanxuanxn.top/gtbbmhyota.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jianghu66.top/gtbfkcackd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shuidangran.top/gtbmysalzv.html

C#:   x is int or double or decimal
来源：http://hz.chenzaomai.com/gtgbaljrdm.html

[B14] 判断值是否在集合内
来源：http://hz.wangshuangyany.cn/gtdwfmixod.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinqigufen.top/gtdprnhnbh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nanxinkj.top/gtplfasevs.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhiwuduotai.top/gtxgmvfasc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.daria6918.cn/gtjvnpdpdu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.9152youxi.cn/gtqaaizdgp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hongshengwenyu.top/gtiehnlnzt.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cashguo.top/gtldykkufo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yangfankeji.com/gtwtmdxmfm.html

[B15] 布尔运算与取反
来源：http://hz.gotoacloud.top/gtvsxhnkqd.html

Py:   a and b or not c
来源：http://hz.sweek.top/gtlzyvlvuv.html

PHP:  $a && $b || !$c
来源：http://hz.chenjidiqi.icu/gthirrunje.html

JS:   a && b || !c
来源：http://hz.ydjk.org.cn/gtxcbslkim.html

TS:   a && b || !c
来源：http://hz.316326.xyz/gtfxplodia.html

Java: a && b || !c
来源：http://hz.jqgufenzy.top/gtmdvtypre.html

Go:   a && b || !c
来源：http://hz.jianghu66.top/gtlhgilgyk.html

Ruby: a && b || !c
来源：http://hz.zhoulong.xyz/gtswadfewv.html

C#:   a && b || !c
来源：http://hz.zhengqikj.top/gthpjdqpsq.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tianlin.xyz/gtubwpwppx.html

Py:   if not data: return
来源：http://hz.smart0.xyz/gtlqlvdeyk.html

PHP:  if (!$data) { return; }
来源：http://hz.316326.xyz/gtxnyaatau.html

JS:   if (!data) return;
来源：http://hz.chenzaomai.com/gtxntagqii.html

TS:   if (!data) return;
来源：http://hz.aizwys.cn/gtgsbldyze.html

Java: if (data == null) return;
来源：http://hz.c1oappe.top/gtsumhqccf.html

Go:   if data == nil { return }
来源：http://hz.c1oappe.top/gtmjkstrnj.html

Ruby: return if data.nil?
来源：http://hz.zycfv.cn/gtrhiysrwi.html

C#:   if (data == null) return;
来源：http://hz.nanxinkj.top/gtwqquxsue.html

================================================================================
来源：http://hz.jinqigfzy.top/gtitjpospj.html

C. 函数与作用域
来源：http://hz.hysaishi.cn/gtoytkrgqr.html

================================================================================
来源：http://hz.cheryme.top/gtxduyglew.html

[C01] 定义函数
来源：http://hz.redwolf501.top/gtedufpykx.html

Py:   def add(a, b): return a + b
来源：http://hz.jinghuilouyu.cn/gtndilhmge.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.c1oappe.top/gtfaziepmf.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtvsfjyuex.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.havefunace.top/gtglvllthp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtktccwodx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhijiandao.cn/gthxqrvwhp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenzaomai.com/gtfajhngoo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtkkkphmiv.html

[C02] 默认参数
来源：http://hz.yvedp.cn/gtwjqpzocn.html

Py:   def greet(name="World"): return name
来源：http://hz.shanyushiyangkeji.top/gtioefjhab.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.pengpengdd.cyou/gtylsbjbxc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.wangdashe.top/gtvucokgrj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.dianchejie.cn/gtxgolxffr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cashguo.top/gtoatrlaui.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jiagoushi.top/gtlqvjjpht.html

Ruby: def greet(name = "World") = name
来源：http://hz.sweek.top/gtlzvhlkui.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shanyushiyangtech.top/gtcykjrfzl.html

[C03] 可变参数
来源：http://hz.fzhhl.top/gtraiomurr.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhixingplan.top/gtcvyvalye.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dashuyun.cn/gtolmfprve.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.andypj.xyz/gtjuejyiim.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gttcbmjikj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.aibaodan.cn/gtjkigmycc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shangyingyoupin.top/gtkcxwpbdo.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.fengsongda.top/gtimojrxhw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fengsongda.top/gtnyljzsjg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xylfe.cn/gtxybzuhrc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cheryme.top/gtcnuwyfuf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jqgfzy.top/gtizcfgodk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tanke756.top/gtsupdcsvl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.havefunace.top/gtcekkbwzw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.316326.xyz/gtdaltogwc.html

Go:   // 无：用配置结构体参数
来源：http://hz.smart0.xyz/gtzeugremm.html

Ruby: f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtwqtkmlqq.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtxbnnezao.html

[C05] 返回多个值
来源：http://hz.cheryme.top/gtrugemvha.html

Py:   return a, b
来源：http://hz.tanke756.top/gtzsunokmx.html

PHP:  return [$a, $b];
来源：http://hz.xziqi.cn/gtciqcaqfy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.andypj.xyz/gtupdecejz.html

TS:   return { a, b };
来源：http://hz.jianghu66.top/gtkcsnqelg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.feifeiyinyue.top/gtpcayxkhj.html

Go:   return a, b
来源：http://hz.vqdsnc.cn/gtafxcfnlw.html

Ruby: return a, b
来源：http://hz.yj202588.top/gtcmeybtir.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dianchejie.cn/gtfenaitvi.html

[C06] 匿名函数 / lambda
来源：http://hz.hywenlv.cn/gtkvclybve.html

Py:   square = lambda x: x * x
来源：http://hz.shzxlz.cn/gtwsjhtxxc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xuetiantiany.cn/gthvdcodft.html

JS:   const square = x => x * x;
来源：http://hz.andypj.xyz/gttggjxgat.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.kuanghao11.cn/gtycykavgq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shzxlz.cn/gtprqwfprz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.guannengcc.top/gtsmywipnh.html

Ruby: square = ->(x) { x * x }
来源：http://hz.c1oappe.top/gtrfnryorh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.mhx1999.top/gtnsyrhzif.html

[C07] 把函数作为参数传入
来源：http://hz.0kj1m.cn/gtlbemhepm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinqigfzy.top/gtyrolgxqj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tian-w.cn/gtdpzefooz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jyoumei.cn/gtynosjppq.html

TS:   arr.map(String)
来源：http://hz.daxiang520.top/gtfkuvoazd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.dashuyun.cn/gtbclicexn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.dashuyun.cn/gtbrsdoupy.html

Ruby: arr.map(&:upcase)
来源：http://hz.yuxming.cn/gtdkvtgfij.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gogol.net.cn/gtlgcfemrl.html

[C08] 闭包
来源：http://hz.gaohongyu789.top/gtnydwczwz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.52xcode.cn/gtiomozrlx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.0kj1m.cn/gtajdicsht.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtpdvkqfty.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.pycfn.com/gthgagubad.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jqgfzy.top/gthpmejwhi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jqgfzy.top/gtbviqybsd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.smart0.xyz/gtgkbtshvb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj202588.top/gtqijpnkky.html

[C09] 递归
来源：http://hz.fengsongda.top/gtjvvnqxfa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtiyvvjbou.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.fzhhl.top/gtdbidmndb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenlongwang.top/gtuiepzsqt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shzxlz.cn/gtycbpdaih.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gogol.net.cn/gtppztzasv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhiwuduotai.top/gtkehdnkdy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hysaishi.cn/gtmhgvdqhy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zdqjudy.top/gtuppimdcg.html

[C10] 变量作用域
来源：http://hz.hammf.cn/gtbpovfegx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cqqwz.cn/gtxddknzbc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.dashuyun.cn/gtvluzdwcr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shangyingyoupin.top/gtspjugrck.html

TS:   同 JS
来源：http://hz.smart0.xyz/gtwkrprasm.html

Java: 方法内为块级作用域
来源：http://hz.jiagoushi.top/gthobnzivp.html

Go:   花括号块级作用域
来源：http://hz.yj202588.top/gtkydmeflj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhoulong.xyz/gtepjrempj.html

C#:   块级作用域
来源：http://hz.ehwqpu.com/gtffojonug.html

[C11] 模块导入与导出
来源：http://hz.mhx1999.top/gtwkbwvulf.html

Py:   from module import func
来源：http://hz.snrcjt.cn/gtktsodcik.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ivvv.top/gtlfmvenoo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.0kj1m.cn/gtfwtrsswb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ehwqpu.com/gtiqjxfvjp.html

Java: import java.util.List;
来源：http://hz.vqdsnc.cn/gtzzpqxcwn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydjk.org.cn/gtfgizasbk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhixingplan.top/gtsakcyose.html

C#:   using System.Text;
来源：http://hz.zycfv.cn/gttumbnjzf.html

[C12] 立即执行函数 IIFE
来源：http://hz.xingfuxueyuan.xyz/gtuudfgnma.html

Py:   (lambda: print("run"))()
来源：http://hz.hywenlv.cn/gtxzffbhgh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhengqikj.top/gtvfwmiiew.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sufxvd.cn/gtnetniguh.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yvedp.cn/gtemnjhuns.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nwbrower.top/gtwbmpdcmd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jiagoushi.top/gthmchrcad.html

Ruby: -> { puts "run" }.call
来源：http://hz.meibo888.top/gterpcscgg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cqqwz.cn/gthaqzuqas.html

[C13] 类型声明 / 类型注解
来源：http://hz.cheryme.top/gtebnhkxan.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangshuangyany.cn/gtrxafdjhy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tianlin.xyz/gtdyzkycgp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.redwolf501.top/gttsuckrrl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guowangkeji.top/gtemnjohlh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinqigfzy.top/gtgjlnlszw.html

Go:   func add(a, b int) int
来源：http://hz.redwolf501.top/gtabxcdsag.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gzhubu.top/gtgtffgkdp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ydzc1.top/gtqktiazjc.html

[C14] 泛型函数
来源：http://hz.hnxiangtu.top/gtzkweeido.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.dianchejie.cn/gtrwwvuxnb.html

PHP:  // 无泛型
来源：http://hz.gotoacloud.top/gtegyexsek.html

JS:   // 无泛型
来源：http://hz.zhengqikj.top/gtutdoowkh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jyoumei.cn/gtbtpspdyf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangdashe.top/gtpixoqbhu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinghuilouyu.cn/gtikabptse.html

Ruby: # 无泛型
来源：http://hz.0kj1m.cn/gtuynrisie.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cashguo.top/gtlivibech.html

[C15] 解构 / 展开参数
来源：http://hz.chenlongwang.top/gtsxvlhuhh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xuetiantiany.cn/gtdldnodaj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gogol.net.cn/gtxcdgzeth.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhijiandao.cn/gtjqcnurqr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shanyushiyangtech.top/gtoqdwybdl.html

Java: // 无解构
来源：http://hz.cashguo.top/gtukdqwrmh.html

Go:   // 无解构
来源：http://hz.daria6918.cn/gtzhvmmdho.html

Ruby: a, b = pair
来源：http://hz.ivvv.top/gtmccbnfxt.html

C#:   var (a, b) = pair;
来源：http://hz.wangdashe.top/gtoeaaxlkh.html

[C16] 函数 / 方法重载
来源：http://hz.hysaishi.cn/gtvnccqhco.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tanke756.top/gttiwqjdzc.html

PHP:  // 无重载
来源：http://hz.gogol.net.cn/gtrrhzapws.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hywenlv.cn/gtuxstrdwf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.guannengcc.top/gtlkruatdd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj20258.top/gtqxqfvfjh.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj20258888.top/gtkgtzgunz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gogol.net.cn/gtdmzfwhjr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jiagoushi.top/gtsorqejnt.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmtgbmzmq.html

D. 数组 / 列表 / 集合
来源：http://hz.meibo888.top/gtnbmhztcr.html

================================================================================
来源：http://hz.cqqwz.cn/gthmtiaixq.html

[D01] 创建数组 / 列表
来源：http://hz.zhaomingkeji.xyz/gtgdipnkjv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xinyue.icu/gtrjlynxvk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jiagoushi.top/gtdjsqdzox.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hnqzz.top/gtsjiorvit.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zycfv.cn/gtisrznczz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenzaomai.com/gtpuodutqy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.svipenyu.cn/gtlqabiwtt.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnxiangtu.top/gtrpcfgojn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ppjwa.cn/gthiyktzmw.html

[D02] 追加元素到末尾
来源：http://hz.tianlin.xyz/gtiapjujlt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.svipenyu.cn/gtmbhabctk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shuidangran.top/gtliikwfvv.html

JS:   arr.push(4);
来源：http://hz.yuxming.cn/gtznbpetgg.html

TS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtojdwafkq.html

Java: list.add(4);
来源：http://hz.meibo888.top/gtvnivyzam.html

Go:   arr = append(arr, 4)
来源：http://hz.ehwqpu.com/gtggvakiqa.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cdnleiting.top/gtxbwfdjyn.html

C#:   list.Add(4);
来源：http://hz.sufxvd.cn/gtvuxrkrqk.html

[D03] 在指定位置插入元素
来源：http://hz.52xcode.cn/gtbegbcnur.html

Py:   arr.insert(0, 0)
来源：http://hz.ivvv.top/gtashfhxnt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj20258.top/gtwyuldsao.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.fengsongda.top/gtqlcwxpro.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.c1oappe.top/gtrkfslkxi.html

Java: list.add(0, 0);
来源：http://hz.dashuyun.cn/gtnrxpcewy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuetiantiany.cn/gtsjasijki.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gotoacloud.top/gtalcwhenf.html

C#:   list.Insert(0, 0);
来源：http://hz.cashguo.top/gtmhcqyzvr.html

[D04] 删除元素
来源：http://hz.zhijiandao.cn/gtfmaxnsyk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yj202588.top/gtufoqwlvi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.wangdashe.top/gttrujwwdw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cheryme.top/gtvtnxvokg.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigufen.top/gtovmycsvk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhijiandao.cn/gtwfalhqwu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shanyushiyangkeji.top/gtkriggzzh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.dianchejie.cn/gtqbluatnc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cheryme.top/gtnrvqxnfi.html

[D05] 访问与修改元素
来源：http://hz.mhx1999.top/gteqzpwyye.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nwbrower.top/gtxtbrmsha.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hongshengwenyu.top/gtrlwwbwrg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shuidangran.top/gtoyakbjsj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.0kj1m.cn/gtarkuskdj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.pycfn.com/gtudlysrtd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtgoktrbix.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtomexodze.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhijiandao.cn/gtjykohbng.html

[D06] 数组长度
来源：http://hz.hysaishi.cn/gtmtowrhlw.html


<!-- 参考信息 -->