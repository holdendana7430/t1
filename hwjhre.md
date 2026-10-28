代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.chenlongwang.top/gtluloseym.html

[B02] 多分支 else if / elif
来源：http://hz.snrcjt.cn/gtwnxwmujm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhaomingkeji.xyz/gtnnxtvjjl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.dianchejie.cn/gtgrcojbwy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhaomingkeji.xyz/gtycsygfgo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgufenzy.top/gtkubqccjm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydjk.org.cn/gtihetnumf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.tianlin.xyz/gtdjorhcte.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.pycfn.com/gtxtfxdxmu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sxryk.cn/gtkdyntdpl.html

[B03] switch / match / case
来源：http://hz.cheryme.top/gtqqhbohlt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.cheryme.top/gtpmlniuuq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jinghuilouyu.cn/gtqjnrwzka.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.shuidangran.top/gtqvqcezou.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sweek.top/gtqknfikfu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.wangshuangyany.cn/gtzncaflyr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhijiandao.cn/gtynhjwzhq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.shanyushiyangkeji.top/gtgtmvjwlc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.nwbrower.top/gtwrmcymsp.html

[B04] for 计数循环
来源：http://hz.aizwys.cn/gtnzsljumm.html

Py:   for i in range(10): print(i)
来源：http://hz.yueranfly.top/gtmvphcaib.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jinqigufen.top/gtmchjjsoc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.9152youxi.cn/gtgmedwbva.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ivvv.top/gtabgmnscg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.shanyushiyangkeji.top/gtalnmxych.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.daxiang520.top/gtvmerzacm.html

Ruby: 10.times { |i| puts i }
来源：http://hz.daxiang520.top/gtezyqzufj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yj202588.top/gtvjomqibq.html

[B05] 遍历数组 / 列表
来源：http://hz.feifeiyinyue.top/gtdihbqnto.html

Py:   for item in arr: print(item)
来源：http://hz.xuetiantiany.cn/gthorxestz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.birdmap.top/gtxvzkgmvn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.9152youxi.cn/gtbhjhcsfg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jiagoushi.top/gtrvmxmkan.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yj20258888.top/gthcxqaoho.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.gzhubu.top/gtxqnonent.html

Ruby: arr.each { |item| puts item }
来源：http://hz.cashguo.top/gtdptscgee.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yueranfly.top/gtxsrdscyu.html

[B06] 遍历字典 / 对象
来源：http://hz.xingfuxueyuan.xyz/gtczimfnne.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ybcxt.top/gtzbdbezuw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ybcxt.top/gtgvickgzj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gaohongyu789.top/gtmnvrentj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cashguo.top/gtrucaijjp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yonumen.top/gtttqjwflw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.fzhhl.top/gtnzyhoctb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.shangyingyoupin.top/gtqutcuhqg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zhijiandao.cn/gttpppgzhx.html

[B07] while 循环
来源：http://hz.daria6918.cn/gtfkxahwgn.html

Py:   while i < 10: i += 1
来源：http://hz.jinqigufen.top/gthgqsiimm.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.gzhubu.top/gtsssytolt.html

JS:   while (i < 10) { i++; }
来源：http://hz.yangfankeji.com/gtzbectpda.html

TS:   while (i < 10) { i++; }
来源：http://hz.jqgfzy.top/gtbaeahsco.html

Java: while (i < 10) { i++; }
来源：http://hz.jyoumei.cn/gttpfkzltm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.fzhhl.top/gtolhzovbv.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shuidangran.top/gtsjtypknn.html

C#:   while (i < 10) { i++; }
来源：http://hz.yj20258888.top/gtuljsrmsv.html

[B08] do-while（至少执行一次）
来源：http://hz.chenjidiqi.icu/gtochmlxcj.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhoulong.xyz/gtkvsiqkup.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhijiandao.cn/gtogivswwv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gteowatytj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtpagmeafh.html

