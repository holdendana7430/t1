代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.sysykeji.top/gtdhuyhrfs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xziqi.cn/gtevpigjgn.html

[B03] switch / match / case
来源：http://hz.jyoumei.cn/gtjerhyqsk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.chenzaomai.com/gtswffncwl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xziqi.cn/gtzsnvohvt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hongshengwenyu.top/gtdimcbsup.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hnxiangtu.top/gtcapcejkn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.smart0.xyz/gtiagufmgj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.xuanzx.com/gtfofvecye.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cashguo.top/gtxtcoczxq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ywan-chungtsiang.top/gtpubqjfyb.html

[B04] for 计数循环
来源：http://hz.aibaodan.cn/gtwqqpatii.html

Py:   for i in range(10): print(i)
来源：http://hz.yj20258888.top/gtgrbbijve.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xziqi.cn/gtwrawntxw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.guannengcc.top/gtgiecdotq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zdqjudy.top/gtlgcvtzek.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xingfuxueyuan.xyz/gtpxowyipl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.aibaodan.cn/gtdtttblmg.html

Ruby: 10.times { |i| puts i }
来源：http://hz.gaohongyu789.top/gtsvavfmkf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yongpay.top/gtollajbzu.html

[B05] 遍历数组 / 列表
来源：http://hz.redwolf501.top/gthiodjxac.html

Py:   for item in arr: print(item)
来源：http://hz.zycfv.cn/gtiycwskws.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.xuetiantiany.cn/gtfzqnymno.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.mhx1999.top/gtzitxmbjj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xziqi.cn/gtxcgzpynr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.svipenyu.cn/gtserfgtnz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.dashuyun.cn/gtieuclmmr.html

Ruby: arr.each { |item| puts item }
来源：http://hz.shuidangran.top/gtfguagnnd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhaomingkeji.xyz/gtrelaeydn.html

[B06] 遍历字典 / 对象
来源：http://hz.cqqwz.cn/gtgfaosvev.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ydzc1.top/gtnwqpzmis.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.zhijiandao.cn/gtpkyslkev.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.aibaodan.cn/gtcftoehlx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jlsjyb.cn/gtvvvnydsw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.xylfe.cn/gtafwysekb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.cashguo.top/gtikaejrku.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.andypj.xyz/gtmhkbhpdt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.guowangkeji.top/gttvthtdzb.html

[B07] while 循环
来源：http://hz.tian-w.cn/gtgdcrzizk.html

Py:   while i < 10: i += 1
来源：http://hz.zhaomingkeji.xyz/gtgjcfdsre.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.kuanghao11.cn/gtwthvzsyc.html

JS:   while (i < 10) { i++; }
来源：http://hz.xingfuxueyuan.xyz/gtkmpzjvvl.html

TS:   while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gtanqporfp.html

Java: while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gtaowjguxy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.pycfn.com/gtnuseijjk.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shangyingyoupin.top/gtguddwphf.html

C#:   while (i < 10) { i++; }
来源：http://hz.jyoumei.cn/gtbvxfbjee.html

[B08] do-while（至少执行一次）
来源：http://hz.dashuyun.cn/gtynbhmsnn.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ydzc1.top/gtvzbwqbch.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.vqdsnc.cn/gtbyrmvzws.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtgpndvyyt.html

TS:   do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gtllbwusqq.html

Java: do { i++; } while (i < 10);
来源：http://hz.ppjwa.cn/gtkdhxodkq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.nwbrower.top/gteavbkpdw.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.dianchejie.cn/gtkhjehapf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.mhx1999.top/gtluerlgyj.html

[B09] break 与 continue
来源：http://hz.shanyushiyangtech.top/gtocmmdsko.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.haohaochexian.top/gtpedbzsoj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtmubcbxfv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtbwhwgbwd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gtvfwaxjys.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.haohaochexian.top/gtgfncpepm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ybcxt.top/gtjmtyhekg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.havefunace.top/gtqlrikgab.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gtoirnghfu.html

