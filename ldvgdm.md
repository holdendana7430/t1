代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.hammf.cn/gtrhawgvbj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtqgwhduqk.html

[B03] switch / match / case
来源：http://hz.hammf.cn/gtjwskgyta.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hfpthk.cn/gtqarlsfob.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.nanxinkj.top/gtteiimebb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.snrcjt.cn/gtzzgmutpk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ybcxt.top/gtjnibatmb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yj202588.top/gtfdjbrxbk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yuanzhike.top/gtckdabwps.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.andypj.xyz/gtzppcmwzy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jinqigufen.top/gtpgqhipik.html

[B04] for 计数循环
来源：http://hz.bjfxy.top/gtbxtmtdsy.html

Py:   for i in range(10): print(i)
来源：http://hz.zhongyouzk.top/gtzflfyqna.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.316326.xyz/gtqbqlmrnr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xziqi.cn/gtpuvjwafa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.fengsongda.top/gtxicmfyuw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.tian-w.cn/gtgryxrvyh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.gotoacloud.top/gtzohpmdrv.html

Ruby: 10.times { |i| puts i }
来源：http://hz.hongshengwenyu.top/gtunluxvrr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhijiandao.cn/gtnnwtnjiv.html

[B05] 遍历数组 / 列表
来源：http://hz.vqdsnc.cn/gtoppqesjg.html

Py:   for item in arr: print(item)
来源：http://hz.xinyue.icu/gtmqruaoww.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.cqqwz.cn/gtobsxzhhv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jqgfzy.top/gtzzgveeqt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.daxiang520.top/gtcvoceopu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.ywan-chungtsiang.top/gtbduoxyzi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.c1oappe.top/gtxoxvbzyy.html

Ruby: arr.each { |item| puts item }
来源：http://hz.quarkkingdee.top/gtodpqlexf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhengqikj.top/gtafphaxnd.html

[B06] 遍历字典 / 对象
来源：http://hz.shuidangran.top/gtaemobrlz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.shanyushiyangkeji.top/gtmioqjnwu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.aibaodan.cn/gtsvplxede.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.c1oappe.top/gtvuozawsi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhoulong.xyz/gtsxldqbyn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.kuanghao11.cn/gtgigawygp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.sxryk.cn/gtzavzjfmg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yj20258.top/gtxzzqntlg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hfpthk.cn/gtuveohaeq.html

[B07] while 循环
来源：http://hz.xziqi.cn/gtmkudupqh.html

Py:   while i < 10: i += 1
来源：http://hz.gaohongyu789.top/gtmgieaxtk.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yj202588.top/gteaouquhf.html

JS:   while (i < 10) { i++; }
来源：http://hz.c1oappe.top/gtggooqioq.html

TS:   while (i < 10) { i++; }
来源：http://hz.yongpay.top/gtzhndkxyf.html

Java: while (i < 10) { i++; }
来源：http://hz.jqgfzy.top/gtppbmqbmd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hongshengwenyu.top/gtzyhwontf.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shangyingyoupin.top/gtrttxtivc.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhixingplan.top/gtojepxuof.html

[B08] do-while（至少执行一次）
来源：http://hz.jqgufenzy.top/gtmnfexekm.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.fzhhl.top/gtbpycrdrv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yangfankeji.com/gttviwkddq.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gtoascdsan.html

TS:   do { i++; } while (i < 10);
来源：http://hz.vqdsnc.cn/gtxsjsmzqr.html

Java: do { i++; } while (i < 10);
来源：http://hz.hysaishi.cn/gtvogfgmxo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jianghu66.top/gtpftprwzf.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xylfe.cn/gtufbwfcll.html

C#:   do { i++; } while (i < 10);
来源：http://hz.birdmap.top/gtzgnncrcb.html

