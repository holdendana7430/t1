代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ydjk.org.cn/gtbjlejaua.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ydzc1.top/gtpqkpalel.html

Ruby: 10.times { |i| puts i }
来源：http://hz.aibaodan.cn/gtvsexkkth.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xuanzx.com/gtollpcxut.html

[B05] 遍历数组 / 列表
来源：http://hz.yj20258888.top/gtygapfdnb.html

Py:   for item in arr: print(item)
来源：http://hz.haohaochexian.top/gtvjjslefu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.dashuyun.cn/gtsgqvvreb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yangfankeji.com/gtigaamurc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.tian-w.cn/gtipfkxivp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.havefunace.top/gtsxfdqtqe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.quarkkingdee.top/gtdqvqgecg.html

Ruby: arr.each { |item| puts item }
来源：http://hz.meibo888.top/gtpixzibhg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.vqdsnc.cn/gtslkwcrds.html

[B06] 遍历字典 / 对象
来源：http://hz.ydjk.org.cn/gtxpbpxycn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.vqdsnc.cn/gtncjjeaaj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.kuanghao11.cn/gtifztbbpe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gogol.net.cn/gthounsrri.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.quarkkingdee.top/gtuhnleudz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.haohaochexian.top/gtwklclgpn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xziqi.cn/gthrxjiuds.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.gogol.net.cn/gtjgacyvve.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.wangdashe.top/gtxziuryjy.html

[B07] while 循环
来源：http://hz.9152youxi.cn/gthxhyhprb.html

Py:   while i < 10: i += 1
来源：http://hz.ywan-chungtsiang.top/gtqgunffuk.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.daria6918.cn/gthtslhcth.html

JS:   while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gtsvvqubnk.html

TS:   while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gtafglhvgk.html

Java: while (i < 10) { i++; }
来源：http://hz.dianchejie.cn/gtiibyegmp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.daria6918.cn/gtckjhnwgh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jiagoushi.top/gtixubmafu.html

C#:   while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gttwwqveuq.html

[B08] do-while（至少执行一次）
来源：http://hz.cqqwz.cn/gteczfbrxj.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.feifeiyinyue.top/gtspfellzc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.sysykeji.top/gthxzrrxqs.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yueranfly.top/gtvxqzwtro.html

TS:   do { i++; } while (i < 10);
来源：http://hz.chenlongwang.top/gtydqehweu.html

Java: do { i++; } while (i < 10);
来源：http://hz.sysykeji.top/gtyxyqwytq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cqqwz.cn/gtiselphbe.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jlsjyb.cn/gtutjlhyvq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.guannengcc.top/gtipczgvcy.html

[B09] break 与 continue
来源：http://hz.ydjk.org.cn/gtaerncryk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yangfankeji.com/gtglgndslq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtlpzuabze.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fzhhl.top/gtihofgxjx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jianghu66.top/gtnyyqixwd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.iojbl.cn/gtbafrxbhl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.snrcjt.cn/gtapxlrzgy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.guannengcc.top/gtqsocgmkq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhixingplan.top/gtuxlhlton.html

[B10] 遍历同时拿索引
来源：http://hz.guannengcc.top/gtruywsdyz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ybcxt.top/gthckwvdfe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gaohongyu789.top/gtadbzkfek.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zycfv.cn/gtngyutxyl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.cheryme.top/gtqgtpxfzt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.quarkkingdee.top/gtwvhsoxbk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yanxiufei.cn/gtbxmtbebm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.c1oappe.top/gtyrhmfucg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shuidangran.top/gtwqcuqqdo.html

[B11] 生成数字序列 / 区间
来源：http://hz.ehwqpu.com/gtroirndcz.html

Py:   list(range(0, 10, 2))
来源：http://hz.mhx1999.top/gtsjwbsoaq.html

PHP:  range(0, 10, 2);
来源：http://hz.ppjwa.cn/gtwyikvizf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tian-w.cn/gthdtxnijl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fengsongda.top/gtclxdyugi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.sufxvd.cn/gtudxipadk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gogol.net.cn/gtiniqnmcg.html

