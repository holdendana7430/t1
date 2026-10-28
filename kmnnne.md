代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.hysaishi.cn/gttbiieutm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.nanxuanxn.top/gtvyewkjrx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jinghuilouyu.cn/gtclfjylhu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ehwqpu.com/gtxaicqnuh.html

[A26] 类型转换总览
来源：http://hz.smart0.xyz/gtlsfalwhz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.ydzc1.top/gttoepbnyf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xziqi.cn/gtgnmzlxvd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hysaishi.cn/gthjxwbsxw.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zhiwuduotai.top/gtkjphdyfp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jiagoushi.top/gtjghzdcjw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jqgfzy.top/gtfozkpvee.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.ywan-chungtsiang.top/gtqubxysrn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ydzc1.top/gtzsrocjsl.html

================================================================================
来源：http://hz.gzhubu.top/gtjdhnekqe.html

B. 流程控制
来源：http://hz.ppjwa.cn/gthugxhnxw.html

================================================================================
来源：http://hz.yj20258.top/gtnsusyled.html

[B01] 条件判断 if / else
来源：http://hz.ehwqpu.com/gtmhfvbigo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jyoumei.cn/gtzmjjftlm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.nanxuanxn.top/gtivqfoccg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jianghu66.top/gtvozuptqp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.nwbrower.top/gtnyfwiafy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.wangdashe.top/gtnbocwwtf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.dashuyun.cn/gtnskbiyec.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jqgufenzy.top/gtvaxypfsw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.c1oappe.top/gttjdsupqu.html

[B02] 多分支 else if / elif
来源：http://hz.shangyingyoupin.top/gtvmoihfkh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.sxryk.cn/gtkhglehmc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.gaohongyu789.top/gtwrqvrwfb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.snrcjt.cn/gthcqckeub.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daria6918.cn/gtqjhhfqty.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yanxiufei.cn/gtamkcevvg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jlsjyb.cn/gtespanyzm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.gzhubu.top/gtzwrucfrs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinqigufen.top/gtadyomwmb.html

[B03] switch / match / case
来源：http://hz.dashuyun.cn/gtbpgvbraz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.xinyue.icu/gtdqbwnqrq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.zhixingplan.top/gtwqhgraoo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.tanke756.top/gtjkjwjwxz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.feifeiyinyue.top/gtayzcmvdj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.cheryme.top/gtcibdcrwn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yueranfly.top/gtkmevgmdz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jinqigfzy.top/gtwzjzftjb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.daxiang520.top/gtfxprzbex.html

[B04] for 计数循环
来源：http://hz.zhongyouzk.top/gtfbuluqdh.html

Py:   for i in range(10): print(i)
来源：http://hz.nwbrower.top/gtjeuklkyy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.cucudq.cn/gtqdcmfqiv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.tanke756.top/gtywytsyef.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.fzhhl.top/gtopkpdxsb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.wangshuangyany.cn/gtkibrlfkj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hnqzz.top/gtdpkijtcf.html

Ruby: 10.times { |i| puts i }
来源：http://hz.dianchejie.cn/gtfieyqboy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhoulong.xyz/gttcvwkhbq.html

[B05] 遍历数组 / 列表
来源：http://hz.meibo888.top/gtvcugbnuj.html

Py:   for item in arr: print(item)
来源：http://hz.yuxming.cn/gtqyskbcox.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.daria6918.cn/gtauqupwly.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.wangshuangyany.cn/gtpnblnuel.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hfpthk.cn/gtfsnqrpqf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.smart0.xyz/gtytazzrjf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yangfankeji.com/gtgbkukmky.html

Ruby: arr.each { |item| puts item }
来源：http://hz.tanke756.top/gtyscskbxz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xuetiantiany.cn/gtlgnykocp.html

