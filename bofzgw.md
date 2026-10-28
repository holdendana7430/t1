代发 wailian999

[A26] 类型转换总览
来源：http://hz.daria6918.cn/gthwpowopj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.hywenlv.cn/gtengowhkn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.meibo888.top/gtwblupzsh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.316326.xyz/gtntqnhjai.html

TS:   Number() String() Boolean() x as number
来源：http://hz.c1oappe.top/gtlzqzcvsz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.ppjwa.cn/gtlalslmcr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jiagoushi.top/gtfqtkihrg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.316326.xyz/gtomkvdciq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.9152youxi.cn/gtsqzyknyw.html

================================================================================
来源：http://hz.vqdsnc.cn/gtgxtwwdow.html

B. 流程控制
来源：http://hz.ywan-chungtsiang.top/gtcnezdvzb.html

================================================================================
来源：http://hz.xuanzx.com/gtbusrwnpg.html

[B01] 条件判断 if / else
来源：http://hz.hfpthk.cn/gtskeqgaet.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.daria6918.cn/gtyghnblwx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.kuanghao11.cn/gtfznxgupv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangtech.top/gtndqwwuhr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.fzhhl.top/gthvjnnhuk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xuanzx.com/gthxzuchjv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ywan-chungtsiang.top/gtuyfrdgps.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhiwuduotai.top/gtbkseinfw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yongpay.top/gttxpvinqr.html

[B02] 多分支 else if / elif
来源：http://hz.chenzaomai.com/gtfagupwge.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.cqqwz.cn/gtbrkrvlii.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yanxiufei.cn/gtryrwpunh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.feifeiyinyue.top/gtkxtoqhsh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgfzy.top/gtmnouoywa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hywenlv.cn/gtepzlktqx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.52xcode.cn/gtoprgitpn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yj20258.top/gtoxxqymnm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhengqikj.top/gtiqmavjlp.html

[B03] switch / match / case
来源：http://hz.mhx1999.top/gtcfujdcix.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.dianchejie.cn/gtkbzbgcno.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.cqqwz.cn/gtibwoaxfj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinyuanbaomall.cn/gtqukrluxv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sweek.top/gtxmthuuap.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.andypj.xyz/gtwyzhfycz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hnxiangtu.top/gtfcfembhv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.0kj1m.cn/gtvibiifkn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zycfv.cn/gtdarkfwis.html

[B04] for 计数循环
来源：http://hz.0kj1m.cn/gtduoqwhyw.html

Py:   for i in range(10): print(i)
来源：http://hz.chenjidiqi.icu/gteonschfe.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.0kj1m.cn/gtpzyvvijx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hysaishi.cn/gtcdoewwrs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gotoacloud.top/gteocgmuad.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.chenlongwang.top/gtavwizosv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.aizwys.cn/gttkojheat.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhongyouzk.top/gttbefrrng.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yanxiufei.cn/gtywoarfft.html

[B05] 遍历数组 / 列表
来源：http://hz.yj20258.top/gtkxcohlqn.html

Py:   for item in arr: print(item)
来源：http://hz.wangshuangyany.cn/gthfnpnrhw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hammf.cn/gtgghafvfr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xziqi.cn/gteweipbjk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.nwbrower.top/gtqwmofeyz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shanyushiyangkeji.top/gtybpctlbu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ehwqpu.com/gthlxtaoru.html

Ruby: arr.each { |item| puts item }
来源：http://hz.mhx1999.top/gtodckitzr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhengqikj.top/gtutpnncii.html

[B06] 遍历字典 / 对象
来源：http://hz.tanke756.top/gtvrtwmtri.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhixingplan.top/gtzfgphteb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.fzhhl.top/gtbztxddyf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.birdmap.top/gtytrjibkl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.pengpengdd.cyou/gtumvextsx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.aizwys.cn/gttgaccdvj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.kuanghao11.cn/gtofiixaxe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhoulong.xyz/gtswijegyb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jqgfzy.top/gtbxehizbo.html