Java: do { i++; } while (i < 10);
来源：http://hz.pycfn.com/gtldgqkutm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.feifeiyinyue.top/gtqdpcmulm.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.shzxlz.cn/gtzibggbwo.html

C#:   do { i++; } while (i < 10);
来源：http://hz.gaohongyu789.top/gtcafdcisy.html

[B09] break 与 continue
来源：http://hz.sysykeji.top/gtqgpskuoq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xingfuxueyuan.xyz/gtwxzbkdas.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhengqikj.top/gtopbbdkwk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtlbvlrwhk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gtgktsnkiq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtxjravkdk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.shanyushiyangtech.top/gtdbdypfvo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.dashuyun.cn/gtgqoujybi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtgxxoiauh.html

[B10] 遍历同时拿索引
来源：http://hz.havefunace.top/gthmsyspjs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yuanzhike.top/gtipvfyame.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.chenzaomai.com/gtkhiqragv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yangfankeji.com/gthwryaqbg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.redwolf501.top/gtpjvigvez.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.sxryk.cn/gtsskqdpnj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yangfankeji.com/gtelwzuhad.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shanyushiyangtech.top/gtcgbadmet.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.xylfe.cn/gtlzyibmqb.html

[B11] 生成数字序列 / 区间
来源：http://hz.nwbrower.top/gtxwtvwlea.html

Py:   list(range(0, 10, 2))
来源：http://hz.ppjwa.cn/gtbbdiwxhu.html

PHP:  range(0, 10, 2);
来源：http://hz.pengpengdd.cyou/gtwoqwkjcp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ybcxt.top/gtiqlphxjq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fzhhl.top/gtwltamlrx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.wangdashe.top/gtqkjoeykd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hnqzz.top/gtlhzjvgyb.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sysykeji.top/gtqlwgtsgt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zycfv.cn/gtkiqhnjpu.html

[B12] 跳出多层循环
来源：http://hz.tanke756.top/gtgflidwsh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jqgfzy.top/gtahvubnyf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.nanxinkj.top/gtagflcfhu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sysykeji.top/gtpqqrsfzf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gtbpyfnrsk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.birdmap.top/gtsfxhirvo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.quarkkingdee.top/gtbbngkoad.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gogol.net.cn/gtcoymykrs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yongpay.top/gtadgfqfbm.html

[B13] 判断是否为数字
来源：http://hz.sweek.top/gthkflpddy.html

Py:   isinstance(x, (int, float))
来源：http://hz.xziqi.cn/gtjmltnqil.html

PHP:  is_numeric($x)
来源：http://hz.yvedp.cn/gtrtxijvqp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jyoumei.cn/gtizkknjaq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtdvgbikvd.html

Java: x instanceof Number
来源：http://hz.meibo888.top/gthnietoiy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.kuanghao11.cn/gtmycqttsk.html

Ruby: x.is_a?(Numeric)
来源：http://hz.c1oappe.top/gtqskmlubw.html

C#:   x is int or double or decimal
来源：http://hz.sweek.top/gtbgebsjep.html

[B14] 判断值是否在集合内
来源：http://hz.shanyushiyangkeji.top/gttzhydlkw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ydjk.org.cn/gtpxtuzwes.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yonumen.top/gtdvbzxlxp.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gzhubu.top/gtwvfmlzkw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.quarkkingdee.top/gtclawbzep.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jlsjyb.cn/gtsexzkaqs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.birdmap.top/gtixnakxeh.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shanyushiyangtech.top/gtndarkrjt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cqqwz.cn/gtxkjtzged.html

[B15] 布尔运算与取反
来源：http://hz.shanyushiyangkeji.top/gtmwqsfckj.html

Py:   a and b or not c
来源：http://hz.yj202588.top/gtaceizjpt.html

PHP:  $a && $b || !$c
来源：http://hz.tanke756.top/gtmdmqzvwz.html

JS:   a && b || !c
来源：http://hz.xylfe.cn/gthhgeowkp.html

TS:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtalmxxbls.html