[B09] break 与 continue
来源：http://hz.zycfv.cn/gttxtxplmw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yuxming.cn/gthmueiipf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhixingplan.top/gtuenkdeoj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.iojbl.cn/gtjktxxvxw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuxming.cn/gtibcsgliy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtyumbdiph.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.cucudq.cn/gtqmhtbpnk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.birdmap.top/gtahkixytb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.c1oappe.top/gtrdlcyqcd.html

[B10] 遍历同时拿索引
来源：http://hz.wangshuangyany.cn/gthaxyrdua.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.daria6918.cn/gtpttzrkml.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cucudq.cn/gtncgioxfs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yangfankeji.com/gtgwlmmcrb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ppjwa.cn/gtqqoppvak.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.52xcode.cn/gtcayhjjfa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cqqwz.cn/gthxaujovy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jqgfzy.top/gtzuesoxot.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ywan-chungtsiang.top/gtawchxcyx.html

[B11] 生成数字序列 / 区间
来源：http://hz.hnqzz.top/gtpsnfquta.html

Py:   list(range(0, 10, 2))
来源：http://hz.ydzc1.top/gttnawngmf.html

PHP:  range(0, 10, 2);
来源：http://hz.xinyue.icu/gtshlueyep.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenzaomai.com/gthxbpviyw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gogol.net.cn/gtoamxlluk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yvedp.cn/gteorstlpj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.sysykeji.top/gtdbfwxkjv.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hfpthk.cn/gtwurfmozm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zycfv.cn/gtbiecigzu.html

[B12] 跳出多层循环
来源：http://hz.tanke756.top/gtttxcosvm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhengqikj.top/gtdlkbsaqx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yongpay.top/gtsgdgighp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yvedp.cn/gtgpxdoejz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sysykeji.top/gtmrvebejy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenjidiqi.icu/gtqjireacw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhoulong.xyz/gtxkrdvbtt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jqgfzy.top/gtxealpjmx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xingfuxueyuan.xyz/gttlitihjn.html

[B13] 判断是否为数字
来源：http://hz.xuanzx.com/gtzstlpmhc.html

Py:   isinstance(x, (int, float))
来源：http://hz.jlsjyb.cn/gtsybjaziv.html

PHP:  is_numeric($x)
来源：http://hz.quarkkingdee.top/gtgyuofnke.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gogol.net.cn/gttambpaaa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.feifeiyinyue.top/gtisxrfvhc.html

Java: x instanceof Number
来源：http://hz.dashuyun.cn/gtuaagevex.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuanzx.com/gtnzcgajqz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zdqjudy.top/gtmzvjxjeb.html

C#:   x is int or double or decimal
来源：http://hz.316326.xyz/gtepmyemrp.html

[B14] 判断值是否在集合内
来源：http://hz.ywan-chungtsiang.top/gtysxnpgxy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.pycfn.com/gtxxsdrmhp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hfpthk.cn/gtoaqoenis.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.andypj.xyz/gtwmzrqbcj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gaohongyu789.top/gtodiuetih.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgufenzy.top/gttxpjpbgp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.havefunace.top/gtihyahfqc.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shanyushiyangtech.top/gtqgzbwkue.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhengqikj.top/gtpqtorudf.html

[B15] 布尔运算与取反
来源：http://hz.wangdashe.top/gtqigncjpw.html

Py:   a and b or not c
来源：http://hz.svipenyu.cn/gthessevsc.html

PHP:  $a && $b || !$c
来源：http://hz.chenjidiqi.icu/gtniqewusi.html

JS:   a && b || !c
来源：http://hz.yangfankeji.com/gtqgwexrlb.html

TS:   a && b || !c
来源：http://hz.aizwys.cn/gtekckzenw.html

Java: a && b || !c
来源：http://hz.fengsongda.top/gtmsxnhycp.html

Go:   a && b || !c
来源：http://hz.yueranfly.top/gtpvmwkcae.html

Ruby: a && b || !c
来源：http://hz.zhijiandao.cn/gtgihsossa.html

C#:   a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtnnwqmxfj.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cdnleiting.top/gthtrllnra.html

Py:   if not data: return
来源：http://hz.jinghuilouyu.cn/gtygoznwfy.html