[B07] while 循环
来源：http://hz.wangshuangyany.cn/gtbyguwosi.html

Py:   while i < 10: i += 1
来源：http://hz.aizwys.cn/gtsgjaecxv.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ppjwa.cn/gtchdaqdyk.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhoulong.xyz/gtlongcwjp.html

TS:   while (i < 10) { i++; }
来源：http://hz.vqdsnc.cn/gttemermbt.html

Java: while (i < 10) { i++; }
来源：http://hz.zhixingplan.top/gtjxsytyop.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.wangdashe.top/gtpvigwwil.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ydzc1.top/gtiarpwdqx.html

C#:   while (i < 10) { i++; }
来源：http://hz.hongshengwenyu.top/gtypyhtptl.html

[B08] do-while（至少执行一次）
来源：http://hz.shuidangran.top/gtqlpfnasj.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.haohaochexian.top/gtnctohnmw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zdqjudy.top/gtwterfsku.html

JS:   do { i++; } while (i < 10);
来源：http://hz.9152youxi.cn/gtcyrdtrnf.html

TS:   do { i++; } while (i < 10);
来源：http://hz.fzhhl.top/gteefeokkc.html

Java: do { i++; } while (i < 10);
来源：http://hz.sysykeji.top/gtsardtlcs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.guannengcc.top/gtslbuqgrl.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hnxiangtu.top/gtjtisltrq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.kuanghao11.cn/gtcytqnsdo.html

[B09] break 与 continue
来源：http://hz.pengpengdd.cyou/gtvfdfxgvj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.snrcjt.cn/gtaxkqstbf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.316326.xyz/gterlyaqkk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtrsxlwcpn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gttvqubmxc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtfodcfdbd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yanxiufei.cn/gtzmvquoix.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hongshengwenyu.top/gthbdtyxnx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtktmbuxfs.html

[B10] 遍历同时拿索引
来源：http://hz.jlsjyb.cn/gtwwndkkmz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gogol.net.cn/gtxaplcwom.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhoulong.xyz/gtjxlcvdgq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.pycfn.com/gthyzpbedp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shuidangran.top/gttrglcuzp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinqigufen.top/gtjudksxas.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.svipenyu.cn/gtlgqdnyeu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tianlin.xyz/gtvzswqxfn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.fzhhl.top/gthcwtjprq.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinqigfzy.top/gtzqsryldp.html

Py:   list(range(0, 10, 2))
来源：http://hz.aizwys.cn/gtumxlgybt.html

PHP:  range(0, 10, 2);
来源：http://hz.zhaomingkeji.xyz/gttqniztvd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gzhubu.top/gttecyzgql.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.c1oappe.top/gtmkirdqlw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.tian-w.cn/gtpudtrlse.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yonumen.top/gtyknuczed.html

Ruby: (0...10).step(2).to_a
来源：http://hz.havefunace.top/gtmecjdjub.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ivvv.top/gtktmjxcou.html

[B12] 跳出多层循环
来源：http://hz.zhoulong.xyz/gtazzliber.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jinyuanbaomall.cn/gtxdpxgmje.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jinyuanbaomall.cn/gtzaxrgmco.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.birdmap.top/gtgcudpnti.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sysykeji.top/gtbjzurfeu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.0kj1m.cn/gtblmmjmor.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.birdmap.top/gttuzcleko.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jlsjyb.cn/gtgqjncuel.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.pycfn.com/gtlgrasooy.html

[B13] 判断是否为数字
来源：http://hz.tanke756.top/gtwcywclxp.html

Py:   isinstance(x, (int, float))
来源：http://hz.dianchejie.cn/gtktcjjlbp.html

PHP:  is_numeric($x)
来源：http://hz.nanxinkj.top/gtejdptzsb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daria6918.cn/gtevgxdtms.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.quarkkingdee.top/gtdmkoyngh.html

