代发 wailian999

[A26] 类型转换总览
来源：http://hz.jinqigfzy.top/gtidldxrie.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.nanxinkj.top/gtciocxlnp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.sweek.top/gtkzoaqmbp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ehwqpu.com/gtottlpshz.html

TS:   Number() String() Boolean() x as number
来源：http://hz.cucudq.cn/gteezpoiig.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yanxiufei.cn/gtithcgxpa.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yvedp.cn/gtxrwwuzgt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.redwolf501.top/gtjvdbvkxh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhixingplan.top/gtjtgfhbhe.html

================================================================================
来源：http://hz.hfpthk.cn/gttrrbqtxg.html

B. 流程控制
来源：http://hz.jinqigufen.top/gtpvaryuyq.html

================================================================================
来源：http://hz.nanxinkj.top/gttncktfyf.html

[B01] 条件判断 if / else
来源：http://hz.guannengcc.top/gtebwnsjti.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.kuanghao11.cn/gtecbvveyw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.c1oappe.top/gtbkryosmx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.vqdsnc.cn/gtdraweycp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.gaohongyu789.top/gtvfgsxydm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhijiandao.cn/gtosapdgxz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.wangdashe.top/gtyxnaeknr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhiwuduotai.top/gtsayhlact.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.cqqwz.cn/gtjratlqiv.html

[B02] 多分支 else if / elif
来源：http://hz.chenlongwang.top/gtunccwzql.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.wangshuangyany.cn/gtopjphhom.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.pycfn.com/gtpbdihgoq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shzxlz.cn/gtaugtagtp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.birdmap.top/gtsdrrnvpb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daria6918.cn/gtjhalbdgf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.guannengcc.top/gtbgyvuaab.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.ydzc1.top/gtsdqgduer.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sxryk.cn/gtoadifuxa.html

[B03] switch / match / case
来源：http://hz.mhx1999.top/gtdjzccdqb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.gotoacloud.top/gtwjzvgnrv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jianghu66.top/gtikubswmz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ywan-chungtsiang.top/gtqvfggypj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jiagoushi.top/gtwisfllci.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jiagoushi.top/gtjtsnbbgy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.ivvv.top/gtkyeuwrap.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cqqwz.cn/gtkrkfglav.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.gotoacloud.top/gtobqgabnv.html

[B04] for 计数循环
来源：http://hz.pengpengdd.cyou/gtprvotgad.html

Py:   for i in range(10): print(i)
来源：http://hz.quarkkingdee.top/gtmqwjqbay.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.hfpthk.cn/gtrmmgawcc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hammf.cn/gtpdjgofmg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yueranfly.top/gtvlnarphm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.aibaodan.cn/gtfmsxyfnz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.tianlin.xyz/gtgjntybqh.html

Ruby: 10.times { |i| puts i }
来源：http://hz.hywenlv.cn/gtkiwqkjbh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhixingplan.top/gtgqejvqku.html

[B05] 遍历数组 / 列表
来源：http://hz.jinyuanbaomall.cn/gtoakumdig.html

Py:   for item in arr: print(item)
来源：http://hz.yueranfly.top/gtocyvakeu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.cucudq.cn/gtmzeaxhos.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj20258888.top/gtpjmzicrx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hnqzz.top/gtgtgalcqw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jiagoushi.top/gtfojxvgkv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.redwolf501.top/gteofajpdh.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zhengqikj.top/gtkxrxltbs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.fengsongda.top/gthjgkuwfb.html

[B06] 遍历字典 / 对象
来源：http://hz.jinghuilouyu.cn/gtybjlzmlf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhongyouzk.top/gtqezwnyvm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yanxiufei.cn/gtjigfxsyg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yanxiufei.cn/gtwekkopfb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.svipenyu.cn/gtmuhtcgpa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cheryme.top/gtguaikewc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yj20258.top/gthssfpmsx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xinyue.icu/gtepofqqqz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jinqigfzy.top/gtimqmlxir.html

