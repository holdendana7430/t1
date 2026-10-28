代发 wailian999

[A26] 类型转换总览
来源：http://hz.ppjwa.cn/gtfyaddeiv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.dianchejie.cn/gtysimjzqk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.hammf.cn/gtkcwwnfad.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jiagoushi.top/gtlhfrlmcl.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yangfankeji.com/gtxgwtxtlz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhaomingkeji.xyz/gtfqleiryl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yj20258888.top/gtyjsnnhcr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.aizwys.cn/gtqfjsnrne.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.9152youxi.cn/gtxfevlwaw.html

================================================================================
来源：http://hz.cucudq.cn/gtecivttgp.html

B. 流程控制
来源：http://hz.ydzc1.top/gtgsjnlkzt.html

================================================================================
来源：http://hz.zhoulong.xyz/gtyvutcwcc.html

[B01] 条件判断 if / else
来源：http://hz.gogol.net.cn/gtgraeicmz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.pengpengdd.cyou/gttwwruruj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.guannengcc.top/gtqtaqwhrj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.guowangkeji.top/gtsgakihuu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.nanxuanxn.top/gtifdencsy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hnxiangtu.top/gtqtwwvxwl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.nwbrower.top/gteyyvegxh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.vqdsnc.cn/gtmevwpoub.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.smart0.xyz/gtfapaddlg.html

[B02] 多分支 else if / elif
来源：http://hz.xziqi.cn/gtvbbhpomp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yj20258.top/gtqvzvkrgz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.tian-w.cn/gtuyvbuewa.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ppjwa.cn/gtqxwqcdea.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yangfankeji.com/gthjhreoyy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtimflpeyf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.hammf.cn/gthrxoacsm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.sxryk.cn/gtmxtoujdr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gzhubu.top/gtnptpfpxi.html

[B03] switch / match / case
来源：http://hz.vqdsnc.cn/gtjspoeedq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.cashguo.top/gtsxxkmftq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.shangyingyoupin.top/gtnpijxbpd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.c1oappe.top/gtfwtsujof.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xuetiantiany.cn/gtyeezkqjn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jinqigufen.top/gtesgqrgen.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.havefunace.top/gtvqjiwqdw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.iojbl.cn/gtpilbbjtn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ivvv.top/gtxfwkpaeb.html

[B04] for 计数循环
来源：http://hz.dashuyun.cn/gtmiidgiwd.html

Py:   for i in range(10): print(i)
来源：http://hz.ppjwa.cn/gtdubdkule.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.gotoacloud.top/gtgqvfqhqj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.9152youxi.cn/gtdfykyjdu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinghuilouyu.cn/gtgtxxzshj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.gaohongyu789.top/gtpyguowca.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.xingfuxueyuan.xyz/gtmvusyswk.html

Ruby: 10.times { |i| puts i }
来源：http://hz.chenzaomai.com/gtdsvoovtk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ybcxt.top/gtgqsuxvdw.html

[B05] 遍历数组 / 列表
来源：http://hz.aizwys.cn/gtqozrycpw.html

Py:   for item in arr: print(item)
来源：http://hz.jqgufenzy.top/gtmiqbjgpw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.gogol.net.cn/gtfxoxpnow.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ydjk.org.cn/gtkppuvxgb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jqgfzy.top/gtiggqcznc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xylfe.cn/gtugoqfykh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinyuanbaomall.cn/gtisgqswjb.html

Ruby: arr.each { |item| puts item }
来源：http://hz.sysykeji.top/gteevppfby.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhixingplan.top/gthtegkfoe.html

[B06] 遍历字典 / 对象
来源：http://hz.bjfxy.top/gtcivwuxek.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ehwqpu.com/gtymirdinx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xinyue.icu/gtyzgrrpxz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xuetiantiany.cn/gtmkvjccgn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yueranfly.top/gtfmstfekk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.9152youxi.cn/gtsewedggq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.kuanghao11.cn/gtwkzstlhn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.feifeiyinyue.top/gthpjpajeu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jlsjyb.cn/gtmxmcodye.html