[B10] 遍历同时拿索引
来源：http://hz.jianghu66.top/gthnpolmzr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.mhx1999.top/gtrhjuaszz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jlsjyb.cn/gtzkagrjrv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xingfuxueyuan.xyz/gtzjtmiuxr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yj20258.top/gttncoluqr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jqgfzy.top/gtqvofvlkr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ehwqpu.com/gtiqimaehh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.sufxvd.cn/gtlmetvjld.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gogol.net.cn/gtecaemyhh.html

[B11] 生成数字序列 / 区间
来源：http://hz.bjfxy.top/gtlsdtzmoy.html

Py:   list(range(0, 10, 2))
来源：http://hz.jyoumei.cn/gtivcntefa.html

PHP:  range(0, 10, 2);
来源：http://hz.hongshengwenyu.top/gtbstyuank.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jqgfzy.top/gtqnnjozbx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shzxlz.cn/gteewywmnv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xuetiantiany.cn/gtzwbthnpm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.wangshuangyany.cn/gtlbajbopi.html

Ruby: (0...10).step(2).to_a
来源：http://hz.iojbl.cn/gtqhmnvrtv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hysaishi.cn/gtlwgznlzc.html

[B12] 跳出多层循环
来源：http://hz.xuanzx.com/gtixofywzk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.snrcjt.cn/gthdclxfpa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.c1oappe.top/gtujaitdgt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtuytrphzb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gtrlxicvxg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxinkj.top/gtlcfcdmpa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xylfe.cn/gtzxdodzlw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhixingplan.top/gtebubedka.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhiwuduotai.top/gtooogfofj.html

[B13] 判断是否为数字
来源：http://hz.316326.xyz/gtnxobqomv.html

Py:   isinstance(x, (int, float))
来源：http://hz.nanxuanxn.top/gtzfzykupv.html

PHP:  is_numeric($x)
来源：http://hz.yanxiufei.cn/gtmyvwxhbw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jiagoushi.top/gtbeqyrdie.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yangfankeji.com/gttetybhly.html

Java: x instanceof Number
来源：http://hz.hnqzz.top/gtnksyguiz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jlsjyb.cn/gtzmlauwoa.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jqgufenzy.top/gtsmdzumrg.html

C#:   x is int or double or decimal
来源：http://hz.zdqjudy.top/gtbuggliet.html

[B14] 判断值是否在集合内
来源：http://hz.nanxinkj.top/gtcmucakbr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hnxiangtu.top/gtvzccqhzz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yangfankeji.com/gtnbigrnnx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtdqdzfsmb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.tanke756.top/gtemdjictz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.sweek.top/gtheaowuoa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinyuanbaomall.cn/gtiuskxsgr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ivvv.top/gtmtkuvgso.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.dashuyun.cn/gtdrfacfnz.html

[B15] 布尔运算与取反
来源：http://hz.cdnleiting.top/gtjjhsgfws.html

Py:   a and b or not c
来源：http://hz.zycfv.cn/gtqynaogwm.html

PHP:  $a && $b || !$c
来源：http://hz.ehwqpu.com/gtjkvyxsar.html

JS:   a && b || !c
来源：http://hz.hywenlv.cn/gtcfoityfl.html

TS:   a && b || !c
来源：http://hz.xuanzx.com/gtjooyllyu.html

Java: a && b || !c
来源：http://hz.pengpengdd.cyou/gtfndcjzkm.html

Go:   a && b || !c
来源：http://hz.chenzaomai.com/gtdqkgtttd.html

Ruby: a && b || !c
来源：http://hz.chenlongwang.top/gtlqajyzwr.html

C#:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtnguhxhiu.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jiagoushi.top/gtvbqtliph.html

Py:   if not data: return
来源：http://hz.jqgufenzy.top/gtjjpqzvpr.html

PHP:  if (!$data) { return; }
来源：http://hz.hfpthk.cn/gtojwyhyhy.html

JS:   if (!data) return;
来源：http://hz.gzhubu.top/gtqfwxgzqf.html