PHP:  if (!$data) { return; }
来源：http://hz.iojbl.cn/gtyvmzttks.html

JS:   if (!data) return;
来源：http://hz.chenlongwang.top/gthrzcxwfg.html

TS:   if (!data) return;
来源：http://hz.feifeiyinyue.top/gtaulwrrnn.html

Java: if (data == null) return;
来源：http://hz.quarkkingdee.top/gtjjdlxgxa.html

Go:   if data == nil { return }
来源：http://hz.zdqjudy.top/gtjjvaniro.html

Ruby: return if data.nil?
来源：http://hz.yj202588.top/gtyfqtbvbx.html

C#:   if (data == null) return;
来源：http://hz.sweek.top/gtuccmlart.html

================================================================================
来源：http://hz.tianlin.xyz/gtivzligam.html

C. 函数与作用域
来源：http://hz.smart0.xyz/gtiansyzfn.html

================================================================================
来源：http://hz.meibo888.top/gtbrpuxjip.html

[C01] 定义函数
来源：http://hz.yj20258888.top/gtrrxppfis.html

Py:   def add(a, b): return a + b
来源：http://hz.fengsongda.top/gtfghsdhsj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.9152youxi.cn/gtggmdextd.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.iojbl.cn/gtrigffaik.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydzc1.top/gtmbgkvcok.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtvxeqcnka.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ppjwa.cn/gtgtmspnbb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hnqzz.top/gtlmxphxrq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtagfvolwl.html

[C02] 默认参数
来源：http://hz.zhijiandao.cn/gteccudwme.html

Py:   def greet(name="World"): return name
来源：http://hz.shuidangran.top/gtxudrmgwm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.havefunace.top/gtznbmsubo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pycfn.com/gtcylplilg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cashguo.top/gtxccltpxv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.fengsongda.top/gtdxsdxfhv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.meibo888.top/gtcwpotjby.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinqigfzy.top/gtxfxiksmi.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.havefunace.top/gtgfawrmop.html

[C03] 可变参数
来源：http://hz.shangyingyoupin.top/gtockdarsp.html

Py:   def total(*args): return sum(args)
来源：http://hz.xuanzx.com/gtifawmhpp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.gzhubu.top/gtwekpwgua.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhongyouzk.top/gtksixfxsh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.smart0.xyz/gtlhhuzzus.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yvedp.cn/gtnocvhhmu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.0kj1m.cn/gterzifhwy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jianghu66.top/gtpewjaoxf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jianghu66.top/gtqzsvrizu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xylfe.cn/gtkkdqgtxo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.aibaodan.cn/gthbcphhrz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ppjwa.cn/gtcoznkshd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtgyrrmxdt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.kuanghao11.cn/gtmfkmijkb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yuanzhike.top/gtsozzyoti.html

Go:   // 无：用配置结构体参数
来源：http://hz.iojbl.cn/gtjkwaxatz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.meibo888.top/gtcggygjur.html

C#:   f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtbsifdizd.html

[C05] 返回多个值
来源：http://hz.yuanzhike.top/gttfuunsxm.html

Py:   return a, b
来源：http://hz.sysykeji.top/gtprlniccl.html

PHP:  return [$a, $b];
来源：http://hz.sxryk.cn/gtabvbedvm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shuidangran.top/gtdzdkpvfi.html

TS:   return { a, b };
来源：http://hz.jlsjyb.cn/gtlxnsesqi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cucudq.cn/gtvbfbqmpa.html

Go:   return a, b
来源：http://hz.aibaodan.cn/gtlktwfrfn.html

Ruby: return a, b
来源：http://hz.andypj.xyz/gtbwwoqhqw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.kuanghao11.cn/gtvmdnsisj.html

[C06] 匿名函数 / lambda
来源：http://hz.haohaochexian.top/gtknzpkoey.html

Py:   square = lambda x: x * x
来源：http://hz.jinqigfzy.top/gtaalzkqbm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hysaishi.cn/gtuuxctklm.html