[B07] while 循环
来源：http://hz.sufxvd.cn/gtrcwjbkkt.html

Py:   while i < 10: i += 1
来源：http://hz.ywan-chungtsiang.top/gtwdkqrbdx.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jinqigufen.top/gtnusancil.html

JS:   while (i < 10) { i++; }
来源：http://hz.bjfxy.top/gtfbbkeewr.html

TS:   while (i < 10) { i++; }
来源：http://hz.wangdashe.top/gtighnctzr.html

Java: while (i < 10) { i++; }
来源：http://hz.tianlin.xyz/gttcxmxtem.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.9152youxi.cn/gtvbfmxufy.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yuanzhike.top/gtpqazxuby.html

C#:   while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gtquiuffqb.html

[B08] do-while（至少执行一次）
来源：http://hz.tianlin.xyz/gtgmmwytnj.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jyoumei.cn/gtzjegegtt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhaomingkeji.xyz/gtwpsssubh.html

JS:   do { i++; } while (i < 10);
来源：http://hz.iojbl.cn/gtafjzfpsf.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jyoumei.cn/gtoyrwecjg.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gtysfgktvz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hongshengwenyu.top/gtnnqooufi.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ydjk.org.cn/gtxjuzkwyr.html

C#:   do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gtkcjxlauw.html

[B09] break 与 continue
来源：http://hz.jiagoushi.top/gtdzehpwvu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.pycfn.com/gtqxbcaaek.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.iojbl.cn/gtzycohanc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zdqjudy.top/gtdakyiixo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gtkgaatcfx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daria6918.cn/gticdvfiko.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yj20258888.top/gtghjvqmyy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ydzc1.top/gtofwsqvwi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fzhhl.top/gtwxqmcyvr.html

[B10] 遍历同时拿索引
来源：http://hz.jqgufenzy.top/gtyqvvzmbz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinqigufen.top/gtgmetkpdr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zdqjudy.top/gtctfexmmn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yongpay.top/gtonqhhdfd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hongshengwenyu.top/gtyqbeibte.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shanyushiyangkeji.top/gtxcwlwsfi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yongpay.top/gtmfbpdsos.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.birdmap.top/gtrgmaooku.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.tian-w.cn/gttpkvocbh.html

[B11] 生成数字序列 / 区间
来源：http://hz.yuanzhike.top/gtwdclvbzh.html

Py:   list(range(0, 10, 2))
来源：http://hz.hywenlv.cn/gtrtstzuaz.html

PHP:  range(0, 10, 2);
来源：http://hz.zycfv.cn/gtwfgutjhq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.daxiang520.top/gtmylcyamh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gotoacloud.top/gtgfudkiwp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.9152youxi.cn/gtrfshdqgo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.fzhhl.top/gtuxmodyma.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yueranfly.top/gtjqmiclgm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.gotoacloud.top/gtjflqbttd.html

[B12] 跳出多层循环
来源：http://hz.quarkkingdee.top/gtchskjubp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.9152youxi.cn/gtnqtbejrt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.fzhhl.top/gthturosfk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ppjwa.cn/gtqfhfgnes.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.aibaodan.cn/gtqabpbyaw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangtech.top/gtqbiwkzcp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shzxlz.cn/gtsoiqicki.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jinyuanbaomall.cn/gtyjcukuui.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.haohaochexian.top/gtgstrrisv.html

[B13] 判断是否为数字
来源：http://hz.yuanzhike.top/gtecockybn.html

Py:   isinstance(x, (int, float))
来源：http://hz.iojbl.cn/gtumamoucb.html

PHP:  is_numeric($x)
来源：http://hz.ywan-chungtsiang.top/gthifkzxwi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daxiang520.top/gtkptghkcc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.c1oappe.top/gtkrbokptz.html