Ruby: (0...10).step(2).to_a
来源：http://hz.quarkkingdee.top/gtmcpjkjuj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ydzc1.top/gtwhfhwjqt.html

[B12] 跳出多层循环
来源：http://hz.nanxinkj.top/gtpibiaekn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xingfuxueyuan.xyz/gtimdowwqa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sufxvd.cn/gtuepulodg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guannengcc.top/gtzbxhpwij.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtdvelcswi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtyhrdouxl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.bjfxy.top/gtvxuaowkj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.redwolf501.top/gttqwvpfyh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cdnleiting.top/gtqzslwswd.html

[B13] 判断是否为数字
来源：http://hz.zycfv.cn/gtxpbjlyqi.html

Py:   isinstance(x, (int, float))
来源：http://hz.jiagoushi.top/gtyczunayr.html

PHP:  is_numeric($x)
来源：http://hz.chenjidiqi.icu/gtwnstbxsg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.9152youxi.cn/gtinxmihkr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.vqdsnc.cn/gtbrkebfqc.html

Java: x instanceof Number
来源：http://hz.kuanghao11.cn/gteuvsfdhw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.chenlongwang.top/gtfmevxxry.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jianghu66.top/gtglgurmul.html

C#:   x is int or double or decimal
来源：http://hz.snrcjt.cn/gthqvhhlun.html

[B14] 判断值是否在集合内
来源：http://hz.pengpengdd.cyou/gtgxdyydfl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhiwuduotai.top/gtghhiwntf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jiagoushi.top/gtuekscvxj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.nanxuanxn.top/gtizqwjkyt.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.quarkkingdee.top/gtjbobmthb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nwbrower.top/gtlxyiopoy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hnqzz.top/gtncolksyo.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.chenlongwang.top/gtkvdjxczx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.guowangkeji.top/gtfyofctvp.html

[B15] 布尔运算与取反
来源：http://hz.svipenyu.cn/gttdrsuhid.html

Py:   a and b or not c
来源：http://hz.yuanzhike.top/gtooxjnvnt.html

PHP:  $a && $b || !$c
来源：http://hz.pycfn.com/gttrvxzqyi.html

JS:   a && b || !c
来源：http://hz.hfpthk.cn/gtdjnnlabr.html

TS:   a && b || !c
来源：http://hz.wangshuangyany.cn/gthibfupym.html

Java: a && b || !c
来源：http://hz.xinyue.icu/gtehwlmflu.html

Go:   a && b || !c
来源：http://hz.daxiang520.top/gtrdvhbszl.html

Ruby: a && b || !c
来源：http://hz.ydzc1.top/gtxvygplmb.html

C#:   a && b || !c
来源：http://hz.jlsjyb.cn/gtonuhpook.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.svipenyu.cn/gtpnttcwtt.html

Py:   if not data: return
来源：http://hz.jyoumei.cn/gtabvjkmxd.html

PHP:  if (!$data) { return; }
来源：http://hz.xinyue.icu/gtedjzqyht.html

JS:   if (!data) return;
来源：http://hz.aibaodan.cn/gtiwunhkyz.html

TS:   if (!data) return;
来源：http://hz.shuidangran.top/gtvzxgsxko.html

Java: if (data == null) return;
来源：http://hz.sxryk.cn/gtlunipake.html

Go:   if data == nil { return }
来源：http://hz.chenlongwang.top/gtoglzoamt.html

Ruby: return if data.nil?
来源：http://hz.svipenyu.cn/gtvhesaxhh.html

C#:   if (data == null) return;
来源：http://hz.mhx1999.top/gtthghsezy.html

================================================================================
来源：http://hz.cdnleiting.top/gtnejowljm.html

C. 函数与作用域
来源：http://hz.gogol.net.cn/gtkjcdqlsa.html

================================================================================
来源：http://hz.zycfv.cn/gttnsnyxmg.html

[C01] 定义函数
来源：http://hz.jinqigfzy.top/gtfgtzxzjg.html