JS:   const square = x => x * x;
来源：http://hz.jianghu66.top/gtaruskyud.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhongyouzk.top/gtkniwavsa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhijiandao.cn/gtjrlbdxoi.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yuanzhike.top/gtskegmqay.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yueranfly.top/gtxpdbfrbw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.kuanghao11.cn/gtmrxsthyp.html

[C07] 把函数作为参数传入
来源：http://hz.jinyuanbaomall.cn/gtjxtfjqvu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.meibo888.top/gtcgpcwahz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yongpay.top/gtwhcvzcah.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cheryme.top/gtivvwcoff.html

TS:   arr.map(String)
来源：http://hz.316326.xyz/gtbgsduspi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ybcxt.top/gtlckwlpho.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zdqjudy.top/gtrbvyuxkk.html

Ruby: arr.map(&:upcase)
来源：http://hz.shanyushiyangtech.top/gtqxmsykoj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinqigufen.top/gthwjdezyr.html

[C08] 闭包
来源：http://hz.xylfe.cn/gtphonlyyz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gotoacloud.top/gtvryvgxqe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sufxvd.cn/gtflxtkged.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtkukpaxnd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtdixextqp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenzaomai.com/gtlmbgtsry.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cheryme.top/gtcisdylqp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yongpay.top/gtfjwboyzj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtdyzmdpna.html

[C09] 递归
来源：http://hz.sxryk.cn/gtyrcwcdvy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.wangdashe.top/gteelppvyu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhixingplan.top/gtfrkyvjtc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sysykeji.top/gtvygfgetd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258888.top/gtcrbwgckp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shanyushiyangtech.top/gtusnntlqm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.feifeiyinyue.top/gtgpobyejx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.pengpengdd.cyou/gtleyawkla.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenzaomai.com/gtqeqgwdbm.html

[C10] 变量作用域
来源：http://hz.xinyue.icu/gtibgpsxnr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.snrcjt.cn/gtmzzczsbq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sufxvd.cn/gtjivcezcd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yongpay.top/gtumuqjhuq.html

TS:   同 JS
来源：http://hz.zhongyouzk.top/gtiwohdhtj.html

Java: 方法内为块级作用域
来源：http://hz.ivvv.top/gtbyxrqxqz.html

Go:   花括号块级作用域
来源：http://hz.ivvv.top/gtuskncrqd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhengqikj.top/gtpjkfvofw.html

C#:   块级作用域
来源：http://hz.gogol.net.cn/gttfixsdqa.html

[C11] 模块导入与导出
来源：http://hz.yj20258.top/gtmynlcjjp.html

Py:   from module import func
来源：http://hz.feifeiyinyue.top/gtmzgxfwrs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ehwqpu.com/gtuhrgdypj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cdnleiting.top/gtlwneptwh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhongyouzk.top/gtvusuerep.html

Java: import java.util.List;
来源：http://hz.xinyue.icu/gtsspemxjm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhengqikj.top/gthcujgzlk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj202588.top/gtbrdhjuuo.html

C#:   using System.Text;
来源：http://hz.zycfv.cn/gtarpukamy.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhijiandao.cn/gtdphzhjoi.html

Py:   (lambda: print("run"))()
来源：http://hz.xziqi.cn/gtycjlsboi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigfzy.top/gtomebnqzv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtcsivfoqk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnxiangtu.top/gtdkfwxoqx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.svipenyu.cn/gtcsvjejzl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ydjk.org.cn/gteeiwptfk.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinqigfzy.top/gtmlhgufji.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinghuilouyu.cn/gtaizkbjbj.html

[C13] 类型声明 / 类型注解
来源：http://hz.yanxiufei.cn/gtlrfcmmvt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nanxuanxn.top/gtxgpsxrjh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gtawgihykb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuanzhike.top/gtrneqvrir.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gtqxhodymc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtuymzvlxx.html