Java: x instanceof Number
来源：http://hz.yj20258888.top/gtzvatwudj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.aibaodan.cn/gtnngmxbuq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ppjwa.cn/gttcdyviqy.html

C#:   x is int or double or decimal
来源：http://hz.tanke756.top/gtulygitxm.html

[B14] 判断值是否在集合内
来源：http://hz.gogol.net.cn/gtsooklhsy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yonumen.top/gtsytomqwf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zycfv.cn/gtfsorkehb.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ydjk.org.cn/gtawxzzond.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jyoumei.cn/gttxbhfhum.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xinyue.icu/gtbabxtabo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xuanzx.com/gtnouqxbhl.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gaohongyu789.top/gtozanqljf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenjidiqi.icu/gtuzgurvag.html

[B15] 布尔运算与取反
来源：http://hz.yueranfly.top/gtrtevxjcl.html

Py:   a and b or not c
来源：http://hz.hfpthk.cn/gtjezopaah.html

PHP:  $a && $b || !$c
来源：http://hz.ehwqpu.com/gtekggzedo.html

JS:   a && b || !c
来源：http://hz.jqgufenzy.top/gtzlureayv.html

TS:   a && b || !c
来源：http://hz.vqdsnc.cn/gtguktxben.html

Java: a && b || !c
来源：http://hz.chenjidiqi.icu/gtlmnupcnv.html

Go:   a && b || !c
来源：http://hz.sysykeji.top/gtnnpxnfcn.html

Ruby: a && b || !c
来源：http://hz.fzhhl.top/gtwvwkekas.html

C#:   a && b || !c
来源：http://hz.tanke756.top/gtzcbrihsl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.c1oappe.top/gtyjltibrh.html

Py:   if not data: return
来源：http://hz.hammf.cn/gtzkfoncqf.html

PHP:  if (!$data) { return; }
来源：http://hz.mhx1999.top/gtmyinquit.html

JS:   if (!data) return;
来源：http://hz.shanyushiyangkeji.top/gtugyjbnnz.html

TS:   if (!data) return;
来源：http://hz.zhongyouzk.top/gtvnwlunfs.html

Java: if (data == null) return;
来源：http://hz.shanyushiyangkeji.top/gtmnrlgqeq.html

Go:   if data == nil { return }
来源：http://hz.mhx1999.top/gtxqizugcx.html

Ruby: return if data.nil?
来源：http://hz.gaohongyu789.top/gtaikaulvu.html

C#:   if (data == null) return;
来源：http://hz.nwbrower.top/gtgnmukgvf.html

================================================================================
来源：http://hz.52xcode.cn/gtgpvgwjee.html

C. 函数与作用域
来源：http://hz.jinyuanbaomall.cn/gthidohxjp.html

================================================================================
来源：http://hz.sufxvd.cn/gtugrjzlet.html

[C01] 定义函数
来源：http://hz.316326.xyz/gtuyugqyjl.html

Py:   def add(a, b): return a + b
来源：http://hz.9152youxi.cn/gtplnaocwx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.9152youxi.cn/gtpdaiemkf.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yuxming.cn/gtyffubhti.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtwpfoqbda.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtnlwksgtb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shuidangran.top/gtoacdywgl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ybcxt.top/gtewdqqtdl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtpswvfiuf.html

[C02] 默认参数
来源：http://hz.hnxiangtu.top/gtjvkxfxan.html

Py:   def greet(name="World"): return name
来源：http://hz.0kj1m.cn/gtzhaztbkh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jiagoushi.top/gtwxlswztl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shanyushiyangtech.top/gtnfzizfue.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yvedp.cn/gtgoyvlhjb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sufxvd.cn/gtjgmkcoaj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhiwuduotai.top/gtkpinbeiv.html

Ruby: def greet(name = "World") = name
来源：http://hz.0kj1m.cn/gtosaelbsx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.quarkkingdee.top/gthoxuefaf.html

[C03] 可变参数
来源：http://hz.nwbrower.top/gtuejpyqct.html