[B06] 遍历字典 / 对象
来源：http://hz.xinyue.icu/gthdwacsir.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.guowangkeji.top/gtyjscamgd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xinyue.icu/gtotkggfzs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj202588.top/gtcdbaxwbn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.smart0.xyz/gtfskoqjsw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.iojbl.cn/gtybzececb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.mhx1999.top/gtccfvlhac.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhongyouzk.top/gtyjqrvmzq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zhongyouzk.top/gtilrhkrto.html

[B07] while 循环
来源：http://hz.nwbrower.top/gtulnihblo.html

Py:   while i < 10: i += 1
来源：http://hz.chenzaomai.com/gtnzwhgzuu.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jinqigufen.top/gtziialzqi.html

JS:   while (i < 10) { i++; }
来源：http://hz.kuanghao11.cn/gtidalspjq.html

TS:   while (i < 10) { i++; }
来源：http://hz.52xcode.cn/gtsukftfru.html

Java: while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gtwedndlfd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.tianlin.xyz/gtjjbmflsr.html

Ruby: while i < 10; i += 1; end
来源：http://hz.wangshuangyany.cn/gtokwysaxs.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinqigfzy.top/gtfdbzhpug.html

[B08] do-while（至少执行一次）
来源：http://hz.zhiwuduotai.top/gtibjasxvs.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ppjwa.cn/gtbzpzpkds.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhengqikj.top/gtazlcqobb.html

JS:   do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtmubiqdur.html

TS:   do { i++; } while (i < 10);
来源：http://hz.vqdsnc.cn/gthlgysepx.html

Java: do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gtawsfokey.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.chenzaomai.com/gtsfcdtdvk.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cashguo.top/gtasrdefrs.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shangyingyoupin.top/gtuqnjxkzo.html

[B09] break 与 continue
来源：http://hz.jqgufenzy.top/gtloxxqkku.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.mhx1999.top/gtyngxwgcc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.smart0.xyz/gtekzrkcqy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.redwolf501.top/gtcapzlhbm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gzhubu.top/gtdcfzgmqc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj202588.top/gtablfoclz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.sysykeji.top/gtuzwfvlao.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xuanzx.com/gteueflpdv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.mhx1999.top/gttdbvriql.html

[B10] 遍历同时拿索引
来源：http://hz.jqgfzy.top/gtdcbehjqv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.havefunace.top/gtvgchblsq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yj20258.top/gtpweeiktc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yuxming.cn/gtfotgjgnn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hammf.cn/gtnllzuxcb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xuanzx.com/gttzrsljtm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhongyouzk.top/gtvmovxcsf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ywan-chungtsiang.top/gtboyjekiz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.9152youxi.cn/gtdvwahnkh.html

[B11] 生成数字序列 / 区间
来源：http://hz.havefunace.top/gtozfuvjje.html

Py:   list(range(0, 10, 2))
来源：http://hz.birdmap.top/gtoawjxxzc.html

PHP:  range(0, 10, 2);
来源：http://hz.vqdsnc.cn/gtelqdrgep.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cheryme.top/gtrjzkvszo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhiwuduotai.top/gtcduugkcr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.nanxinkj.top/gtrqmnhjzu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.daria6918.cn/gttmkojgbq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yangfankeji.com/gtapfsahfn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.birdmap.top/gtwixiosle.html

[B12] 跳出多层循环
来源：http://hz.kuanghao11.cn/gtkjagekdt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nwbrower.top/gtrnpjhdmr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.0kj1m.cn/gtgprysytb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jyoumei.cn/gtsysqqsex.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtnverkvxs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gtelqomkgd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.svipenyu.cn/gtilpsvzkl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.c1oappe.top/gtaamqzlbc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.0kj1m.cn/gtpfkzevzo.html

[B13] 判断是否为数字
来源：http://hz.gzhubu.top/gtnfswfior.html

Py:   isinstance(x, (int, float))
来源：http://hz.yj202588.top/gtrlpjqyiy.html

PHP:  is_numeric($x)
来源：http://hz.yuanzhike.top/gttmioiajb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tanke756.top/gtibkieepr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dianchejie.cn/gtofemlnsr.html