Py:   def add(a, b): return a + b
来源：http://hz.cheryme.top/gtgjqrvhpv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtxiepqxgv.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.sufxvd.cn/gtdrtnfhpo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.birdmap.top/gttjcgdmkz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtgaxnqbda.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.meibo888.top/gtevwhrigt.html

Ruby: def add(a, b); a + b; end
来源：http://hz.andypj.xyz/gtwzouxtbw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtyybjcvta.html

[C02] 默认参数
来源：http://hz.gotoacloud.top/gtxzmhbmfi.html

Py:   def greet(name="World"): return name
来源：http://hz.redwolf501.top/gtwvmdutfg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shuidangran.top/gtduagqyfs.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hongshengwenyu.top/gteuepxscu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinqigfzy.top/gtylnifkxr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cashguo.top/gtzcwfraeo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sweek.top/gtwibucahl.html

Ruby: def greet(name = "World") = name
来源：http://hz.gaohongyu789.top/gtestiuxfm.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tianlin.xyz/gtqjcpodez.html

[C03] 可变参数
来源：http://hz.dashuyun.cn/gtcstjaulw.html

Py:   def total(*args): return sum(args)
来源：http://hz.andypj.xyz/gtjjtpzwod.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhijiandao.cn/gtxxnzojql.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxuanxn.top/gtnofnudnp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenlongwang.top/gtoopdzihj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.snrcjt.cn/gtqntpowqy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yongpay.top/gtpvsbbsdg.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nwbrower.top/gtmiarjcky.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yongpay.top/gtjhwzjcgw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinyuanbaomall.cn/gtkvnwlvwa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xziqi.cn/gtkmccniga.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ydzc1.top/gtikqcdrvq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gtbtxrohhh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhoulong.xyz/gtrpxyyemj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.dianchejie.cn/gtobfrllig.html

Go:   // 无：用配置结构体参数
来源：http://hz.bjfxy.top/gthnzgwbbz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtjgeropek.html

C#:   f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gtjmizkbrp.html

[C05] 返回多个值
来源：http://hz.fzhhl.top/gtctzpzkct.html

Py:   return a, b
来源：http://hz.sysykeji.top/gtzdwtfapc.html

PHP:  return [$a, $b];
来源：http://hz.yuanzhike.top/gttbvojzdd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hnxiangtu.top/gtxmcesfbb.html

TS:   return { a, b };
来源：http://hz.yangfankeji.com/gtkclrirhw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xziqi.cn/gtpkalbpck.html

Go:   return a, b
来源：http://hz.shanyushiyangtech.top/gtfldyxpgc.html

Ruby: return a, b
来源：http://hz.bjfxy.top/gtdpqvdffi.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinqigufen.top/gtvtuyzrsc.html

[C06] 匿名函数 / lambda
来源：http://hz.bjfxy.top/gtdmkvavbz.html

Py:   square = lambda x: x * x
来源：http://hz.aizwys.cn/gtagysuiwu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yueranfly.top/gtofwlasae.html

JS:   const square = x => x * x;
来源：http://hz.yj202588.top/gtaofyncml.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.wangshuangyany.cn/gtshevtaag.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.havefunace.top/gtrmrsbedm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ybcxt.top/gtjheklnvd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shzxlz.cn/gtcvxcjkue.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hnqzz.top/gtyisiyudd.html

[C07] 把函数作为参数传入
来源：http://hz.ydjk.org.cn/gtrgmjtycr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jlsjyb.cn/gtoqfelsru.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhaomingkeji.xyz/gtfzdfnvib.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shanyushiyangtech.top/gtwxckghkz.html

TS:   arr.map(String)
来源：http://hz.nwbrower.top/gtntpjbgbv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgfzy.top/gtsriqbooc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.wangshuangyany.cn/gthitbqdbm.html

Ruby: arr.map(&:upcase)
来源：http://hz.yvedp.cn/gtjmjlwkzn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fzhhl.top/gtxjboouig.html