Java: x instanceof Number
来源：http://hz.yueranfly.top/gtwgakkuvl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.shangyingyoupin.top/gtdeoixoeu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.quarkkingdee.top/gttyyrxzzf.html

C#:   x is int or double or decimal
来源：http://hz.zhijiandao.cn/gtxubtqjci.html

[B14] 判断值是否在集合内
来源：http://hz.jinyuanbaomall.cn/gtaxncpwkq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhoulong.xyz/gttaxrnzkp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gogol.net.cn/gtwqrntywk.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ivvv.top/gtgkjfwqke.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yueranfly.top/gtvxmtmrgb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tian-w.cn/gtzbjybiqr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.gotoacloud.top/gtbexlmzgq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.mhx1999.top/gtyrfprrwa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenjidiqi.icu/gtlalzarib.html

[B15] 布尔运算与取反
来源：http://hz.bjfxy.top/gthtmmfhfw.html

Py:   a and b or not c
来源：http://hz.hywenlv.cn/gtpvhfohep.html

PHP:  $a && $b || !$c
来源：http://hz.zhixingplan.top/gttbbytfsf.html

JS:   a && b || !c
来源：http://hz.redwolf501.top/gtplppihgw.html

TS:   a && b || !c
来源：http://hz.redwolf501.top/gtubqpuymc.html

Java: a && b || !c
来源：http://hz.quarkkingdee.top/gtxqvcitbi.html

Go:   a && b || !c
来源：http://hz.bjfxy.top/gtkzehbelc.html

Ruby: a && b || !c
来源：http://hz.hywenlv.cn/gtxllooqtg.html

C#:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtmfeivzev.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhongyouzk.top/gtqqlxrqdz.html

Py:   if not data: return
来源：http://hz.zdqjudy.top/gtihtkkqwk.html

PHP:  if (!$data) { return; }
来源：http://hz.jqgufenzy.top/gtuzsbpeye.html

JS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtvpxbkbhz.html

TS:   if (!data) return;
来源：http://hz.fengsongda.top/gtpojqowdi.html

Java: if (data == null) return;
来源：http://hz.jinghuilouyu.cn/gtwefkexli.html

Go:   if data == nil { return }
来源：http://hz.wangshuangyany.cn/gtfuwujqol.html

Ruby: return if data.nil?
来源：http://hz.52xcode.cn/gtpnbiiktg.html

C#:   if (data == null) return;
来源：http://hz.yj202588.top/gtwbfzpwxq.html

================================================================================
来源：http://hz.cashguo.top/gtcglznhal.html

C. 函数与作用域
来源：http://hz.sxryk.cn/gtxsuzxifp.html

================================================================================
来源：http://hz.yvedp.cn/gtjnqpwway.html

[C01] 定义函数
来源：http://hz.shangyingyoupin.top/gtpmacynoa.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxinkj.top/gtjqvuvfrj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenzaomai.com/gtxubeoatw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.sufxvd.cn/gtafutklcd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gtibngadav.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtvdtasctl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gzhubu.top/gtpqyczauq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.316326.xyz/gtswkjsbjd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gtepbgljzk.html

[C02] 默认参数
来源：http://hz.xylfe.cn/gtlxkqhzhk.html

Py:   def greet(name="World"): return name
来源：http://hz.meibo888.top/gtrjbnquzp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nanxinkj.top/gtxvddzxsb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydjk.org.cn/gtifqdfzgm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jyoumei.cn/gtznomrhdk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jianghu66.top/gtukfctukl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yongpay.top/gtqsqpglyl.html

Ruby: def greet(name = "World") = name
来源：http://hz.xziqi.cn/gtsscduqcc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj202588.top/gtecwsnsca.html

[C03] 可变参数
来源：http://hz.xylfe.cn/gtcdrlbilv.html