[B07] while 循环
来源：http://hz.zhaomingkeji.xyz/gtqadmndzh.html

Py:   while i < 10: i += 1
来源：http://hz.yj20258888.top/gtznpiuoid.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.tian-w.cn/gtgwodcjjz.html

JS:   while (i < 10) { i++; }
来源：http://hz.jqgufenzy.top/gtaemifnsr.html

TS:   while (i < 10) { i++; }
来源：http://hz.wangdashe.top/gtcxvvlpgc.html

Java: while (i < 10) { i++; }
来源：http://hz.yj20258.top/gtscmfjzog.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jinyuanbaomall.cn/gtscbtphah.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hammf.cn/gtyzmuaboa.html

C#:   while (i < 10) { i++; }
来源：http://hz.yj20258888.top/gtudfjvrus.html

[B08] do-while（至少执行一次）
来源：http://hz.yuxming.cn/gtbtzpzjab.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hongshengwenyu.top/gtghakiacw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhixingplan.top/gtlknrvjzh.html

JS:   do { i++; } while (i < 10);
来源：http://hz.aibaodan.cn/gtaoemiqca.html

TS:   do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtiurebcox.html

Java: do { i++; } while (i < 10);
来源：http://hz.sufxvd.cn/gtwkwepxfa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.birdmap.top/gtninyxysf.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.tanke756.top/gtivbsxrti.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xingfuxueyuan.xyz/gtolfxgmxd.html

[B09] break 与 continue
来源：http://hz.yanxiufei.cn/gtqopmgwsl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.chenzaomai.com/gtlhfxudch.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.guowangkeji.top/gtphgxsidw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj202588.top/gtrvaxakpn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gtohwmsimo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gtjzwkrctv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.andypj.xyz/gtrtvmqdvj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hongshengwenyu.top/gtcfhrrsoo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gtjscjdrek.html

[B10] 遍历同时拿索引
来源：http://hz.guowangkeji.top/gtvesdrsip.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ehwqpu.com/gtokemvwtq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zdqjudy.top/gtnmdxrutr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shuidangran.top/gtvqzinusj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.andypj.xyz/gtvgkulngp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xuetiantiany.cn/gtodkujhfy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj20258888.top/gttjbmmiwb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jiagoushi.top/gtvqgbxsnx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhaomingkeji.xyz/gtnvqkfklo.html

[B11] 生成数字序列 / 区间
来源：http://hz.tianlin.xyz/gtayvcakgn.html

Py:   list(range(0, 10, 2))
来源：http://hz.snrcjt.cn/gtzvmnjibq.html

PHP:  range(0, 10, 2);
来源：http://hz.aizwys.cn/gttrmqifyw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cheryme.top/gtqevogvfc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tian-w.cn/gtfjiwqqwp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ybcxt.top/gtjdaqiemd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.iojbl.cn/gtwzafdenr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.aibaodan.cn/gtkzqbwrdo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xylfe.cn/gtnrkodujb.html

[B12] 跳出多层循环
来源：http://hz.ivvv.top/gtslehvmrz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yj20258.top/gtjnydsusf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jqgufenzy.top/gtuhkyhfla.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jlsjyb.cn/gtnrzfkiqy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangdashe.top/gtafrwxtos.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtnsdsgvnx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.redwolf501.top/gttpnsbdur.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.52xcode.cn/gtziksbkea.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cashguo.top/gtukpazzfq.html

[B13] 判断是否为数字
来源：http://hz.tianlin.xyz/gtipotvnap.html

Py:   isinstance(x, (int, float))
来源：http://hz.cdnleiting.top/gtbrmewmvj.html

PHP:  is_numeric($x)
来源：http://hz.yongpay.top/gtjpjvqjzh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.havefunace.top/gtljmwbzpn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.havefunace.top/gtxspioulx.html

Java: x instanceof Number
来源：http://hz.hnxiangtu.top/gtdpehsxqn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhixingplan.top/gtlgsiasks.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shzxlz.cn/gthxbojwyt.html

