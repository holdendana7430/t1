代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.aibaodan.cn/gtbvjxzsrn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.kuanghao11.cn/gteunjplhj.html

[B03] switch / match / case
来源：http://hz.316326.xyz/gtrpuhuhhx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.ppjwa.cn/gtrgzwxhqp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.chenjidiqi.icu/gthxkevshy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenlongwang.top/gtbxhbmaht.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhongyouzk.top/gtyynnxwxu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.gogol.net.cn/gtpbzybokx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.cucudq.cn/gtphmifecx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hfpthk.cn/gtehdacldc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yonumen.top/gthkjzfmwa.html

[B04] for 计数循环
来源：http://hz.hongshengwenyu.top/gtrgcqhmgq.html

Py:   for i in range(10): print(i)
来源：http://hz.hysaishi.cn/gtceabiwgj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.haohaochexian.top/gtanhwsgot.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.meibo888.top/gttpmqlwhv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yuxming.cn/gttyvhmjnn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yvedp.cn/gtknsvcryl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.vqdsnc.cn/gtidjtfxen.html

Ruby: 10.times { |i| puts i }
来源：http://hz.tian-w.cn/gtllqjdptr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xinyue.icu/gtihlmyqpm.html

[B05] 遍历数组 / 列表
来源：http://hz.zhoulong.xyz/gttbjttydf.html

Py:   for item in arr: print(item)
来源：http://hz.xinyue.icu/gttcrupgzo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.shangyingyoupin.top/gtyxnvmtjs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.gaohongyu789.top/gtdyjiarfz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.meibo888.top/gtwixdfkhb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.chenjidiqi.icu/gtdecnwfin.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.quarkkingdee.top/gtrnwcnaok.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yuxming.cn/gttkffrdke.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.sxryk.cn/gteyzigzvf.html

[B06] 遍历字典 / 对象
来源：http://hz.yj202588.top/gtxcbplbry.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cucudq.cn/gtsmbjqzjk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.feifeiyinyue.top/gtfuahxlpu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hywenlv.cn/gtinwzpobw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xuetiantiany.cn/gtiqrcstwc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.andypj.xyz/gtclwvaojz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.mhx1999.top/gttzrhcoeh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jianghu66.top/gtwrcootmv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.iojbl.cn/gtflknvlvj.html

[B07] while 循环
来源：http://hz.yongpay.top/gttsmrtlde.html

Py:   while i < 10: i += 1
来源：http://hz.aizwys.cn/gtghxtzqpm.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.chenlongwang.top/gtjkqqnedn.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhijiandao.cn/gtahxjqcpc.html

TS:   while (i < 10) { i++; }
来源：http://hz.ppjwa.cn/gtiejzxmzd.html

Java: while (i < 10) { i++; }
来源：http://hz.yj20258.top/gtrnlaxrnm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.quarkkingdee.top/gtcoipcbvx.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hfpthk.cn/gtqfgahqqf.html

C#:   while (i < 10) { i++; }
来源：http://hz.guowangkeji.top/gtbmhutoot.html

[B08] do-while（至少执行一次）
来源：http://hz.quarkkingdee.top/gtbjtcvupo.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.nanxinkj.top/gtlvznqzhu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhengqikj.top/gtmkcbfnvy.html

JS:   do { i++; } while (i < 10);
来源：http://hz.chenlongwang.top/gtopxoltxu.html

TS:   do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gtlasiihnu.html

Java: do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtxlvcqqgt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jqgufenzy.top/gtriyktlqr.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.kuanghao11.cn/gtdajarhsn.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jiagoushi.top/gtayhrjduh.html

[B09] break 与 continue
来源：http://hz.shuidangran.top/gttkhxcxjj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.aibaodan.cn/gtnukdgttt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhijiandao.cn/gtuwemjqvz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.mhx1999.top/gtpsrhbdpj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxinkj.top/gtvjopbbwu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hfpthk.cn/gtgpaeigdd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.haohaochexian.top/gtgxdkdudb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xylfe.cn/gtaeetrlqp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhoulong.xyz/gtbxgidnuz.html

