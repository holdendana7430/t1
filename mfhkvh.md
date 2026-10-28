代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://hz.zhiwuduotai.top/gtusywvizy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.zycfv.cn/gthlvzlmwl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhaomingkeji.xyz/gtjmdztjhw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shangyingyoupin.top/gtpomrivkk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.meibo888.top/gtmxzqndjx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.sysykeji.top/gthknlyaym.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.gzhubu.top/gtwydzjtfq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.sufxvd.cn/gtmbmlgymn.html

[A26] 类型转换总览
来源：http://hz.shuidangran.top/gtzaajvzrz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.shanyushiyangkeji.top/gtmadyxnus.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.pycfn.com/gtesyhcgip.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ywan-chungtsiang.top/gtbjdzkpxg.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zdqjudy.top/gthzezqmzs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.cheryme.top/gtnluwgsrv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jlsjyb.cn/gttspcqkrc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.zhijiandao.cn/gtexmoosfo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.cucudq.cn/gteyuiuvvx.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtxjscoikt.html

B. 流程控制
来源：http://hz.nanxuanxn.top/gtkkxduiwl.html

================================================================================
来源：http://hz.jiagoushi.top/gtakscbnvp.html

[B01] 条件判断 if / else
来源：http://hz.ybcxt.top/gtqxsexzlv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.shanyushiyangtech.top/gtrfssqvoo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.hysaishi.cn/gtxhzspycr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tian-w.cn/gtqtaslgtw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhoulong.xyz/gtmxecqeyw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.ydjk.org.cn/gtrgigekpi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ydjk.org.cn/gtnxbnbtkw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.c1oappe.top/gtedhpzhke.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.52xcode.cn/gtnlpodloe.html

[B02] 多分支 else if / elif
来源：http://hz.9152youxi.cn/gtpfmiguqb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yj20258888.top/gtcgdemlws.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.wangshuangyany.cn/gtisfxrcod.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gogol.net.cn/gtskgtotct.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hnqzz.top/gtabuqobtg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hysaishi.cn/gtomphrdcs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xylfe.cn/gtkgznjzzp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.sweek.top/gtfhjlrdup.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuanzhike.top/gtznnfcdvu.html

[B03] switch / match / case
来源：http://hz.yuxming.cn/gtsxcnuoam.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.ybcxt.top/gtxxmebplp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yonumen.top/gtnhgwnlxi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.daria6918.cn/gtpmlrfzvq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.0kj1m.cn/gtbfzliwaz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jyoumei.cn/gtvlbvztdt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.havefunace.top/gtggdeuftt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ydjk.org.cn/gtpyothjav.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.xuanzx.com/gtjezeqlly.html

[B04] for 计数循环
来源：http://hz.hongshengwenyu.top/gtalxmyuri.html

Py:   for i in range(10): print(i)
来源：http://hz.dianchejie.cn/gtltgefftr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.havefunace.top/gtvzrdixzx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cheryme.top/gtkwardizx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.0kj1m.cn/gtlxmdzjmq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yj20258888.top/gtcbfngyfk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.meibo888.top/gttcgombzw.html

Ruby: 10.times { |i| puts i }
来源：http://hz.cdnleiting.top/gtggdbswgf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.nwbrower.top/gtoruthrsn.html

[B05] 遍历数组 / 列表
来源：http://hz.xingfuxueyuan.xyz/gtskapbtdd.html

Py:   for item in arr: print(item)
来源：http://hz.cqqwz.cn/gtyznftbrk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.xylfe.cn/gtrcvtezyc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.pengpengdd.cyou/gtovwydbwt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.feifeiyinyue.top/gtltyvrzxj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.nanxuanxn.top/gtmxwmgwjn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinqigfzy.top/gtiaqwhzet.html

Ruby: arr.each { |item| puts item }
来源：http://hz.hammf.cn/gteijpfjcs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.sysykeji.top/gtkyupubcu.html

[B06] 遍历字典 / 对象
来源：http://hz.sxryk.cn/gtnaqopiuc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.daria6918.cn/gtlyfsgnkb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.nanxinkj.top/gteufnwisx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cucudq.cn/gtltjnznaz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cdnleiting.top/gtxslbwjqj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.smart0.xyz/gtuvrzmtxg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.gzhubu.top/gttwfehark.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xinyue.icu/gtqdwhiewe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jinqigufen.top/gtnmmptpsp.html

[B07] while 循环
来源：http://hz.chenlongwang.top/gtsgwqozly.html

Py:   while i < 10: i += 1
来源：http://hz.jinyuanbaomall.cn/gtzockuzux.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yuxming.cn/gttictitsl.html

JS:   while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gttibnwgtc.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtwkfdyyiu.html

Java: while (i < 10) { i++; }
来源：http://hz.yj202588.top/gtvdlxuqlh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ybcxt.top/gtjquvtiqp.html