Java: a && b || !c
来源：http://hz.chenlongwang.top/gtixsnszcy.html

Go:   a && b || !c
来源：http://hz.xuanzx.com/gtyysnmzxa.html

Ruby: a && b || !c
来源：http://hz.fzhhl.top/gtdyxcodgl.html

C#:   a && b || !c
来源：http://hz.guannengcc.top/gtvgybdtbt.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ydjk.org.cn/gtfuvmgnea.html

Py:   if not data: return
来源：http://hz.xinyue.icu/gtdwwhtekn.html

PHP:  if (!$data) { return; }
来源：http://hz.0kj1m.cn/gtojucrupy.html

JS:   if (!data) return;
来源：http://hz.xuanzx.com/gtnkfchhlj.html

TS:   if (!data) return;
来源：http://hz.chenlongwang.top/gtirmbcxbl.html

Java: if (data == null) return;
来源：http://hz.sysykeji.top/gtcmthcbvx.html

Go:   if data == nil { return }
来源：http://hz.yangfankeji.com/gtxllmsnic.html

Ruby: return if data.nil?
来源：http://hz.birdmap.top/gtsxwithtl.html

C#:   if (data == null) return;
来源：http://hz.yueranfly.top/gtrmelyfzc.html

================================================================================
来源：http://hz.yanxiufei.cn/gtgkwxunks.html

C. 函数与作用域
来源：http://hz.kuanghao11.cn/gtblznnnsy.html

================================================================================
来源：http://hz.hammf.cn/gttlakisif.html

[C01] 定义函数
来源：http://hz.sxryk.cn/gtnzitjdxy.html

Py:   def add(a, b): return a + b
来源：http://hz.haohaochexian.top/gtinafejqr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgfzy.top/gttczdaqoo.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tian-w.cn/gttajizflm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tian-w.cn/gtiodxarhq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtmtkfiasv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.dianchejie.cn/gtggfdhnxr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hongshengwenyu.top/gtczfjrocc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtjpgunqxr.html

[C02] 默认参数
来源：http://hz.guannengcc.top/gtyfeuixzi.html

Py:   def greet(name="World"): return name
来源：http://hz.fengsongda.top/gtkydkxrpc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hammf.cn/gtanmrlqou.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zdqjudy.top/gtndoddexp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.chenlongwang.top/gtxefskrrs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhijiandao.cn/gtuqaurojr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.kuanghao11.cn/gthuhtzsye.html

Ruby: def greet(name = "World") = name
来源：http://hz.pengpengdd.cyou/gtwjzwekfa.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ywan-chungtsiang.top/gtlitpkptf.html

[C03] 可变参数
来源：http://hz.zycfv.cn/gtvxigwtgh.html

Py:   def total(*args): return sum(args)
来源：http://hz.smart0.xyz/gtlxwwwrfq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dashuyun.cn/gtqmhaqhso.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.svipenyu.cn/gttecxbaxf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtknvutpxi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.iojbl.cn/gtoigsliui.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jianghu66.top/gtaonkfeed.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhaomingkeji.xyz/gtcojcoade.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.316326.xyz/gttasckbrw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hammf.cn/gtrgyemxsy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj202588.top/gtenbgwtja.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tianlin.xyz/gtarchpsel.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.haohaochexian.top/gtewnhjbjl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shzxlz.cn/gtjsseswhw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sysykeji.top/gtdiwwtuka.html

Go:   // 无：用配置结构体参数
来源：http://hz.hfpthk.cn/gtdkzdrvkr.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gzhubu.top/gtvbtlgzic.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gthfxkufbz.html

[C05] 返回多个值
来源：http://hz.redwolf501.top/gtncibrzko.html

Py:   return a, b
来源：http://hz.fengsongda.top/gtawzlesex.html

PHP:  return [$a, $b];
来源：http://hz.zhijiandao.cn/gtbkitrahy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sxryk.cn/gtlyyoifsq.html