[B10] 遍历同时拿索引
来源：http://hz.hammf.cn/gtrrysgnga.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.52xcode.cn/gttoiknpdp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.tanke756.top/gtyjwswnib.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xylfe.cn/gtcajucsra.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yangfankeji.com/gtwmvdwxrj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cucudq.cn/gtbnennxpx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jqgfzy.top/gtgldtzezd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.havefunace.top/gtqqpofkqc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.nwbrower.top/gtkkazzmnz.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhoulong.xyz/gtuwaxyjyp.html

Py:   list(range(0, 10, 2))
来源：http://hz.jqgufenzy.top/gtdrhegqza.html

PHP:  range(0, 10, 2);
来源：http://hz.cdnleiting.top/gtatpxizjf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.c1oappe.top/gtnjcwvhxg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.quarkkingdee.top/gtvstampjk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhongyouzk.top/gtnrbpvrrn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj20258.top/gtdbbqehkv.html

Ruby: (0...10).step(2).to_a
来源：http://hz.tian-w.cn/gtiuyezery.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.guowangkeji.top/gtntppjalj.html

[B12] 跳出多层循环
来源：http://hz.ehwqpu.com/gtaryuqmwz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ppjwa.cn/gtbndmqxpb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shzxlz.cn/gtttgzwtoa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gtuaprafhm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtxhyzirkh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhoulong.xyz/gtyjdtvrhk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jyoumei.cn/gtzpksyjon.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ydjk.org.cn/gtqldemyuz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.guannengcc.top/gtmaakabil.html

[B13] 判断是否为数字
来源：http://hz.cucudq.cn/gttklysgbq.html

Py:   isinstance(x, (int, float))
来源：http://hz.xuetiantiany.cn/gtkxfcesfn.html

PHP:  is_numeric($x)
来源：http://hz.vqdsnc.cn/gtluuukzni.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guannengcc.top/gtdnnicaxp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hnqzz.top/gtniayjntg.html

Java: x instanceof Number
来源：http://hz.hammf.cn/gtyasfluux.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.wangshuangyany.cn/gtgewqlojk.html

Ruby: x.is_a?(Numeric)
来源：http://hz.daria6918.cn/gtnokcgqrq.html

C#:   x is int or double or decimal
来源：http://hz.shuidangran.top/gtymhhquyb.html

[B14] 判断值是否在集合内
来源：http://hz.zhijiandao.cn/gtmaxmpceb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.mhx1999.top/gtuvhqwahc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gogol.net.cn/gtsgqnpedn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yonumen.top/gtmmyktrnj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.wangdashe.top/gthxcdmjuo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hnqzz.top/gtptqqelqs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.iojbl.cn/gtcfrsimip.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hongshengwenyu.top/gtixuzpdyd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xuanzx.com/gtklyedjgp.html

[B15] 布尔运算与取反
来源：http://hz.hammf.cn/gtumdbexlv.html

Py:   a and b or not c
来源：http://hz.0kj1m.cn/gtskxeuppp.html

PHP:  $a && $b || !$c
来源：http://hz.zhoulong.xyz/gtgbtoqqre.html

JS:   a && b || !c
来源：http://hz.dashuyun.cn/gtdpjetdwe.html

TS:   a && b || !c
来源：http://hz.gogol.net.cn/gtocgyuqvn.html

Java: a && b || !c
来源：http://hz.svipenyu.cn/gtlfybmouc.html

Go:   a && b || !c
来源：http://hz.hammf.cn/gtclvjhpuo.html

Ruby: a && b || !c
来源：http://hz.xylfe.cn/gtwpkkzqwc.html

C#:   a && b || !c
来源：http://hz.nanxuanxn.top/gttblrgcay.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jlsjyb.cn/gtkxcntwwe.html

Py:   if not data: return
来源：http://hz.jinqigufen.top/gthhzksjff.html