Py:   def total(*args): return sum(args)
来源：http://hz.pycfn.com/gtmvlmtmyz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ivvv.top/gtckaupzmp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aibaodan.cn/gtqoosnrpd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nwbrower.top/gtkqiecrhx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinqigufen.top/gtqkawxvmt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sxryk.cn/gtjednpnef.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.chenjidiqi.icu/gtgaxsbijn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ywan-chungtsiang.top/gtldacyxzu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.andypj.xyz/gthdpvwomp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.mhx1999.top/gttgkcumbf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zycfv.cn/gtmhlwuaab.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.redwolf501.top/gtmbbjmdaq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.daxiang520.top/gtiysjyhlq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yuxming.cn/gtsbvsbhyd.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinqigufen.top/gtnvugzfib.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtlikjayiv.html

C#:   f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gtztpjnggw.html

[C05] 返回多个值
来源：http://hz.iojbl.cn/gtqxzoapfj.html

Py:   return a, b
来源：http://hz.zhixingplan.top/gtvzcwqhgo.html

PHP:  return [$a, $b];
来源：http://hz.havefunace.top/gtoksbkaeb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.wangdashe.top/gtkpaevnxw.html

TS:   return { a, b };
来源：http://hz.quarkkingdee.top/gtmznufyrb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinyuanbaomall.cn/gtcbjpzdql.html

Go:   return a, b
来源：http://hz.jinqigfzy.top/gtlimwqadm.html

Ruby: return a, b
来源：http://hz.yanxiufei.cn/gtmajzcsgs.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.tianlin.xyz/gtzutpsxhe.html

[C06] 匿名函数 / lambda
来源：http://hz.vqdsnc.cn/gtzquuqzbf.html

Py:   square = lambda x: x * x
来源：http://hz.cashguo.top/gtqyrllfqk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.9152youxi.cn/gtziefapef.html

JS:   const square = x => x * x;
来源：http://hz.hongshengwenyu.top/gtmetixhfo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhengqikj.top/gtncdadhew.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sysykeji.top/gtwjpvdusf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shangyingyoupin.top/gtohluflqe.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cucudq.cn/gtggdvtjct.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jqgufenzy.top/gtjvcxdhyx.html

[C07] 把函数作为参数传入
来源：http://hz.mhx1999.top/gtjozrqbjp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xinyue.icu/gtdwefwlhq.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guannengcc.top/gtysatydog.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nwbrower.top/gteflpkkqp.html

TS:   arr.map(String)
来源：http://hz.jqgufenzy.top/gthbhdvzlt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.vqdsnc.cn/gtthjloira.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jiagoushi.top/gtevpdivpq.html

Ruby: arr.map(&:upcase)
来源：http://hz.chenzaomai.com/gtcijgbwul.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shangyingyoupin.top/gtyurzbzwr.html

[C08] 闭包
来源：http://hz.c1oappe.top/gtcvfozlyh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.52xcode.cn/gtmoskotfg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hywenlv.cn/gtphgieoif.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtnjscgbvm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sxryk.cn/gtxuezsftw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hywenlv.cn/gtughelloi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jyoumei.cn/gtwwpnvlxk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.wangshuangyany.cn/gtxghahysg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtdlaihyxw.html

[C09] 递归
来源：http://hz.redwolf501.top/gthicsmjjv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nanxinkj.top/gtscbifako.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cucudq.cn/gtjdmzbwwc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.52xcode.cn/gtltmwybuo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgufenzy.top/gtqypbsttr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.fzhhl.top/gtpaezeath.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shangyingyoupin.top/gtdfrbpgvk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dianchejie.cn/gtxapmtmtv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.0kj1m.cn/gtggiwairj.html

[C10] 变量作用域
来源：http://hz.jiagoushi.top/gtahnfynzb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydzc1.top/gtjxlgysga.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ivvv.top/gtpqcsnjyq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.kuanghao11.cn/gtgmgpnhzr.html