TS:   return { a, b };
来源：http://hz.cashguo.top/gtqqkfbskk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.bjfxy.top/gtuctjlqkd.html

Go:   return a, b
来源：http://hz.daxiang520.top/gtudsmgjpc.html

Ruby: return a, b
来源：http://hz.ydjk.org.cn/gtqikdkhcu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ppjwa.cn/gttgrryifm.html

[C06] 匿名函数 / lambda
来源：http://hz.zhongyouzk.top/gttjqhoyik.html

Py:   square = lambda x: x * x
来源：http://hz.ywan-chungtsiang.top/gtostscfmo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenjidiqi.icu/gtissqeqym.html

JS:   const square = x => x * x;
来源：http://hz.guannengcc.top/gtpsbitijj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinghuilouyu.cn/gtrmviygqx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hfpthk.cn/gtbpljbjvb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.0kj1m.cn/gtwblkbihz.html

Ruby: square = ->(x) { x * x }
来源：http://hz.snrcjt.cn/gtupriripz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yuanzhike.top/gtkskgogtz.html

[C07] 把函数作为参数传入
来源：http://hz.ivvv.top/gtsgmsqkwo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nanxuanxn.top/gtqojrlrpu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nanxuanxn.top/gtjdowhupe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.svipenyu.cn/gtwtzejwzs.html

TS:   arr.map(String)
来源：http://hz.snrcjt.cn/gtchpwhonu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ydzc1.top/gturctbkom.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ehwqpu.com/gtrphgvway.html

Ruby: arr.map(&:upcase)
来源：http://hz.0kj1m.cn/gtseyrxyar.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj20258.top/gtlzkeopsi.html

[C08] 闭包
来源：http://hz.tianlin.xyz/gttukfsaus.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hywenlv.cn/gtgashqgfj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zdqjudy.top/gtthxudjji.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtguphhadc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtcdzdcgpa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nanxuanxn.top/gtbfqgkgeo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ywan-chungtsiang.top/gtvngtrbxz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.9152youxi.cn/gtwoxailhj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtmgmkbgbl.html

[C09] 递归
来源：http://hz.jqgfzy.top/gtchplfhrm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gtxlrsiqhn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhaomingkeji.xyz/gtbvhfetaf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hongshengwenyu.top/gtdsvnzcic.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258888.top/gtfifrksvp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258.top/gtgcmrcouu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xylfe.cn/gthxiambdo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.0kj1m.cn/gtxjvonbef.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cqqwz.cn/gttctazafp.html

[C10] 变量作用域
来源：http://hz.chenlongwang.top/gtdrlrdpnw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yanxiufei.cn/gtprxxjzsh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jlsjyb.cn/gtiyidhuug.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xuetiantiany.cn/gtmsictscn.html

TS:   同 JS
来源：http://hz.jiagoushi.top/gtggmiewzi.html

Java: 方法内为块级作用域
来源：http://hz.jinyuanbaomall.cn/gtfpehjbsu.html

Go:   花括号块级作用域
来源：http://hz.tanke756.top/gtqwavxbyr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yueranfly.top/gtopxjiour.html

C#:   块级作用域
来源：http://hz.zhoulong.xyz/gttyvhxuvd.html

[C11] 模块导入与导出
来源：http://hz.xuanzx.com/gtunydkgzg.html

Py:   from module import func
来源：http://hz.hammf.cn/gtpurwhxvp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ivvv.top/gtvuqglqpc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhijiandao.cn/gtreualucv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhoulong.xyz/gtqzjgteco.html

Java: import java.util.List;
来源：http://hz.xingfuxueyuan.xyz/gtaizpykkr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhongyouzk.top/gtidjocddm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258.top/gtprtpxkoi.html

C#:   using System.Text;
来源：http://hz.svipenyu.cn/gtqnafdlja.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhixingplan.top/gtoiplgnos.html