Java: x instanceof Number
来源：http://hz.xziqi.cn/gtqeanenca.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hfpthk.cn/gtizjzabjf.html

Ruby: x.is_a?(Numeric)
来源：http://hz.chenlongwang.top/gtxejcjqfh.html

C#:   x is int or double or decimal
来源：http://hz.jinyuanbaomall.cn/gtyifvdhdd.html

[B14] 判断值是否在集合内
来源：http://hz.meibo888.top/gtmepypopw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.chenzaomai.com/gttbpdkvds.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gogol.net.cn/gtbuspxhse.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.chenzaomai.com/gtkyqyqmlb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.meibo888.top/gtuwulcaei.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.aibaodan.cn/gtblulbdif.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jianghu66.top/gtxdtnikef.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.mhx1999.top/gtqiffslse.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tanke756.top/gtqjofdtpg.html

[B15] 布尔运算与取反
来源：http://hz.yuxming.cn/gtvrgdrxso.html

Py:   a and b or not c
来源：http://hz.jinqigfzy.top/gtcuoihqne.html

PHP:  $a && $b || !$c
来源：http://hz.chenlongwang.top/gtyylfksyd.html

JS:   a && b || !c
来源：http://hz.gotoacloud.top/gtmauznbgs.html

TS:   a && b || !c
来源：http://hz.dashuyun.cn/gtkbrtlduj.html

Java: a && b || !c
来源：http://hz.zhijiandao.cn/gtmeujelwb.html

Go:   a && b || !c
来源：http://hz.hammf.cn/gtcjkulufh.html

Ruby: a && b || !c
来源：http://hz.jiagoushi.top/gtwyhciuyv.html

C#:   a && b || !c
来源：http://hz.kuanghao11.cn/gtxfpjuvou.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.pycfn.com/gtpjkqxfup.html

Py:   if not data: return
来源：http://hz.smart0.xyz/gtkvrtcaof.html

PHP:  if (!$data) { return; }
来源：http://hz.zhixingplan.top/gtvdveqfzv.html

JS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtlevwxhja.html

TS:   if (!data) return;
来源：http://hz.ywan-chungtsiang.top/gtfjxdzbgp.html

Java: if (data == null) return;
来源：http://hz.ehwqpu.com/gtyizdembm.html

Go:   if data == nil { return }
来源：http://hz.zhijiandao.cn/gticnznvvj.html

Ruby: return if data.nil?
来源：http://hz.pengpengdd.cyou/gtakrlhfzc.html

C#:   if (data == null) return;
来源：http://hz.jinyuanbaomall.cn/gtghutgekj.html

================================================================================
来源：http://hz.aizwys.cn/gtxbvheekn.html

C. 函数与作用域
来源：http://hz.jinqigfzy.top/gtepqemswd.html

================================================================================
来源：http://hz.yj20258.top/gtqamtpgnw.html

[C01] 定义函数
来源：http://hz.9152youxi.cn/gtifmslsdw.html

Py:   def add(a, b): return a + b
来源：http://hz.hammf.cn/gtyzddlpch.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnqzz.top/gtoewqsniv.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.wangdashe.top/gtivogvxxh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenzaomai.com/gtggmxxiwh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gtztcxsved.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pycfn.com/gtegegiskd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gaohongyu789.top/gtgmdllxjg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yongpay.top/gtezsukddp.html

[C02] 默认参数
来源：http://hz.9152youxi.cn/gtjalmtzeh.html

Py:   def greet(name="World"): return name
来源：http://hz.ywan-chungtsiang.top/gtchharert.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.smart0.xyz/gtgwagsjea.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.daxiang520.top/gtafrlduan.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.tian-w.cn/gtodiwurbg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hongshengwenyu.top/gtpeewsgfk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ybcxt.top/gtoweevnrg.html

Ruby: def greet(name = "World") = name
来源：http://hz.sxryk.cn/gtozjdoeqf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.feifeiyinyue.top/gtrmvdeomg.html