C#:   x is int or double or decimal
来源：http://hz.ywan-chungtsiang.top/gtfcbwlxos.html

[B14] 判断值是否在集合内
来源：http://hz.sysykeji.top/gtirbhifvg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.smart0.xyz/gtbywppxft.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jqgfzy.top/gtwylhossf.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.chenlongwang.top/gtxgvbovsp.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ydzc1.top/gttxqaqmko.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cheryme.top/gtbpckoppe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cqqwz.cn/gtillppfdm.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.iojbl.cn/gtmaiwgufx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.dashuyun.cn/gtjoizalrv.html

[B15] 布尔运算与取反
来源：http://hz.yvedp.cn/gtmuxyoixq.html

Py:   a and b or not c
来源：http://hz.hongshengwenyu.top/gtdjvyqhlz.html

PHP:  $a && $b || !$c
来源：http://hz.sufxvd.cn/gtxhpzrbzq.html

JS:   a && b || !c
来源：http://hz.nanxuanxn.top/gtgwaltnxw.html

TS:   a && b || !c
来源：http://hz.tanke756.top/gtbovvpfwu.html

Java: a && b || !c
来源：http://hz.jinghuilouyu.cn/gtzcyfuvbr.html

Go:   a && b || !c
来源：http://hz.nwbrower.top/gtagvijacj.html

Ruby: a && b || !c
来源：http://hz.vqdsnc.cn/gtljvanzkb.html

C#:   a && b || !c
来源：http://hz.daria6918.cn/gtzfemaldq.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.daxiang520.top/gtgeoimlgy.html

Py:   if not data: return
来源：http://hz.zhengqikj.top/gtyltinubj.html

PHP:  if (!$data) { return; }
来源：http://hz.316326.xyz/gtgdwxvzan.html

JS:   if (!data) return;
来源：http://hz.feifeiyinyue.top/gtukyzunal.html

TS:   if (!data) return;
来源：http://hz.guannengcc.top/gtqkdbmati.html

Java: if (data == null) return;
来源：http://hz.shuidangran.top/gtlkpxxjau.html

Go:   if data == nil { return }
来源：http://hz.cqqwz.cn/gtlinvjrjp.html

Ruby: return if data.nil?
来源：http://hz.andypj.xyz/gtqepzatym.html

C#:   if (data == null) return;
来源：http://hz.shzxlz.cn/gtfsogqxzg.html

================================================================================
来源：http://hz.meibo888.top/gtorrmgfpe.html

C. 函数与作用域
来源：http://hz.yuanzhike.top/gtquitwujw.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvpuijiyn.html

[C01] 定义函数
来源：http://hz.hnqzz.top/gtuzspvcro.html

Py:   def add(a, b): return a + b
来源：http://hz.andypj.xyz/gthqibroub.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangkeji.top/gtumymrgrd.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xylfe.cn/gttlcdxaio.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.iojbl.cn/gtlgpdpolh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtpecjlkud.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jiagoushi.top/gtuagblkuk.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xingfuxueyuan.xyz/gtmlnfeowy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtsgichhqu.html

[C02] 默认参数
来源：http://hz.ydjk.org.cn/gtrrcnvhps.html

Py:   def greet(name="World"): return name
来源：http://hz.cdnleiting.top/gtxcgmtzzp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.guannengcc.top/gtkldavaqp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xinyue.icu/gtacmapvto.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sweek.top/gtsbatqtoi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jlsjyb.cn/gtiwchspbb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hywenlv.cn/gtephgjsxk.html

Ruby: def greet(name = "World") = name
来源：http://hz.meibo888.top/gtawmsvmky.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jqgfzy.top/gtbzldpvas.html

[C03] 可变参数
来源：http://hz.wangshuangyany.cn/gtoskxlhxk.html