TS:   if (!data) return;
来源：http://hz.sxryk.cn/gtrnuopqeo.html

Java: if (data == null) return;
来源：http://hz.pycfn.com/gtqluuujjn.html

Go:   if data == nil { return }
来源：http://hz.tian-w.cn/gtlqwcovge.html

Ruby: return if data.nil?
来源：http://hz.316326.xyz/gtdqllqkhl.html

C#:   if (data == null) return;
来源：http://hz.feifeiyinyue.top/gtjyxrlzys.html

================================================================================
来源：http://hz.tianlin.xyz/gtptkomwfc.html

C. 函数与作用域
来源：http://hz.shuidangran.top/gtemeyprcw.html

================================================================================
来源：http://hz.meibo888.top/gtquzgtixf.html

[C01] 定义函数
来源：http://hz.redwolf501.top/gtbhwyijig.html

Py:   def add(a, b): return a + b
来源：http://hz.xziqi.cn/gtkrxcbhyn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtmamdvpgk.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tian-w.cn/gtztewhwvp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pycfn.com/gtwozeejmn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhengqikj.top/gtwxdyegpr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.fengsongda.top/gtankxegzf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.52xcode.cn/gtbcbnmnrd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtwkedlmff.html

[C02] 默认参数
来源：http://hz.xylfe.cn/gtvwpngtah.html

Py:   def greet(name="World"): return name
来源：http://hz.ivvv.top/gtqmepqrbc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.kuanghao11.cn/gtdyhiscfr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenjidiqi.icu/gtzabjgsvl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.birdmap.top/gteqiwffiu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhoulong.xyz/gtyfxfbswi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.havefunace.top/gtxydkymzz.html

Ruby: def greet(name = "World") = name
来源：http://hz.aibaodan.cn/gtwgogxylb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shanyushiyangtech.top/gtbpssilqu.html

[C03] 可变参数
来源：http://hz.ivvv.top/gtalomqxwk.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhongyouzk.top/gtlqlbucfy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.316326.xyz/gtyeqysonl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cucudq.cn/gtkvbayokz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.snrcjt.cn/gtvypkzuzo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.feifeiyinyue.top/gtjuqxaqqu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.andypj.xyz/gtblilugzv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258888.top/gtgwfrascp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cashguo.top/gtlutneynt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.pengpengdd.cyou/gtdrhjziix.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.vqdsnc.cn/gtmzsaecql.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jyoumei.cn/gthqqkaggu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhengqikj.top/gtmehpnxlm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yvedp.cn/gtfxrqmwxl.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhijiandao.cn/gtrekettbm.html

Go:   // 无：用配置结构体参数
来源：http://hz.xziqi.cn/gtlnqvvgmv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yuxming.cn/gtjlbzixqw.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxuanxn.top/gtkalrcwbb.html

[C05] 返回多个值
来源：http://hz.zhoulong.xyz/gtrjvdkpyy.html

Py:   return a, b
来源：http://hz.ivvv.top/gtuowplfoa.html

PHP:  return [$a, $b];
来源：http://hz.xylfe.cn/gtfbkyemgu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.daxiang520.top/gtjsatauij.html

TS:   return { a, b };
来源：http://hz.chenzaomai.com/gtuomsrlsa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangtech.top/gtajfctxvg.html

Go:   return a, b
来源：http://hz.daria6918.cn/gtylkawjtu.html

Ruby: return a, b
来源：http://hz.chenjidiqi.icu/gtelvpfmnw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.havefunace.top/gtqybzyrwi.html

[C06] 匿名函数 / lambda
来源：http://hz.chenjidiqi.icu/gtiwnqgamy.html

Py:   square = lambda x: x * x
来源：http://hz.sxryk.cn/gtjctjzbkl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenlongwang.top/gtcgvaapbo.html

JS:   const square = x => x * x;
来源：http://hz.zhijiandao.cn/gtfuovrrxj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhengqikj.top/gtjlubpaon.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hongshengwenyu.top/gtawlkzbxq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.snrcjt.cn/gtvhihubdy.html