Py:   def total(*args): return sum(args)
来源：http://hz.andypj.xyz/gtvhwotcba.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhixingplan.top/gtnyhjawib.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tanke756.top/gtcrlsvzey.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangshuangyany.cn/gtynpqbcpx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.bjfxy.top/gtpqueulrl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhoulong.xyz/gtuucbouiu.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yongpay.top/gtgropgfut.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.feifeiyinyue.top/gtxbcowbku.html

[C04] 命名参数 / 关键字参数
来源：http://hz.andypj.xyz/gtwnwpuetg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zycfv.cn/gtmtdbhcwp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tian-w.cn/gtopxhfmvm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nanxinkj.top/gtfakeuhoy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.daxiang520.top/gthirozkoo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xinyue.icu/gtcooftafj.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinqigufen.top/gtvucmevyt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ivvv.top/gtqeruvoup.html

C#:   f(a: 1, b: 2)
来源：http://hz.ydzc1.top/gtqwbgntat.html

[C05] 返回多个值
来源：http://hz.jqgfzy.top/gtobduxqht.html

Py:   return a, b
来源：http://hz.pycfn.com/gtzwthbfdl.html

PHP:  return [$a, $b];
来源：http://hz.ydzc1.top/gtokuqzylg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinqigufen.top/gtitajunsf.html

TS:   return { a, b };
来源：http://hz.yongpay.top/gtqesmrucl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj20258.top/gtlekkttcd.html

Go:   return a, b
来源：http://hz.iojbl.cn/gtbxeinvsj.html

Ruby: return a, b
来源：http://hz.xuetiantiany.cn/gtctmtfhix.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pengpengdd.cyou/gtnagkimjx.html

[C06] 匿名函数 / lambda
来源：http://hz.hfpthk.cn/gtrmwmozdc.html

Py:   square = lambda x: x * x
来源：http://hz.tianlin.xyz/gtufputhnv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yuxming.cn/gtkdvgbfsn.html

JS:   const square = x => x * x;
来源：http://hz.shuidangran.top/gtdsgnuecv.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ybcxt.top/gtdpavgelj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.dashuyun.cn/gtjhhpxbpu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jqgfzy.top/gtpyuxzbod.html

Ruby: square = ->(x) { x * x }
来源：http://hz.sxryk.cn/gtktbxvpdx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.iojbl.cn/gttnhnjosn.html

[C07] 把函数作为参数传入
来源：http://hz.dashuyun.cn/gtvzkkfvrw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.fzhhl.top/gtlthwtudw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ydjk.org.cn/gtckntmnvy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dianchejie.cn/gtpkrbpmmu.html

TS:   arr.map(String)
来源：http://hz.hnxiangtu.top/gthnpczytv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hysaishi.cn/gtbfcwmjdz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj20258.top/gtcfsjqygo.html

Ruby: arr.map(&:upcase)
来源：http://hz.sxryk.cn/gtswxymagm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.chenjidiqi.icu/gtumhbgyxf.html

[C08] 闭包
来源：http://hz.bjfxy.top/gtcxqaqadj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jianghu66.top/gtntjfshos.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ywan-chungtsiang.top/gtwcaqqtvg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtsxqkncjb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtgbriluvm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ybcxt.top/gtoftfcwje.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sysykeji.top/gtcvcowpzf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhoulong.xyz/gtnohdhdxg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258888.top/gtfjcbuida.html

[C09] 递归
来源：http://hz.quarkkingdee.top/gtmbvpqdux.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhoulong.xyz/gtjltzoclh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cdnleiting.top/gtvnbizarv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gogol.net.cn/gtphpudbfi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgfzy.top/gteezwtyji.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.nanxinkj.top/gtiwqfpudo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xingfuxueyuan.xyz/gtfychqcvq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.wangdashe.top/gtiveurvux.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.birdmap.top/gtnttumbed.html

[C10] 变量作用域
来源：http://hz.jinqigfzy.top/gtcchllsit.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shzxlz.cn/gtenqimdla.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tian-w.cn/gtuxewvdjr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gaohongyu789.top/gtgekkzmqd.html