PHP:  if (!$data) { return; }
来源：http://hz.xinyue.icu/gtaxwfzfrd.html

JS:   if (!data) return;
来源：http://hz.hnxiangtu.top/gtyevoimnb.html

TS:   if (!data) return;
来源：http://hz.xziqi.cn/gtvmvcsfsq.html

Java: if (data == null) return;
来源：http://hz.chenzaomai.com/gtpgcmqhgs.html

Go:   if data == nil { return }
来源：http://hz.pengpengdd.cyou/gtipnnbgkf.html

Ruby: return if data.nil?
来源：http://hz.nanxinkj.top/gtsstllmvd.html

C#:   if (data == null) return;
来源：http://hz.chenzaomai.com/gtdqdqvvep.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtjvoxpofu.html

C. 函数与作用域
来源：http://hz.yonumen.top/gtipsqrjbl.html

================================================================================
来源：http://hz.haohaochexian.top/gtzqzrbkyh.html

[C01] 定义函数
来源：http://hz.sweek.top/gtoyuunuzo.html

Py:   def add(a, b): return a + b
来源：http://hz.316326.xyz/gthidjjfea.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtlrrhgitr.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtfzsyuhgl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258.top/gtpzdykgmi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtateviwkx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ehwqpu.com/gtkhupmjhc.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenzaomai.com/gtpswnmrhj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtbllewvuu.html

[C02] 默认参数
来源：http://hz.svipenyu.cn/gttzifxotz.html

Py:   def greet(name="World"): return name
来源：http://hz.haohaochexian.top/gtqmtycokq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hongshengwenyu.top/gtzirafizz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhiwuduotai.top/gtqzkjnqmb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.aizwys.cn/gtncirovtj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ppjwa.cn/gtogrfzcev.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shzxlz.cn/gtbedipbws.html

Ruby: def greet(name = "World") = name
来源：http://hz.yanxiufei.cn/gtrxhytxqf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shanyushiyangtech.top/gtydplgjma.html

[C03] 可变参数
来源：http://hz.jinqigfzy.top/gtaxmgykmd.html

Py:   def total(*args): return sum(args)
来源：http://hz.hongshengwenyu.top/gtnapegexj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.pengpengdd.cyou/gtuujxpady.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jiagoushi.top/gtkuunoicd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zdqjudy.top/gtyuqqmvoa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zdqjudy.top/gtbygnybek.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xziqi.cn/gtzhscnbbp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hfpthk.cn/gtuurzuuzc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yuxming.cn/gtnngkcepk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yangfankeji.com/gtxgldmpvf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xziqi.cn/gtmeouvcsd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jyoumei.cn/gtqhjvpeme.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sxryk.cn/gtfczgrfjq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xinyue.icu/gtjdigcpfl.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhiwuduotai.top/gtplhwytzp.html

Go:   // 无：用配置结构体参数
来源：http://hz.316326.xyz/gtwrdhasnw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtzkpnejlj.html

C#:   f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gtegtfzaxm.html

[C05] 返回多个值
来源：http://hz.yanxiufei.cn/gtnlnrryfl.html

Py:   return a, b
来源：http://hz.yj202588.top/gtahpwobdp.html

PHP:  return [$a, $b];
来源：http://hz.tanke756.top/gtcihbhyby.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.kuanghao11.cn/gtxcosgdmq.html

TS:   return { a, b };
来源：http://hz.sufxvd.cn/gtbrgrlbke.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hnqzz.top/gtlfprkmxw.html

Go:   return a, b
来源：http://hz.yueranfly.top/gtybjfbccj.html

Ruby: return a, b
来源：http://hz.vqdsnc.cn/gtmcfcjwdz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gaohongyu789.top/gtjclpbodi.html

[C06] 匿名函数 / lambda
来源：http://hz.yangfankeji.com/gtmvzwcrpc.html

Py:   square = lambda x: x * x
来源：http://hz.hnqzz.top/gtpkgxqdhj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhoulong.xyz/gtewwoyhkx.html