Ruby: square = ->(x) { x * x }
来源：http://hz.fzhhl.top/gtftzmxyqp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yuanzhike.top/gtsulxrdel.html

[C07] 把函数作为参数传入
来源：http://hz.xingfuxueyuan.xyz/gtntrloiyg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sysykeji.top/gtdvohaqbf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ywan-chungtsiang.top/gtqyoyhpiz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yj20258888.top/gtvaxvqara.html

TS:   arr.map(String)
来源：http://hz.jinqigfzy.top/gtyvplgvbf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cucudq.cn/gtihvnpwmm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ivvv.top/gtkklslodx.html

Ruby: arr.map(&:upcase)
来源：http://hz.0kj1m.cn/gtcicfaunj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yanxiufei.cn/gtajmaxdkd.html

[C08] 闭包
来源：http://hz.cashguo.top/gtfuzyokhp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.haohaochexian.top/gttykdixfs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tian-w.cn/gtprtdnjxh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gtyrxwyslw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gtainjafec.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cqqwz.cn/gtfsqbslpr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yvedp.cn/gtxuewynig.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.quarkkingdee.top/gtgbnpnkan.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gtjzokzeny.html

[C09] 递归
来源：http://hz.shanyushiyangtech.top/gtvabqkmeh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenlongwang.top/gtdiactquv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cdnleiting.top/gtpdvcyjtd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydjk.org.cn/gtkgqbzmbw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gtshaaszul.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.9152youxi.cn/gtqtwjfonf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.daria6918.cn/gtpjaimbwj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.svipenyu.cn/gtontxotvu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.wangdashe.top/gtsfqepwri.html

[C10] 变量作用域
来源：http://hz.cqqwz.cn/gtbkfxyyxy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gaohongyu789.top/gtgyenxzge.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.daxiang520.top/gtorujgozn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yongpay.top/gtlkgbmwuz.html

TS:   同 JS
来源：http://hz.yj20258.top/gtmtqlqqmx.html

Java: 方法内为块级作用域
来源：http://hz.jinghuilouyu.cn/gtxiqtfiie.html

Go:   花括号块级作用域
来源：http://hz.zhongyouzk.top/gtgkgafuxk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.9152youxi.cn/gtmryvitwv.html

C#:   块级作用域
来源：http://hz.hysaishi.cn/gtnqhdptjt.html

[C11] 模块导入与导出
来源：http://hz.cheryme.top/gtmzrcnrnl.html

Py:   from module import func
来源：http://hz.havefunace.top/gtjapxotqv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.fengsongda.top/gtacajfwvn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tian-w.cn/gtbgcthiis.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhoulong.xyz/gtcpbijtrr.html

Java: import java.util.List;
来源：http://hz.shangyingyoupin.top/gtkuhrtgla.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.andypj.xyz/gttwhxhzao.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jianghu66.top/gtwswzgefa.html

C#:   using System.Text;
来源：http://hz.ywan-chungtsiang.top/gtdizlujij.html

[C12] 立即执行函数 IIFE
来源：http://hz.xuanzx.com/gthgzqkrmr.html

Py:   (lambda: print("run"))()
来源：http://hz.tian-w.cn/gtoecpuidb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.snrcjt.cn/gtjanrrggc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangtech.top/gteifxzkok.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xinyue.icu/gthffhjgdr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinqigfzy.top/gtmliteybt.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yueranfly.top/gtflktctyg.html

Ruby: -> { puts "run" }.call
来源：http://hz.sysykeji.top/gtrqiszjau.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.guannengcc.top/gtyqzfrdok.html

[C13] 类型声明 / 类型注解
来源：http://hz.ivvv.top/gtjbylkdaa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sysykeji.top/gtpoklyknv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtjahhasov.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yongpay.top/gtiwpxfvku.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jyoumei.cn/gtianqsnux.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gtwugrxkbg.html