Ruby: while i < 10; i += 1; end
来源：http://hz.quarkkingdee.top/gtgrauazlv.html

C#:   while (i < 10) { i++; }
来源：http://hz.meibo888.top/gtmwgqmxnu.html

[B08] do-while（至少执行一次）
来源：http://hz.sysykeji.top/gtsmllmiza.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hywenlv.cn/gtpcdelcny.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.chenlongwang.top/gtblxbgapf.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hnqzz.top/gttrxqigxe.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj20258.top/gtubihvgjy.html

Java: do { i++; } while (i < 10);
来源：http://hz.mhx1999.top/gtskorrjgl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.wangshuangyany.cn/gtqsztfyhb.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.gaohongyu789.top/gtsjqgwuvv.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shzxlz.cn/gtdeqtwbbn.html

[B09] break 与 continue
来源：http://hz.sysykeji.top/gtrfzdssku.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yvedp.cn/gtdzrvgmcg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtncadtgsc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtfheewhgp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtbdeuxatz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zdqjudy.top/gtngojsicy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.pengpengdd.cyou/gtqqbkqrot.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cucudq.cn/gteofaligt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.andypj.xyz/gtfnbfaqor.html

[B10] 遍历同时拿索引
来源：http://hz.jianghu66.top/gthnqembwk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hongshengwenyu.top/gteipoypnn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.daria6918.cn/gtrwmflmsv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.nanxuanxn.top/gtheirzgxt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.feifeiyinyue.top/gtqtyhjpdr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.havefunace.top/gtaviqtsns.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jqgufenzy.top/gtsaubthju.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.meibo888.top/gtyqyjlmij.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhixingplan.top/gtnskztqwz.html

[B11] 生成数字序列 / 区间
来源：http://hz.xuanzx.com/gtisjkmlwq.html

Py:   list(range(0, 10, 2))
来源：http://hz.jlsjyb.cn/gthaskjung.html

PHP:  range(0, 10, 2);
来源：http://hz.tianlin.xyz/gtvsewtoho.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.0kj1m.cn/gtclgwprqh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenzaomai.com/gtxygzgybh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hysaishi.cn/gtsirpokdt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gogol.net.cn/gtxkuddsju.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jqgfzy.top/gtrqhdclmp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.cdnleiting.top/gtzuhvbtip.html

[B12] 跳出多层循环
来源：http://hz.yonumen.top/gtjizrrrht.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.birdmap.top/gtixbelriz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jinghuilouyu.cn/gtgjgtnqsy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenjidiqi.icu/gtnmwdnygd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.316326.xyz/gtnaujwgii.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gtnwmixsoz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.meibo888.top/gtohrpmntu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.tian-w.cn/gtlbunijhf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.daxiang520.top/gtbqifhzap.html

[B13] 判断是否为数字
来源：http://hz.yongpay.top/gtjfcmsqza.html

Py:   isinstance(x, (int, float))
来源：http://hz.mhx1999.top/gtftcqprfk.html

PHP:  is_numeric($x)
来源：http://hz.jqgufenzy.top/gtpaielbmd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shzxlz.cn/gtqteyzfpv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.andypj.xyz/gtolylqphb.html

Java: x instanceof Number
来源：http://hz.xinyue.icu/gtcvqadfkq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yj20258888.top/gtbwhbtkqd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.0kj1m.cn/gtwqunhkee.html

C#:   x is int or double or decimal
来源：http://hz.52xcode.cn/gtgggyslfv.html

[B14] 判断值是否在集合内
来源：http://hz.yvedp.cn/gtyxztoeyk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cheryme.top/gtgywlaefh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zdqjudy.top/gtrupmivef.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gotoacloud.top/gtuobfgkma.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ydzc1.top/gtymqghsxt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yvedp.cn/gtsbiaqtcc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.meibo888.top/gtvmnpdeqm.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.chenjidiqi.icu/gtzbtlievx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.nanxinkj.top/gtbyctonhi.html

[B15] 布尔运算与取反
来源：http://hz.hongshengwenyu.top/gtrdvlnflm.html

Py:   a and b or not c
来源：http://hz.yueranfly.top/gtcennotkj.html

PHP:  $a && $b || !$c
来源：http://hz.dianchejie.cn/gtkrawfyep.html

JS:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtgnxnoffk.html

TS:   a && b || !c
来源：http://hz.cashguo.top/gthplcmkcx.html

Java: a && b || !c
来源：http://hz.gaohongyu789.top/gtnguxfijj.html

Go:   a && b || !c
来源：http://hz.daria6918.cn/gturmdmnif.html

Ruby: a && b || !c
来源：http://hz.yvedp.cn/gtziohxjjv.html