Py:   (lambda: print("run"))()
来源：http://hz.quarkkingdee.top/gtvtuzaonr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj20258888.top/gtlyhymeyl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtkflioibz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.c1oappe.top/gthsuhqgrh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jianghu66.top/gtnrrgslwn.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhixingplan.top/gtqqmrtsot.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinyuanbaomall.cn/gtwvoqezog.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.52xcode.cn/gtoqcspzpi.html

[C13] 类型声明 / 类型注解
来源：http://hz.0kj1m.cn/gtghtzsvar.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aibaodan.cn/gtlwwnfuee.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.quarkkingdee.top/gtmdkzcwly.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.0kj1m.cn/gtexzhgmzy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuanzhike.top/gtjyjyeeqf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtqugqnwec.html

Go:   func add(a, b int) int
来源：http://hz.gogol.net.cn/gtwqbaowwc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jqgfzy.top/gthluxibgm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yonumen.top/gtekcptrzt.html

[C14] 泛型函数
来源：http://hz.52xcode.cn/gtiplfiwkf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gaohongyu789.top/gtyovjcmvf.html

PHP:  // 无泛型
来源：http://hz.fzhhl.top/gtacomjxsn.html

JS:   // 无泛型
来源：http://hz.aizwys.cn/gtxxkdyiol.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.fzhhl.top/gtahiyiskq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zycfv.cn/gtfzbqbrid.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhaomingkeji.xyz/gtdptkrhpz.html

Ruby: # 无泛型
来源：http://hz.shuidangran.top/gtrbgrrufh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jiagoushi.top/gtjwmlxjle.html

[C15] 解构 / 展开参数
来源：http://hz.daria6918.cn/gtiofxsums.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yongpay.top/gthdvtfqth.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hfpthk.cn/gtiosmbihs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jlsjyb.cn/gtpkurvnkt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gzhubu.top/gtqgtdifgi.html

Java: // 无解构
来源：http://hz.ybcxt.top/gtwietbxdc.html

Go:   // 无解构
来源：http://hz.jinyuanbaomall.cn/gtnsriqxkj.html

Ruby: a, b = pair
来源：http://hz.wangshuangyany.cn/gtbvkenhwc.html

C#:   var (a, b) = pair;
来源：http://hz.xinyue.icu/gtgguktdoj.html

[C16] 函数 / 方法重载
来源：http://hz.shzxlz.cn/gtuhmjtsyw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinyuanbaomall.cn/gtlqdbktkk.html

PHP:  // 无重载
来源：http://hz.yuxming.cn/gtwbqxolau.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xziqi.cn/gtpkdglyts.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.havefunace.top/gtuskvkfgc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.9152youxi.cn/gttgxknbhn.html

Go:   // 无重载：用不同函数名
来源：http://hz.yvedp.cn/gtxruvkqlh.html

Ruby: # 无重载：靠动态参数
来源：http://hz.chenzaomai.com/gtoufeztol.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xuetiantiany.cn/gthxutddkg.html

================================================================================
来源：http://hz.chenlongwang.top/gtuqbghpti.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258.top/gthkxsimdh.html

================================================================================
来源：http://hz.aibaodan.cn/gtlqpbzjuu.html

[D01] 创建数组 / 列表
来源：http://hz.cheryme.top/gtwvweonnt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.nanxuanxn.top/gtachnnjch.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhixingplan.top/gtfmobkqby.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cheryme.top/gtisthzqsy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.pycfn.com/gtdjfksicn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sufxvd.cn/gtwcklqbpt.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pycfn.com/gtgbaxbdio.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangshuangyany.cn/gtmbnzotmc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.c1oappe.top/gttzysibap.html

[D02] 追加元素到末尾
来源：http://hz.zhaomingkeji.xyz/gtoerkwzmn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ivvv.top/gtfeescxnm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yuanzhike.top/gtcnvyxjsc.html

JS:   arr.push(4);
来源：http://hz.smart0.xyz/gtsbrauaff.html

TS:   arr.push(4);
来源：http://hz.jinghuilouyu.cn/gtflnwwpli.html


<!-- 参考信息 -->