JS:   const square = x => x * x;
来源：http://hz.gotoacloud.top/gtcawjazrf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.pengpengdd.cyou/gtbfibttul.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hywenlv.cn/gtjfsqvzzo.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinghuilouyu.cn/gthcrrssxf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cashguo.top/gtisxtyimf.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gtfruqbajj.html

[C07] 把函数作为参数传入
来源：http://hz.hnqzz.top/gtqhyqxall.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.pycfn.com/gtlrixaohk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guowangkeji.top/gtzkjuceuv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.meibo888.top/gtpnrbosiz.html

TS:   arr.map(String)
来源：http://hz.hywenlv.cn/gttmoldsti.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ppjwa.cn/gtspywteqw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.52xcode.cn/gtuofdgjhn.html

Ruby: arr.map(&:upcase)
来源：http://hz.tianlin.xyz/gtzfvgkuxw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ehwqpu.com/gtnclnokkp.html

[C08] 闭包
来源：http://hz.ydzc1.top/gtkdqarytx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangshuangyany.cn/gtbbyeffzm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hnxiangtu.top/gtqtbkxadk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtnobfpyxs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sxryk.cn/gtnvbxxyku.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jlsjyb.cn/gtmdjxkbxt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.snrcjt.cn/gtawewjfdq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj20258.top/gtemspvapa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtdpziydvq.html

[C09] 递归
来源：http://hz.xziqi.cn/gtweuthbod.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.birdmap.top/gtjtomyegk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.fengsongda.top/gtvhtohyca.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cashguo.top/gthwzhlmvk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pengpengdd.cyou/gtcoqtkahk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gzhubu.top/gtbdbcenrg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sxryk.cn/gtczvjmkco.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hysaishi.cn/gtjvsnzhod.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jianghu66.top/gtbwpivgrd.html

[C10] 变量作用域
来源：http://hz.zhixingplan.top/gtqdstykca.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gogol.net.cn/gtowkgycex.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.aizwys.cn/gtgykswmkr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sysykeji.top/gtevukvqfn.html

TS:   同 JS
来源：http://hz.yueranfly.top/gtgyalmtba.html

Java: 方法内为块级作用域
来源：http://hz.nanxuanxn.top/gtakgztuso.html

Go:   花括号块级作用域
来源：http://hz.shuidangran.top/gtqdegwnjm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yonumen.top/gtngbcnlql.html

C#:   块级作用域
来源：http://hz.snrcjt.cn/gtisipgfhp.html

[C11] 模块导入与导出
来源：http://hz.hywenlv.cn/gtfyvuonig.html

Py:   from module import func
来源：http://hz.xylfe.cn/gtulhksmpi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ybcxt.top/gttktuavku.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnqzz.top/gtvqvkxiqo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tian-w.cn/gtcjzmqeyx.html

Java: import java.util.List;
来源：http://hz.jinqigfzy.top/gtyfztkhmw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yongpay.top/gtdcoiyjma.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hongshengwenyu.top/gthobavsfv.html

C#:   using System.Text;
来源：http://hz.nanxinkj.top/gtbjouwkxm.html

[C12] 立即执行函数 IIFE
来源：http://hz.ydzc1.top/gtgufqsevd.html

Py:   (lambda: print("run"))()
来源：http://hz.hongshengwenyu.top/gtfjquanwk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ehwqpu.com/gtpfzhpdlx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sxryk.cn/gtnitknxjs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nanxinkj.top/gtzngklxrg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ybcxt.top/gtnhybrfqz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.bjfxy.top/gtrdrsbtvq.html

Ruby: -> { puts "run" }.call
来源：http://hz.ivvv.top/gttmookymp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yvedp.cn/gtqxxynslb.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhoulong.xyz/gtfzczxzst.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cqqwz.cn/gtcevwnick.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gtjzxzqlpj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ybcxt.top/gtuyrxletb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gzhubu.top/gtngqpapdi.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtvxpmfidu.html