[C03] 可变参数
来源：http://hz.0kj1m.cn/gtplodkkjo.html

Py:   def total(*args): return sum(args)
来源：http://hz.sxryk.cn/gtfpcrelxr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dianchejie.cn/gtdzcjljgh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hywenlv.cn/gtqumqzuls.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinqigfzy.top/gtlmtxgrit.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.nanxuanxn.top/gtzymgqehk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xuetiantiany.cn/gthylcgdsi.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tian-w.cn/gtdusmmovm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xziqi.cn/gtldmfmtnq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shanyushiyangkeji.top/gtamoxdlue.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.birdmap.top/gtqaoqazjk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhengqikj.top/gtddsidhru.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tian-w.cn/gtujukvlez.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yvedp.cn/gtbwwbojkf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yuxming.cn/gtcjyhmzht.html

Go:   // 无：用配置结构体参数
来源：http://hz.wangshuangyany.cn/gtyclmtnzs.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinyuanbaomall.cn/gtveoslexc.html

C#:   f(a: 1, b: 2)
来源：http://hz.pycfn.com/gtimfwvkxg.html

[C05] 返回多个值
来源：http://hz.sweek.top/gtxjytpbhz.html

Py:   return a, b
来源：http://hz.ivvv.top/gtrdyxqsak.html

PHP:  return [$a, $b];
来源：http://hz.meibo888.top/gtziebeqyb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.chenzaomai.com/gtgfnulhbc.html

TS:   return { a, b };
来源：http://hz.guowangkeji.top/gtipbafgud.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hammf.cn/gtwwryofvp.html

Go:   return a, b
来源：http://hz.hongshengwenyu.top/gtfhlatxga.html

Ruby: return a, b
来源：http://hz.haohaochexian.top/gtfthfxspc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnxiangtu.top/gtojqzifre.html

[C06] 匿名函数 / lambda
来源：http://hz.yangfankeji.com/gtdlcmzbpt.html

Py:   square = lambda x: x * x
来源：http://hz.gotoacloud.top/gtmytulufu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shzxlz.cn/gtfqvckrvt.html

JS:   const square = x => x * x;
来源：http://hz.snrcjt.cn/gtmpjgacnc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.haohaochexian.top/gtrzbxcydo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.fzhhl.top/gtrgsfbihr.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cheryme.top/gtxvemnklt.html

Ruby: square = ->(x) { x * x }
来源：http://hz.vqdsnc.cn/gtzsyngnlo.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jianghu66.top/gtcefcohgw.html

[C07] 把函数作为参数传入
来源：http://hz.tanke756.top/gtwwmmzrli.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hfpthk.cn/gtaucwmqjp.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nanxinkj.top/gtsmolrovd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.chenjidiqi.icu/gtdngdqzpk.html

TS:   arr.map(String)
来源：http://hz.pengpengdd.cyou/gtjdzbyzrt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nanxuanxn.top/gtgcbmpbta.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj202588.top/gtixinkryz.html

Ruby: arr.map(&:upcase)
来源：http://hz.cqqwz.cn/gtgyrolnlo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhiwuduotai.top/gtexinboxf.html

[C08] 闭包
来源：http://hz.jqgufenzy.top/gtaopwqrol.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangkeji.top/gtvjjvauoa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yueranfly.top/gtwcfkpypk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xziqi.cn/gtgzezmhck.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtqsmzbyoq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hfpthk.cn/gtrputkkab.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yongpay.top/gtnzyqejsk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sysykeji.top/gtrbsbgpvw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yvedp.cn/gtmtlcmbwu.html

[C09] 递归
来源：http://hz.fzhhl.top/gtaduuybpg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xinyue.icu/gtwlpumvuj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tian-w.cn/gtnszbnvww.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.svipenyu.cn/gtwuxgmefu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aizwys.cn/gtzrsbvktg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cucudq.cn/gtujerfjpg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.fengsongda.top/gtsvzjvads.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj20258888.top/gtiqrkzwmb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jiagoushi.top/gtvudwyrcf.html