[C08] 闭包
来源：http://hz.nanxinkj.top/gtzzrirggz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.dashuyun.cn/gtqkcugsuj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ehwqpu.com/gtwembgvcp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtmgmdzouz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hongshengwenyu.top/gtancycoxb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shzxlz.cn/gtjgdgejvk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.wangshuangyany.cn/gtfhsosvnr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhijiandao.cn/gtfnpopngh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.aizwys.cn/gtcopzjzyx.html

[C09] 递归
来源：http://hz.ehwqpu.com/gtzrohiitm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jyoumei.cn/gtviszivkj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shuidangran.top/gtleyxuumh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhiwuduotai.top/gtrzcqhver.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xziqi.cn/gtwytogpzi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xinyue.icu/gtxytvcubk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.birdmap.top/gtrkmwscnn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.aibaodan.cn/gtdbaqtfiz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.iojbl.cn/gtozhdyotw.html

[C10] 变量作用域
来源：http://hz.shanyushiyangtech.top/gtwdtrxtpv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yongpay.top/gttvphpweh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jianghu66.top/gtylirhrsd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinqigfzy.top/gtrgpfqkuq.html

TS:   同 JS
来源：http://hz.fengsongda.top/gtikjmtnsz.html

Java: 方法内为块级作用域
来源：http://hz.zhixingplan.top/gtyfjyjibp.html

Go:   花括号块级作用域
来源：http://hz.ehwqpu.com/gtmvmgmxgd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.dashuyun.cn/gtqlladgzp.html

C#:   块级作用域
来源：http://hz.jlsjyb.cn/gttkkczztg.html

[C11] 模块导入与导出
来源：http://hz.sysykeji.top/gtscrldwmt.html

Py:   from module import func
来源：http://hz.iojbl.cn/gttuibpjdt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xuetiantiany.cn/gtfwtuwksh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sweek.top/gtugdcveqs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.daxiang520.top/gtehfjbsuy.html

Java: import java.util.List;
来源：http://hz.jinghuilouyu.cn/gthzkytpbh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.feifeiyinyue.top/gtshfhmjcu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.guowangkeji.top/gtbftzpulf.html

C#:   using System.Text;
来源：http://hz.xingfuxueyuan.xyz/gtbwiwtbqk.html

[C12] 立即执行函数 IIFE
来源：http://hz.shanyushiyangtech.top/gtcjvckziy.html

Py:   (lambda: print("run"))()
来源：http://hz.xuetiantiany.cn/gthtbwdwld.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shzxlz.cn/gtdcjvnabe.html

JS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gtqgddjrcj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.aizwys.cn/gtmqqsrtls.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sxryk.cn/gtfrioifjv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nanxuanxn.top/gtsqflohnc.html

Ruby: -> { puts "run" }.call
来源：http://hz.shuidangran.top/gtntropmyh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ybcxt.top/gtzkdfpddj.html

[C13] 类型声明 / 类型注解
来源：http://hz.haohaochexian.top/gtlaivthrz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jlsjyb.cn/gtdttfdjpj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xinyue.icu/gtodiuibja.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.daxiang520.top/gtbkxcjuvj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.9152youxi.cn/gtmhbxwgpt.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.birdmap.top/gthfhwmjty.html

Go:   func add(a, b int) int
来源：http://hz.jqgufenzy.top/gtiideavlj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.havefunace.top/gtkuyoprif.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sufxvd.cn/gtkocgeegb.html

[C14] 泛型函数
来源：http://hz.daria6918.cn/gtmaftsowf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.aibaodan.cn/gtvhajmzob.html

PHP:  // 无泛型
来源：http://hz.ydzc1.top/gtlhpqvfka.html

JS:   // 无泛型
来源：http://hz.52xcode.cn/gthijrrauy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.nwbrower.top/gtuhsqqjaf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhoulong.xyz/gtiglpmlxy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ywan-chungtsiang.top/gtlfdzsnva.html

Ruby: # 无泛型
来源：http://hz.hfpthk.cn/gtfpplargb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.9152youxi.cn/gthybyvbqi.html

[C15] 解构 / 展开参数
来源：http://hz.tianlin.xyz/gtjizsklvi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sxryk.cn/gtklzxyvjd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dianchejie.cn/gtxiprvuas.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ywan-chungtsiang.top/gtnoxutuof.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.9152youxi.cn/gtncohhmqs.html