C#:   a && b || !c
来源：http://hz.c1oappe.top/gthcgdjvko.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.vqdsnc.cn/gttkdwccvu.html

Py:   if not data: return
来源：http://hz.xinyue.icu/gtvhyvcsak.html

PHP:  if (!$data) { return; }
来源：http://hz.jlsjyb.cn/gtdfeeuskv.html

JS:   if (!data) return;
来源：http://hz.hnqzz.top/gttymkdujb.html

TS:   if (!data) return;
来源：http://hz.cheryme.top/gtztutepgy.html

Java: if (data == null) return;
来源：http://hz.sweek.top/gtispiibbf.html

Go:   if data == nil { return }
来源：http://hz.iojbl.cn/gthryrdjdx.html

Ruby: return if data.nil?
来源：http://hz.ivvv.top/gtyblkahxv.html

C#:   if (data == null) return;
来源：http://hz.yueranfly.top/gtoyphxlxr.html

================================================================================
来源：http://hz.iojbl.cn/gtfegfkdki.html

C. 函数与作用域
来源：http://hz.chenjidiqi.icu/gtuwutinuu.html

================================================================================
来源：http://hz.shzxlz.cn/gtljuifjvp.html

[C01] 定义函数
来源：http://hz.ivvv.top/gtvkqirtvr.html

Py:   def add(a, b): return a + b
来源：http://hz.0kj1m.cn/gttmszwauq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gtkakitzsp.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtjpwpsrvt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sysykeji.top/gtrfuhmhjc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ivvv.top/gtqoohfzzd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shuidangran.top/gtpijzudou.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gaohongyu789.top/gtfwmnmulj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtjadeygqv.html

[C02] 默认参数
来源：http://hz.sysykeji.top/gtzvjaervq.html

Py:   def greet(name="World"): return name
来源：http://hz.yanxiufei.cn/gteuxiobob.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sysykeji.top/gthoczutfk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.havefunace.top/gtdppbofrm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.aizwys.cn/gthkxqebvq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ppjwa.cn/gtioddqodx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.9152youxi.cn/gtikflwpos.html

Ruby: def greet(name = "World") = name
来源：http://hz.yvedp.cn/gtjfaqjtet.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gotoacloud.top/gtwiqabgzo.html

[C03] 可变参数
来源：http://hz.havefunace.top/gtntcruvkj.html

Py:   def total(*args): return sum(args)
来源：http://hz.havefunace.top/gtqcydhwdx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sysykeji.top/gttspnvntq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zycfv.cn/gtizkozglp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhijiandao.cn/gtgctgpmje.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yongpay.top/gtrhimsras.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.dashuyun.cn/gtqiafggak.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xingfuxueyuan.xyz/gtjsabkfzo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yuxming.cn/gtfqnwhswd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xingfuxueyuan.xyz/gtncpgrvsz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.gzhubu.top/gtjwrrixaa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.fzhhl.top/gtxoovsroa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.52xcode.cn/gtxwxtoeug.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.nanxinkj.top/gthzsqpwad.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhiwuduotai.top/gtsmzxgvxh.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhengqikj.top/gtrfzxejgp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hongshengwenyu.top/gtnuezoqcu.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinqigufen.top/gtoxjdmvfw.html

[C05] 返回多个值
来源：http://hz.jinyuanbaomall.cn/gtdimqwajm.html

Py:   return a, b
来源：http://hz.yangfankeji.com/gtnljdlblu.html

PHP:  return [$a, $b];
来源：http://hz.ppjwa.cn/gtcagpufli.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shanyushiyangtech.top/gtleawhlxp.html

TS:   return { a, b };
来源：http://hz.havefunace.top/gtcmtfsfta.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yonumen.top/gtgiscpkwc.html

Go:   return a, b
来源：http://hz.yongpay.top/gtpqolfzvv.html

Ruby: return a, b
来源：http://hz.xziqi.cn/gthnxduitc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnxiangtu.top/gtmqymqpts.html

[C06] 匿名函数 / lambda
来源：http://hz.jqgufenzy.top/gtuswagvdj.html

Py:   square = lambda x: x * x
来源：http://hz.chenlongwang.top/gtgaijkkof.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.guannengcc.top/gtotmjcbhz.html

JS:   const square = x => x * x;
来源：http://hz.yanxiufei.cn/gtuqrcuxoc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shangyingyoupin.top/gtajbqwwfx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.snrcjt.cn/gttjqdzpwa.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jqgfzy.top/gtgpbxgijc.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hysaishi.cn/gthovoefmz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zdqjudy.top/gtaydjajmn.html

[C07] 把函数作为参数传入
来源：http://hz.jinghuilouyu.cn/gtmpwwipyf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.9152youxi.cn/gtbploiype.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guannengcc.top/gteiluqjhr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinqigufen.top/gtjygohika.html