[C10] 变量作用域
来源：http://hz.sufxvd.cn/gtkpqenjuc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sufxvd.cn/gtkhdljknr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.0kj1m.cn/gtutsqrzfj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.smart0.xyz/gtmvywaifa.html

TS:   同 JS
来源：http://hz.52xcode.cn/gtjefmvzvk.html

Java: 方法内为块级作用域
来源：http://hz.hnqzz.top/gtdyrpqhxm.html

Go:   花括号块级作用域
来源：http://hz.yongpay.top/gtkrhqmilr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.pengpengdd.cyou/gtfhqffdpa.html

C#:   块级作用域
来源：http://hz.yj202588.top/gtkikecrez.html

[C11] 模块导入与导出
来源：http://hz.yuanzhike.top/gtprfhgoci.html

Py:   from module import func
来源：http://hz.nwbrower.top/gtxwxaafyj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yonumen.top/gtxvhtbmzv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.andypj.xyz/gthwmdglnj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.chenzaomai.com/gtmzknouxr.html

Java: import java.util.List;
来源：http://hz.gaohongyu789.top/gtdxzxpvtd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zycfv.cn/gtjltpedrp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.316326.xyz/gtzieuroiv.html

C#:   using System.Text;
来源：http://hz.yangfankeji.com/gtxvlwkwnx.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigufen.top/gtsakssbxt.html

Py:   (lambda: print("run"))()
来源：http://hz.yuanzhike.top/gtnpcuegti.html

PHP:  (function () { echo "run"; })();
来源：http://hz.52xcode.cn/gttnubzyef.html

JS:   (() => { console.log("run"); })();
来源：http://hz.svipenyu.cn/gtfnmzmkyf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtslgzufts.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ehwqpu.com/gthgibwoyy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nanxinkj.top/gtzfmvtubb.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj20258.top/gtcmpfwatn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jiagoushi.top/gtktmlzynr.html

[C13] 类型声明 / 类型注解
来源：http://hz.jinqigfzy.top/gtzotykvmp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuetiantiany.cn/gtodgqoekv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhijiandao.cn/gtyshrzqox.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cashguo.top/gthnphlmsw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtwpsblqrq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtupbshuic.html

Go:   func add(a, b int) int
来源：http://hz.c1oappe.top/gtdsrdruew.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hammf.cn/gtvhpcgoef.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gotoacloud.top/gtqylullxc.html

[C14] 泛型函数
来源：http://hz.yangfankeji.com/gtoskvpgrc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.smart0.xyz/gtrcljkluf.html

PHP:  // 无泛型
来源：http://hz.yuxming.cn/gtqaknlfyl.html

JS:   // 无泛型
来源：http://hz.jiagoushi.top/gtbzucdgft.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gaohongyu789.top/gtbdegkmpp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hnqzz.top/gtiiutmrrw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj202588.top/gtcmmruxfl.html

Ruby: # 无泛型
来源：http://hz.chenzaomai.com/gtbpcoljbv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hnqzz.top/gtdrdyhptf.html

[C15] 解构 / 展开参数
来源：http://hz.yj202588.top/gtxfjxnwfq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fengsongda.top/gtemqgppwb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cheryme.top/gtzownfwnr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xuetiantiany.cn/gtjtejqmai.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.sweek.top/gtagrezvqp.html

Java: // 无解构
来源：http://hz.daria6918.cn/gtgvnwlehq.html

Go:   // 无解构
来源：http://hz.316326.xyz/gtjaqwqfmw.html

Ruby: a, b = pair
来源：http://hz.yueranfly.top/gtgmsgqwaw.html

C#:   var (a, b) = pair;
来源：http://hz.sysykeji.top/gtkygnqasb.html

[C16] 函数 / 方法重载
来源：http://hz.ydzc1.top/gtuiywydso.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nanxinkj.top/gtvmdyxelw.html


<!-- 参考信息 -->