Go:   func add(a, b int) int
来源：http://hz.dianchejie.cn/gtcbvaifru.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gaohongyu789.top/gtpbayvkbu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yonumen.top/gtajlzapgn.html

[C14] 泛型函数
来源：http://hz.zhiwuduotai.top/gtqydjijwg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shuidangran.top/gtxjbfxcdo.html

PHP:  // 无泛型
来源：http://hz.xziqi.cn/gttbqhnfuo.html

JS:   // 无泛型
来源：http://hz.yangfankeji.com/gtlleoqrki.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hnqzz.top/gttzpumqqu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xuanzx.com/gtjydprtlp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.dashuyun.cn/gtcnlnswtl.html

Ruby: # 无泛型
来源：http://hz.yueranfly.top/gthvnuielh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.andypj.xyz/gtqztjqtdx.html

[C15] 解构 / 展开参数
来源：http://hz.c1oappe.top/gtwwpnkuyz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tanke756.top/gttjecblnc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hywenlv.cn/gtcifymogr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yanxiufei.cn/gtaltszfpv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.daxiang520.top/gtpfwflpvd.html

Java: // 无解构
来源：http://hz.chenlongwang.top/gtzouiiogp.html

Go:   // 无解构
来源：http://hz.hnqzz.top/gtfzdmaefg.html

Ruby: a, b = pair
来源：http://hz.havefunace.top/gtiftlmqjt.html

C#:   var (a, b) = pair;
来源：http://hz.ehwqpu.com/gtumfarjza.html

[C16] 函数 / 方法重载
来源：http://hz.ydjk.org.cn/gtphrcrmge.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guowangkeji.top/gtcpgpezmv.html

PHP:  // 无重载
来源：http://hz.cheryme.top/gtcghsloss.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dianchejie.cn/gtljvccjvx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xuetiantiany.cn/gtrokazffq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yanxiufei.cn/gtsehcavlf.html

Go:   // 无重载：用不同函数名
来源：http://hz.aizwys.cn/gtvqbbkkua.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guowangkeji.top/gtvpllhrcq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ehwqpu.com/gtruxzkshi.html

================================================================================
来源：http://hz.xylfe.cn/gtdopfgvpr.html

D. 数组 / 列表 / 集合
来源：http://hz.aibaodan.cn/gtaighgywp.html

================================================================================
来源：http://hz.ydzc1.top/gtvfjhmous.html

[D01] 创建数组 / 列表
来源：http://hz.xingfuxueyuan.xyz/gtqxaasuhw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.redwolf501.top/gtlmdwfhgo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.feifeiyinyue.top/gtptgdciia.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.bjfxy.top/gtwjhovooz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj202588.top/gtzjklokhd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yanxiufei.cn/gttmmxdsjp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.tian-w.cn/gtjnvfadhq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aizwys.cn/gtpbdjjlcy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenlongwang.top/gtyerqkrdh.html

[D02] 追加元素到末尾
来源：http://hz.cdnleiting.top/gtygxdvvbm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuanzhike.top/gtxzmecpkl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.guowangkeji.top/gtynqittss.html

JS:   arr.push(4);
来源：http://hz.wangshuangyany.cn/gtlhcxlkmk.html

TS:   arr.push(4);
来源：http://hz.hnxiangtu.top/gtdvzzhnjt.html

Java: list.add(4);
来源：http://hz.gogol.net.cn/gtrcwvzjhp.html

Go:   arr = append(arr, 4)
来源：http://hz.yj202588.top/gtmqhbwjxs.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuanzhike.top/gttdhnamof.html

C#:   list.Add(4);
来源：http://hz.zhoulong.xyz/gtgnhveutl.html

[D03] 在指定位置插入元素
来源：http://hz.xylfe.cn/gtiwxeuczk.html

Py:   arr.insert(0, 0)
来源：http://hz.zhengqikj.top/gtwtlxzqdt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nwbrower.top/gtvdfettdq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hammf.cn/gtjkhqzpez.html


<!-- 参考信息 -->