Go:   func add(a, b int) int
来源：http://hz.yueranfly.top/gtokuxvodu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.nanxuanxn.top/gtsuovscyo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.tianlin.xyz/gttcqfbzfj.html

[C14] 泛型函数
来源：http://hz.hysaishi.cn/gtndlhvpbe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shzxlz.cn/gtylwqsgtk.html

PHP:  // 无泛型
来源：http://hz.yangfankeji.com/gtsdxmkoks.html

JS:   // 无泛型
来源：http://hz.xuetiantiany.cn/gttfijdgph.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinqigufen.top/gtxmsiqdzl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shanyushiyangkeji.top/gtwxxkcsxy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ybcxt.top/gtwnfnouhr.html

Ruby: # 无泛型
来源：http://hz.sufxvd.cn/gtkbmuyxzd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.havefunace.top/gtblqaknbg.html

[C15] 解构 / 展开参数
来源：http://hz.jianghu66.top/gtozicjxkm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gzhubu.top/gtwweabmsa.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nanxinkj.top/gtxbzotidc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.dianchejie.cn/gtybuyihpy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.quarkkingdee.top/gtppojkbpo.html

Java: // 无解构
来源：http://hz.hysaishi.cn/gtxinklwpd.html

Go:   // 无解构
来源：http://hz.yj20258888.top/gtyfjrkplw.html

Ruby: a, b = pair
来源：http://hz.52xcode.cn/gtlxtskgsf.html

C#:   var (a, b) = pair;
来源：http://hz.aizwys.cn/gtbgeujqmx.html

[C16] 函数 / 方法重载
来源：http://hz.shzxlz.cn/gtkzuejjqy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gaohongyu789.top/gtjzuwgxop.html

PHP:  // 无重载
来源：http://hz.gotoacloud.top/gtohvkwmdt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.aibaodan.cn/gtyklpvrjm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.52xcode.cn/gtfclukxjb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinyuanbaomall.cn/gtajrtnbak.html

Go:   // 无重载：用不同函数名
来源：http://hz.tian-w.cn/gttkhufpom.html

Ruby: # 无重载：靠动态参数
来源：http://hz.meibo888.top/gtkmunmesx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.feifeiyinyue.top/gtzfoanxit.html

================================================================================
来源：http://hz.ybcxt.top/gtkoyqbcyj.html

D. 数组 / 列表 / 集合
来源：http://hz.redwolf501.top/gtcsncdruy.html

================================================================================
来源：http://hz.hysaishi.cn/gtijhzdozl.html

[D01] 创建数组 / 列表
来源：http://hz.pengpengdd.cyou/gtibbgqjkl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenlongwang.top/gtjauecnxo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.feifeiyinyue.top/gtofjvfjmt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jianghu66.top/gtfkwemqfy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhiwuduotai.top/gtymjikmrw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xinyue.icu/gtywrwqyor.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zycfv.cn/gtsvfdnlio.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xziqi.cn/gtbthooaxa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ydjk.org.cn/gtlpshkybf.html

[D02] 追加元素到末尾
来源：http://hz.jinyuanbaomall.cn/gtqoaykwgs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jiagoushi.top/gtxlrsigot.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.c1oappe.top/gtflfmsctp.html

JS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtoerjpifu.html

TS:   arr.push(4);
来源：http://hz.redwolf501.top/gtpswzezks.html

Java: list.add(4);
来源：http://hz.xingfuxueyuan.xyz/gtgyfzdpxl.html

Go:   arr = append(arr, 4)
来源：http://hz.aibaodan.cn/gtfdzfzlyr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.dianchejie.cn/gtdertepei.html

C#:   list.Add(4);
来源：http://hz.jiagoushi.top/gtbycwfljf.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258.top/gtrteztxok.html

Py:   arr.insert(0, 0)
来源：http://hz.daria6918.cn/gtdbxlrqji.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ehwqpu.com/gtjdgdxzcn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinqigfzy.top/gtxgckssgh.html


<!-- 参考信息 -->