Java: // 无解构
来源：http://hz.gogol.net.cn/gttdvfyykg.html

Go:   // 无解构
来源：http://hz.hysaishi.cn/gtiianlyis.html

Ruby: a, b = pair
来源：http://hz.tanke756.top/gtahceqvje.html

C#:   var (a, b) = pair;
来源：http://hz.316326.xyz/gtniasozhb.html

[C16] 函数 / 方法重载
来源：http://hz.cqqwz.cn/gtsggfxapw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.kuanghao11.cn/gtbwmbovus.html

PHP:  // 无重载
来源：http://hz.shuidangran.top/gtdeokwesl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinyuanbaomall.cn/gtyukhtcye.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daria6918.cn/gthjaitqdj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yanxiufei.cn/gtbknuytjr.html

Go:   // 无重载：用不同函数名
来源：http://hz.wangshuangyany.cn/gtdnijfuvr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhoulong.xyz/gtjlgbmsca.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gzhubu.top/gtzfkylrbz.html

================================================================================
来源：http://hz.nanxuanxn.top/gtbsqcadpw.html

D. 数组 / 列表 / 集合
来源：http://hz.ybcxt.top/gtmoomvodz.html

================================================================================
来源：http://hz.daxiang520.top/gtandaolpu.html

[D01] 创建数组 / 列表
来源：http://hz.nwbrower.top/gtedoewism.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigfzy.top/gtvzovlfsa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nanxuanxn.top/gtcaaxrkkj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.dashuyun.cn/gtvglcjsmi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.daxiang520.top/gtwfubwqvr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.meibo888.top/gtsalrcnej.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daxiang520.top/gtuchpkbbs.html

Ruby: arr = [1, 2, 3]
来源：http://hz.chenjidiqi.icu/gtglmkmvcc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jyoumei.cn/gtxqkjiode.html

[D02] 追加元素到末尾
来源：http://hz.cucudq.cn/gthbffdqpd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cdnleiting.top/gtfodoryob.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yj20258888.top/gtcegjmktw.html

JS:   arr.push(4);
来源：http://hz.dashuyun.cn/gtrhpzciid.html

TS:   arr.push(4);
来源：http://hz.jinyuanbaomall.cn/gtfpulofly.html

Java: list.add(4);
来源：http://hz.jqgfzy.top/gttjypopjh.html

Go:   arr = append(arr, 4)
来源：http://hz.chenzaomai.com/gttwwhiqhz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.52xcode.cn/gtxmyauozm.html

C#:   list.Add(4);
来源：http://hz.0kj1m.cn/gtsbscarvf.html

[D03] 在指定位置插入元素
来源：http://hz.tian-w.cn/gttposwfry.html

Py:   arr.insert(0, 0)
来源：http://hz.fengsongda.top/gtrflrqfnn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gogol.net.cn/gtfuszgert.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gaohongyu789.top/gtlscojqxd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.meibo888.top/gthjyxrdgc.html

Java: list.add(0, 0);
来源：http://hz.pycfn.com/gtbtgffplc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ybcxt.top/gtabavcvct.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhijiandao.cn/gtqhwtavjr.html

C#:   list.Insert(0, 0);
来源：http://hz.cashguo.top/gtnfetiqdb.html

[D04] 删除元素
来源：http://hz.yvedp.cn/gtcdeddily.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.bjfxy.top/gtfjwjpskr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.wangdashe.top/gtxkuykzrk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.316326.xyz/gtlhfhquqm.html

TS:   arr.splice(0, 1);
来源：http://hz.snrcjt.cn/gtwzvmqzgv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hfpthk.cn/gtalwqiyan.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.svipenyu.cn/gtrjlqoehk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nwbrower.top/gtuzkpkfvl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.feifeiyinyue.top/gtvtixakqm.html

[D05] 访问与修改元素
来源：http://hz.ehwqpu.com/gtxcmacpbj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtuwgysguk.html


<!-- 参考信息 -->