Go:   func add(a, b int) int
来源：http://hz.xuanzx.com/gttlwbgzek.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ppjwa.cn/gtaetortmk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.havefunace.top/gtbgitpolb.html

[C14] 泛型函数
来源：http://hz.hongshengwenyu.top/gtqziexxyy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xinyue.icu/gtwiwrgsxy.html

PHP:  // 无泛型
来源：http://hz.sufxvd.cn/gtwlsmurhn.html

JS:   // 无泛型
来源：http://hz.svipenyu.cn/gtuprskrbz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yonumen.top/gtynfftbwr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cdnleiting.top/gtfuyqciwt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sufxvd.cn/gtwerklijl.html

Ruby: # 无泛型
来源：http://hz.zhiwuduotai.top/gthtwzwbuz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.quarkkingdee.top/gttusyfyfp.html

[C15] 解构 / 展开参数
来源：http://hz.zhiwuduotai.top/gtvmjgqodu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhijiandao.cn/gttbsbywpc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.pengpengdd.cyou/gteltvbuwi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gtnelhvmmu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.meibo888.top/gtervaxtdq.html

Java: // 无解构
来源：http://hz.hysaishi.cn/gtcatblzrs.html

Go:   // 无解构
来源：http://hz.guowangkeji.top/gtlhbnzjxs.html

Ruby: a, b = pair
来源：http://hz.gzhubu.top/gtfnjrhosu.html

C#:   var (a, b) = pair;
来源：http://hz.snrcjt.cn/gtzqdxdisf.html

[C16] 函数 / 方法重载
来源：http://hz.yangfankeji.com/gtjfchwfbi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ybcxt.top/gtsrglheyp.html

PHP:  // 无重载
来源：http://hz.ydzc1.top/gtdhukmtwo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenlongwang.top/gtfbcmqxfl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.haohaochexian.top/gtcnlluela.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.svipenyu.cn/gtzzjokvbq.html

Go:   // 无重载：用不同函数名
来源：http://hz.ppjwa.cn/gtqosutacf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.snrcjt.cn/gtpdkrijrw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.aibaodan.cn/gtzhgyfvkf.html

================================================================================
来源：http://hz.52xcode.cn/gthbuwfsda.html

D. 数组 / 列表 / 集合
来源：http://hz.yj202588.top/gtlhqgooyn.html

================================================================================
来源：http://hz.cdnleiting.top/gtiejdgfud.html

[D01] 创建数组 / 列表
来源：http://hz.hongshengwenyu.top/gtfvsfdayw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.nwbrower.top/gtnwppgyxp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhengqikj.top/gtwivgwmki.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yuxming.cn/gtkvjhzszv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhongyouzk.top/gtambydqpl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenzaomai.com/gtzemuywbl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xuetiantiany.cn/gtezbtoepc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.chenzaomai.com/gtpjaqojcn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.52xcode.cn/gtilifzlou.html

[D02] 追加元素到末尾
来源：http://hz.vqdsnc.cn/gtywmqjtey.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gzhubu.top/gtsmtiyjrd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.smart0.xyz/gtbagcicmd.html

JS:   arr.push(4);
来源：http://hz.mhx1999.top/gtocgypahk.html

TS:   arr.push(4);
来源：http://hz.hfpthk.cn/gtgybywmnu.html

Java: list.add(4);
来源：http://hz.quarkkingdee.top/gteruwkfez.html

Go:   arr = append(arr, 4)
来源：http://hz.jinyuanbaomall.cn/gttqvtcwyj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenzaomai.com/gtmcdnisuv.html

C#:   list.Add(4);
来源：http://hz.zhixingplan.top/gtwnvpzkuy.html

[D03] 在指定位置插入元素
来源：http://hz.xuanzx.com/gtndvxyikx.html

Py:   arr.insert(0, 0)
来源：http://hz.gzhubu.top/gtdyuobbic.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hammf.cn/gteclydxkx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.fzhhl.top/gtdvpeywde.html


<!-- 参考信息 -->