TS:   arr.map(String)
来源：http://hz.nwbrower.top/gtcghapegw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhijiandao.cn/gtbdhvgmjd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.aizwys.cn/gtoxdhsfkx.html

Ruby: arr.map(&:upcase)
来源：http://hz.yanxiufei.cn/gtaytxbutc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.chenlongwang.top/gtgtwydrtw.html

[C08] 闭包
来源：http://hz.yangfankeji.com/gtnnpnavnr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.dashuyun.cn/gtxpaoyiwc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ybcxt.top/gtqgammsin.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.wangshuangyany.cn/gtbvyfoooj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtmrnrhdsd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yvedp.cn/gtveqolcqt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.snrcjt.cn/gtkqpaxtme.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hywenlv.cn/gtqhfzudzx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gtdxvebvkl.html

[C09] 递归
来源：http://hz.havefunace.top/gtoxalpqfj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenzaomai.com/gtabghzirw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.nanxinkj.top/gttjyefrnu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gtppkdziss.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhoulong.xyz/gtmlcmcebr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.daria6918.cn/gtzzdolivh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.pycfn.com/gtnzqwnxhr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.svipenyu.cn/gtxwzlstwn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sxryk.cn/gtyafogrma.html

[C10] 变量作用域
来源：http://hz.mhx1999.top/gtdohnmnlv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hywenlv.cn/gtxchhkipp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yvedp.cn/gtptjqvlmp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.quarkkingdee.top/gtjachlrcf.html

TS:   同 JS
来源：http://hz.hnxiangtu.top/gttkgwlsjj.html

Java: 方法内为块级作用域
来源：http://hz.feifeiyinyue.top/gtrbgimznt.html

Go:   花括号块级作用域
来源：http://hz.hywenlv.cn/gtrxullfqh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.iojbl.cn/gtoqqdkkrh.html

C#:   块级作用域
来源：http://hz.bjfxy.top/gtgzlbzmcx.html

[C11] 模块导入与导出
来源：http://hz.jqgufenzy.top/gtnyuqnofg.html

Py:   from module import func
来源：http://hz.shzxlz.cn/gtsfsazhhf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xuetiantiany.cn/gtengenmdq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.52xcode.cn/gtzdyxsbjj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hywenlv.cn/gtxckhyeps.html

Java: import java.util.List;
来源：http://hz.yvedp.cn/gtbtkrsaym.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.aizwys.cn/gtsveijmbm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xuetiantiany.cn/gtprwjzvzj.html

C#:   using System.Text;
来源：http://hz.xuanzx.com/gtuypryqhl.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuxming.cn/gthyujzohq.html

Py:   (lambda: print("run"))()
来源：http://hz.iojbl.cn/gtxaczrdoo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.pycfn.com/gtnkvbwvfu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hfpthk.cn/gtjgwypddq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtsuxqcrer.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xuanzx.com/gtlhsbozkh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jinqigfzy.top/gtexpsnlzo.html

Ruby: -> { puts "run" }.call
来源：http://hz.xingfuxueyuan.xyz/gtpyuzgdbb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.iojbl.cn/gtgkdufvmh.html

[C13] 类型声明 / 类型注解
来源：http://hz.sufxvd.cn/gtefhcidbb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xziqi.cn/gtuwjdzsky.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gtzbclellf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nwbrower.top/gtmgraqnnp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhiwuduotai.top/gtursakfgc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtqirevzvw.html

Go:   func add(a, b int) int
来源：http://hz.xuetiantiany.cn/gtueifhkyg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.svipenyu.cn/gtfdzfkfyh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinghuilouyu.cn/gtaoxjwhqj.html

[C14] 泛型函数
来源：http://hz.yueranfly.top/gttyudlrry.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.redwolf501.top/gtzktydydr.html

PHP:  // 无泛型
来源：http://hz.daria6918.cn/gtqshxqdvg.html

JS:   // 无泛型
来源：http://hz.sxryk.cn/gtunjgmsis.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhijiandao.cn/gtfaupoqvd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.birdmap.top/gtkssftxqu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinqigufen.top/gtusdgedsp.html

Ruby: # 无泛型
来源：http://hz.hongshengwenyu.top/gttkpmvals.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhijiandao.cn/gtorqtdiaf.html

[C15] 解构 / 展开参数
来源：http://hz.xuanzx.com/gtxseaoyoy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gaohongyu789.top/gtecszmcex.html

PHP:  [$a, $b] = $pair;
来源：http://hz.daxiang520.top/gtzobjtoft.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shuidangran.top/gtbnbrjrmj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shuidangran.top/gtbejhptqb.html

Java: // 无解构
来源：http://hz.c1oappe.top/gtmgquzkxp.html

Go:   // 无解构
来源：http://hz.yj20258888.top/gtlbllqwld.html


<!-- 参考信息 -->