TS:   同 JS
来源：http://hz.zhaomingkeji.xyz/gtqbwpapwi.html

Java: 方法内为块级作用域
来源：http://hz.cucudq.cn/gtvlpvgrhs.html

Go:   花括号块级作用域
来源：http://hz.jyoumei.cn/gtxvbcbhtg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nanxuanxn.top/gtaqexjiir.html

C#:   块级作用域
来源：http://hz.ydjk.org.cn/gtshstoitk.html

[C11] 模块导入与导出
来源：http://hz.ybcxt.top/gtdktfhamt.html

Py:   from module import func
来源：http://hz.zhengqikj.top/gtikvbpthp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.quarkkingdee.top/gtlosmyhlk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.quarkkingdee.top/gtkemimsdr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sysykeji.top/gtygdhcjbr.html

Java: import java.util.List;
来源：http://hz.chenzaomai.com/gtpfhxivux.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hysaishi.cn/gtegdmhfsp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.quarkkingdee.top/gtskjgpkzr.html

C#:   using System.Text;
来源：http://hz.sxryk.cn/gtdbppqkrx.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenzaomai.com/gtyzgkvaur.html

Py:   (lambda: print("run"))()
来源：http://hz.kuanghao11.cn/gtsbhqpbzs.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jiagoushi.top/gtalntpmow.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhijiandao.cn/gtzljzmtdw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtxyudnphu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sweek.top/gtaupcdcmo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ivvv.top/gtfzxuqwda.html

Ruby: -> { puts "run" }.call
来源：http://hz.pengpengdd.cyou/gtwtlvloqy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuxming.cn/gtoczwuxgm.html

[C13] 类型声明 / 类型注解
来源：http://hz.hywenlv.cn/gtequebiki.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hongshengwenyu.top/gtohlcagjc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigfzy.top/gtrxvqqumn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuxming.cn/gtgylxytwz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnqzz.top/gtphqytbfd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtwglfsjqo.html

Go:   func add(a, b int) int
来源：http://hz.nanxinkj.top/gtykefqwwo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fzhhl.top/gtbojnzocp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jiagoushi.top/gtpizqqmfl.html

[C14] 泛型函数
来源：http://hz.jinyuanbaomall.cn/gtzqhgdpcs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.316326.xyz/gtrwyktycn.html

PHP:  // 无泛型
来源：http://hz.52xcode.cn/gtsadoxaqi.html

JS:   // 无泛型
来源：http://hz.jinghuilouyu.cn/gtiydcblzw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xingfuxueyuan.xyz/gtrjjdyosc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhiwuduotai.top/gtvvfqcofp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shuidangran.top/gtcncbokce.html

Ruby: # 无泛型
来源：http://hz.tianlin.xyz/gtnklhvlnq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.haohaochexian.top/gtngzbsolb.html

[C15] 解构 / 展开参数
来源：http://hz.nwbrower.top/gthyrdxcjy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ybcxt.top/gtwbiybapz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tianlin.xyz/gtlstuouga.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daxiang520.top/gtfiuszdcm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.quarkkingdee.top/gtvfqwwyjd.html

Java: // 无解构
来源：http://hz.tianlin.xyz/gtbtvitjle.html

Go:   // 无解构
来源：http://hz.gaohongyu789.top/gtnuyonayh.html

Ruby: a, b = pair
来源：http://hz.jlsjyb.cn/gtvjkkrzfh.html

C#:   var (a, b) = pair;
来源：http://hz.9152youxi.cn/gtiikwyenz.html

[C16] 函数 / 方法重载
来源：http://hz.tanke756.top/gtzpixwygr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hongshengwenyu.top/gtptodvple.html

PHP:  // 无重载
来源：http://hz.yj202588.top/gtcqdiedzz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ivvv.top/gtmanhmrvc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gaohongyu789.top/gtmwyrulau.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinyuanbaomall.cn/gtguxysdxp.html


<!-- 参考信息 -->