Py:   def total(*args): return sum(args)
来源：http://hz.jyoumei.cn/gtxlkolphv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhiwuduotai.top/gtfjqhjnkb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daria6918.cn/gtdkftsdgk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj20258888.top/gtczmunxla.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jqgfzy.top/gtkmjkndsq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cheryme.top/gtsrublymh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinqigufen.top/gtfimxpvcj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hywenlv.cn/gtctsavygn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gaohongyu789.top/gtnolqsywf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shangyingyoupin.top/gtvgecbmaq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.daxiang520.top/gtsnukcbdo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zdqjudy.top/gtxvswhwdw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.guannengcc.top/gtjibrzxpm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xuetiantiany.cn/gtyvuxuqdb.html

Go:   // 无：用配置结构体参数
来源：http://hz.quarkkingdee.top/gtulfismqn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtouardxml.html

C#:   f(a: 1, b: 2)
来源：http://hz.tanke756.top/gtaiiafpab.html

[C05] 返回多个值
来源：http://hz.hnxiangtu.top/gtytrovblk.html

Py:   return a, b
来源：http://hz.zhoulong.xyz/gtccljwrlp.html

PHP:  return [$a, $b];
来源：http://hz.shzxlz.cn/gtwjouxpvt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.iojbl.cn/gtodoqmunk.html

TS:   return { a, b };
来源：http://hz.shzxlz.cn/gtfoutkmta.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nwbrower.top/gttuasnixv.html

Go:   return a, b
来源：http://hz.xinyue.icu/gtombtwjnc.html

Ruby: return a, b
来源：http://hz.yj202588.top/gtrtfglqmk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.nanxuanxn.top/gtlyrxjqpu.html

[C06] 匿名函数 / lambda
来源：http://hz.ywan-chungtsiang.top/gtfccuzqct.html

Py:   square = lambda x: x * x
来源：http://hz.xylfe.cn/gtosmchaod.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shangyingyoupin.top/gtgvcpandr.html

JS:   const square = x => x * x;
来源：http://hz.jyoumei.cn/gtanjjstdm.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinghuilouyu.cn/gtjhcmmtme.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.pengpengdd.cyou/gtijcrxxhk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinghuilouyu.cn/gtypfghkrf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.kuanghao11.cn/gtnrckzuno.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xylfe.cn/gtpqqngort.html

[C07] 把函数作为参数传入
来源：http://hz.jqgfzy.top/gtczbqbetn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xingfuxueyuan.xyz/gtsjccbxib.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.0kj1m.cn/gtwhocflyp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nanxinkj.top/gtjltswuow.html

TS:   arr.map(String)
来源：http://hz.hfpthk.cn/gtlpnllnwj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.quarkkingdee.top/gtstvxjads.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenjidiqi.icu/gtimqsblfq.html

Ruby: arr.map(&:upcase)
来源：http://hz.jianghu66.top/gtjeylqiae.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhixingplan.top/gtckmnjkse.html

[C08] 闭包
来源：http://hz.jinyuanbaomall.cn/gtjmkthzwb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.meibo888.top/gtjsezjclt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhijiandao.cn/gttwlwxrbo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gtrrozxufw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtofczgwit.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ivvv.top/gtzfgxnivo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.dashuyun.cn/gtepybneur.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shuidangran.top/gtktylexqy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hywenlv.cn/gtewlewqjx.html

[C09] 递归
来源：http://hz.shanyushiyangkeji.top/gtobzrakbv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gtbvsmvayn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.pengpengdd.cyou/gtbdktdqux.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuetiantiany.cn/gtslvtddlm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtuqcybhvv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.0kj1m.cn/gtrgvimveq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cashguo.top/gtjsmqyddn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xinyue.icu/gtnddurdks.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydjk.org.cn/gtpuzojsjy.html

[C10] 变量作用域
来源：http://hz.hywenlv.cn/gtzwwzixok.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jyoumei.cn/gtsjvsehuw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sysykeji.top/gttdkpadtj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ybcxt.top/gtnjpxjzvp.html