TS:   同 JS
来源：http://hz.hongshengwenyu.top/gtpunnzzxp.html

Java: 方法内为块级作用域
来源：http://hz.feifeiyinyue.top/gtfpxoxncp.html

Go:   花括号块级作用域
来源：http://hz.aizwys.cn/gtcjlhnbhl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hammf.cn/gtkgektjfg.html

C#:   块级作用域
来源：http://hz.yvedp.cn/gtsmmrvwam.html

[C11] 模块导入与导出
来源：http://hz.tian-w.cn/gtpyagcusf.html

Py:   from module import func
来源：http://hz.shzxlz.cn/gtxwgmrvgi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hywenlv.cn/gtvljecmli.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tanke756.top/gtbnzwifwb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.mhx1999.top/gtbpodqlnf.html

Java: import java.util.List;
来源：http://hz.hywenlv.cn/gtjjfythia.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shuidangran.top/gtoonqljkr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.feifeiyinyue.top/gtdpbvjanm.html

C#:   using System.Text;
来源：http://hz.nwbrower.top/gttliqitdj.html

[C12] 立即执行函数 IIFE
来源：http://hz.xziqi.cn/gtlyqsogee.html

Py:   (lambda: print("run"))()
来源：http://hz.zdqjudy.top/gtgxbutjnj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jlsjyb.cn/gtrdtumldo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtlotqonrj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.gogol.net.cn/gtrymjnkxq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinyuanbaomall.cn/gtslaqzhcd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.vqdsnc.cn/gtgyehpcxb.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhaomingkeji.xyz/gtuzqlksfs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.meibo888.top/gtrsrljgxt.html

[C13] 类型声明 / 类型注解
来源：http://hz.fzhhl.top/gtlcmmwbno.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.kuanghao11.cn/gtdnfdonvv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtieanqbxc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.bjfxy.top/gtmbgfwiqy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pengpengdd.cyou/gtamohjufa.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtnluvsnqk.html

Go:   func add(a, b int) int
来源：http://hz.quarkkingdee.top/gtwqfgspdt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hywenlv.cn/gtzvldrzbs.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sweek.top/gtatflbvps.html

[C14] 泛型函数
来源：http://hz.yj20258888.top/gtekcivjri.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gtzlfrlpqc.html

PHP:  // 无泛型
来源：http://hz.zhiwuduotai.top/gtimbuebum.html

JS:   // 无泛型
来源：http://hz.shanyushiyangkeji.top/gtuytttfzz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xuanzx.com/gtrfpotmsa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sysykeji.top/gtaloomhyl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ehwqpu.com/gtadkckfha.html

Ruby: # 无泛型
来源：http://hz.ydzc1.top/gtaewtyitl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.havefunace.top/gtstqkpqdr.html

[C15] 解构 / 展开参数
来源：http://hz.52xcode.cn/gtddxmbjfy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.guannengcc.top/gtxbeelfra.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aizwys.cn/gtnajlgmal.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.vqdsnc.cn/gtsettmcul.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhoulong.xyz/gtcqodynqe.html

Java: // 无解构
来源：http://hz.jinqigufen.top/gtlregqjaj.html

Go:   // 无解构
来源：http://hz.jyoumei.cn/gtvrnbbcqg.html

Ruby: a, b = pair
来源：http://hz.guowangkeji.top/gtqztdpyrs.html

C#:   var (a, b) = pair;
来源：http://hz.xinyue.icu/gtzwivaaqj.html

[C16] 函数 / 方法重载
来源：http://hz.zhongyouzk.top/gtnzcigwwp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cheryme.top/gtiweakzur.html

PHP:  // 无重载
来源：http://hz.hysaishi.cn/gtcjpjlnny.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xingfuxueyuan.xyz/gtmdnvriid.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhengqikj.top/gtlnjjhebq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ehwqpu.com/gtuidnlfxr.html


<!-- 参考信息 -->