TS:   同 JS
来源：http://hz.yueranfly.top/gteowifnmb.html

Java: 方法内为块级作用域
来源：http://hz.hysaishi.cn/gtzlpiftkh.html

Go:   花括号块级作用域
来源：http://hz.xziqi.cn/gtovynknwk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.iojbl.cn/gtoxcxjhir.html

C#:   块级作用域
来源：http://hz.pycfn.com/gtemnqbzgb.html

[C11] 模块导入与导出
来源：http://hz.shangyingyoupin.top/gtoqmccbbc.html

Py:   from module import func
来源：http://hz.shzxlz.cn/gtglhvlkhg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hammf.cn/gtvmqnbwej.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tanke756.top/gtjhkvkgdc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ywan-chungtsiang.top/gtikgcutyv.html

Java: import java.util.List;
来源：http://hz.sxryk.cn/gtgsyudlot.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.haohaochexian.top/gtoahnynzu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.gotoacloud.top/gtupeckuqf.html

C#:   using System.Text;
来源：http://hz.ivvv.top/gttsvjrabs.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuanzhike.top/gtijedjoks.html

Py:   (lambda: print("run"))()
来源：http://hz.hysaishi.cn/gttlvenzvs.html

PHP:  (function () { echo "run"; })();
来源：http://hz.iojbl.cn/gtxvxywlye.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sxryk.cn/gtuupukhge.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xylfe.cn/gtsszeheia.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgfzy.top/gtahwmwsgt.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hongshengwenyu.top/gtwiquxryv.html

Ruby: -> { puts "run" }.call
来源：http://hz.sufxvd.cn/gtqykqfrvp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinghuilouyu.cn/gttkfdjyhm.html

[C13] 类型声明 / 类型注解
来源：http://hz.wangdashe.top/gtvqwsbehm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aibaodan.cn/gtebuwrjri.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtztmbbchk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xylfe.cn/gttqkaitqg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinghuilouyu.cn/gthhnceczr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.havefunace.top/gtcujbetza.html

Go:   func add(a, b int) int
来源：http://hz.fzhhl.top/gtwzkebfuu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhongyouzk.top/gtmefxfmop.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.bjfxy.top/gtvqtcwqiu.html

[C14] 泛型函数
来源：http://hz.nwbrower.top/gtudvxehgg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yuanzhike.top/gtdcmlsdwv.html

PHP:  // 无泛型
来源：http://hz.zhoulong.xyz/gtzymmpebh.html

JS:   // 无泛型
来源：http://hz.sufxvd.cn/gtgginfgaf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.nanxuanxn.top/gtidnskomi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xziqi.cn/gtoewlysin.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cdnleiting.top/gtgmfaejxf.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangkeji.top/gtoloptuif.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.nanxuanxn.top/gtmesybwxz.html

[C15] 解构 / 展开参数
来源：http://hz.yangfankeji.com/gtcccbvets.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.feifeiyinyue.top/gtsgbiyxwx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nanxuanxn.top/gtioazlnmr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yueranfly.top/gtkrgrzdou.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hnqzz.top/gttdswtief.html

Java: // 无解构
来源：http://hz.redwolf501.top/gtlsifpsvw.html

Go:   // 无解构
来源：http://hz.sweek.top/gtqhfgkbaw.html

Ruby: a, b = pair
来源：http://hz.yongpay.top/gtenxtjwys.html

C#:   var (a, b) = pair;
来源：http://hz.nanxuanxn.top/gtpsqulvyi.html

[C16] 函数 / 方法重载
来源：http://hz.xylfe.cn/gtiqvborlh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jiagoushi.top/gthuakhagd.html

PHP:  // 无重载
来源：http://hz.nanxuanxn.top/gtdtqgvgvm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xinyue.icu/gteabdjzws.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yueranfly.top/gtfclhrgcx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhongyouzk.top/gtvupzjmsr.html


<!-- 参考信息 -->