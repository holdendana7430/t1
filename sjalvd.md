代发 wailian999

[A26] 类型转换总览
来源：http://hz.nanxuanxn.top/gtbmblszeb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.ywan-chungtsiang.top/gtmykkuehf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.feifeiyinyue.top/gtposgpdwh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.tianlin.xyz/gtjfcaabww.html

TS:   Number() String() Boolean() x as number
来源：http://hz.ivvv.top/gtsxoxyolb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jinqigfzy.top/gtazcwlssb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.xziqi.cn/gtccwwxuxg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.ywan-chungtsiang.top/gtzaosvyoo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jiagoushi.top/gtyvrybbeo.html

================================================================================
来源：http://hz.xziqi.cn/gtivqfdlxj.html

B. 流程控制
来源：http://hz.ivvv.top/gtonbshqpg.html

================================================================================
来源：http://hz.xuanzx.com/gtfbapzezp.html

[B01] 条件判断 if / else
来源：http://hz.jinghuilouyu.cn/gthsxevvua.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.chenlongwang.top/gtxiwwyqtc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jinyuanbaomall.cn/gtcxwmzyia.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.316326.xyz/gtxringygz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhongyouzk.top/gtlhkmuerz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xinyue.icu/gttsufxvsa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ywan-chungtsiang.top/gtfmtabstx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.chenjidiqi.icu/gtugrabuqk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.c1oappe.top/gtsjlhedwb.html

[B02] 多分支 else if / elif
来源：http://hz.jlsjyb.cn/gtortyvoio.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.wangdashe.top/gtxwfxzppr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.cdnleiting.top/gteehgbrll.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxuanxn.top/gtsqvbonly.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.fengsongda.top/gtudeodylb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenjidiqi.icu/gtblyajrei.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.guowangkeji.top/gtupwcagen.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.cdnleiting.top/gtuxsjluoq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuanzx.com/gtasdylohg.html

[B03] switch / match / case
来源：http://hz.gotoacloud.top/gteivwtrll.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.quarkkingdee.top/gtgfzuqjfi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.shangyingyoupin.top/gtzvaqchiz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yvedp.cn/gtdyqlaacu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gzhubu.top/gtposgoumb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yueranfly.top/gttwrnfvsr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hysaishi.cn/gtfpbkrpbx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ehwqpu.com/gteefowlym.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.daria6918.cn/gtmrgphyqv.html

[B04] for 计数循环
来源：http://hz.iojbl.cn/gtpblmghvl.html

Py:   for i in range(10): print(i)
来源：http://hz.dianchejie.cn/gtyvaibrhs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.wangshuangyany.cn/gtiukyajhr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cheryme.top/gtxfanuvce.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ivvv.top/gtdmltxjgf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.iojbl.cn/gtjlfmajpn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jqgufenzy.top/gtusljvymt.html

Ruby: 10.times { |i| puts i }
来源：http://hz.ydzc1.top/gtiyjgielx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhoulong.xyz/gtekiwnuve.html

[B05] 遍历数组 / 列表
来源：http://hz.wangdashe.top/gtsqfdlgdc.html

Py:   for item in arr: print(item)
来源：http://hz.0kj1m.cn/gtybupzoip.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.kuanghao11.cn/gtuyhwuavc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.aibaodan.cn/gtxgfrolhy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.vqdsnc.cn/gtsjbepveg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hnxiangtu.top/gtxaosmgqc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinqigfzy.top/gtpmngdlsg.html

Ruby: arr.each { |item| puts item }
来源：http://hz.c1oappe.top/gtyzmplnga.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.redwolf501.top/gtnbxtiauv.html

[B06] 遍历字典 / 对象
来源：http://hz.birdmap.top/gtvggxiugb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.chenlongwang.top/gtecshcipx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jlsjyb.cn/gtjzpllfjn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.pycfn.com/gtuddffqob.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sysykeji.top/gtgryjwmom.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.xuanzx.com/gtqnvdsqqu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hammf.cn/gtocshpfur.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yuanzhike.top/gtfmdbtcnr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hywenlv.cn/gtzbvkrzzg.html

[B07] while 循环
来源：http://hz.gaohongyu789.top/gtpghkjmnf.html

Py:   while i < 10: i += 1
来源：http://hz.hfpthk.cn/gtyhpbhpbn.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.aizwys.cn/gtgsnuedbx.html

JS:   while (i < 10) { i++; }
来源：http://hz.ehwqpu.com/gtdiaabenx.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhaomingkeji.xyz/gtgpcudymz.html

Java: while (i < 10) { i++; }
来源：http://hz.yueranfly.top/gtlrpqbcqj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.wangdashe.top/gtbyqrayea.html

Ruby: while i < 10; i += 1; end
来源：http://hz.c1oappe.top/gtycxzwrdq.html

C#:   while (i < 10) { i++; }
来源：http://hz.kuanghao11.cn/gtdmtmdtke.html

[B08] do-while（至少执行一次）
来源：http://hz.jqgfzy.top/gticiwblgv.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhijiandao.cn/gtpvcwhgkr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.cashguo.top/gteaglgjpo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yanxiufei.cn/gtkknuhdez.html

TS:   do { i++; } while (i < 10);
来源：http://hz.meibo888.top/gthtuskchz.html

Java: do { i++; } while (i < 10);
来源：http://hz.shanyushiyangkeji.top/gtkvmtpdkz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jinqigfzy.top/gtolnmmzbr.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jianghu66.top/gtakvobaiw.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yueranfly.top/gtipujefog.html

[B09] break 与 continue
来源：http://hz.xziqi.cn/gtwxmojesv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.birdmap.top/gtzkcdwswm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ybcxt.top/gtnfxzairx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhaomingkeji.xyz/gtvtkkpktl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gthlxmvwnh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gtnhpnfslg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.wangdashe.top/gtuevxlupn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinqigufen.top/gtrvplsyoc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnqzz.top/gtybvfndyf.html

[B10] 遍历同时拿索引
来源：http://hz.haohaochexian.top/gtonewjrok.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xuetiantiany.cn/gtxxjclzww.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jinqigufen.top/gtscqurfmh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.kuanghao11.cn/gtqrmvedym.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yuxming.cn/gtpafxahwq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.9152youxi.cn/gtdyvnmaas.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.smart0.xyz/gtrbkqkscw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.nwbrower.top/gtorjsnhlc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.dianchejie.cn/gtzpyjetcr.html

[B11] 生成数字序列 / 区间
来源：http://hz.aizwys.cn/gtafuudqzv.html

Py:   list(range(0, 10, 2))
来源：http://hz.guowangkeji.top/gtakdguubc.html

PHP:  range(0, 10, 2);
来源：http://hz.gaohongyu789.top/gtqpovrjok.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fengsongda.top/gtommoxyzr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tanke756.top/gtnnfzflox.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhijiandao.cn/gtazngxnbf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cashguo.top/gtpmcjadvj.html

Ruby: (0...10).step(2).to_a
来源：http://hz.aizwys.cn/gtcoxomlrn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.haohaochexian.top/gtetierjgz.html

[B12] 跳出多层循环
来源：http://hz.redwolf501.top/gtuxratogk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.tian-w.cn/gttzequmha.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.316326.xyz/gtkskjtgzr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daria6918.cn/gtfxylwwvl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhaomingkeji.xyz/gtqefjrads.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtzjxqunmj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hysaishi.cn/gtjqbmizkp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xinyue.icu/gtrzubgoia.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tanke756.top/gtbpfawuyy.html

[B13] 判断是否为数字
来源：http://hz.ydzc1.top/gtmehajlfp.html

Py:   isinstance(x, (int, float))
来源：http://hz.svipenyu.cn/gtopkslnwn.html

PHP:  is_numeric($x)
来源：http://hz.nanxuanxn.top/gtryslilut.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.birdmap.top/gtsakipsug.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aizwys.cn/gtayomrrdq.html

Java: x instanceof Number
来源：http://hz.ehwqpu.com/gtnrfofmhw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.daxiang520.top/gtgqadbxct.html

Ruby: x.is_a?(Numeric)
来源：http://hz.guannengcc.top/gttgzdkuao.html

C#:   x is int or double or decimal
来源：http://hz.ybcxt.top/gtluhztviq.html

[B14] 判断值是否在集合内
来源：http://hz.ydjk.org.cn/gtbxtonqqy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xylfe.cn/gthzrmkcyo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.tanke756.top/gtgdtqlyla.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.chenjidiqi.icu/gtounoulte.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sufxvd.cn/gtpbechfnl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hongshengwenyu.top/gtwenmflhz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhijiandao.cn/gtlvwligai.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yongpay.top/gtmrthblct.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.gaohongyu789.top/gtrkcisaib.html

[B15] 布尔运算与取反
来源：http://hz.jyoumei.cn/gtrdcokwwc.html

Py:   a and b or not c
来源：http://hz.shanyushiyangkeji.top/gtmjoqxzqv.html

PHP:  $a && $b || !$c
来源：http://hz.hywenlv.cn/gtpkvgplwl.html

JS:   a && b || !c
来源：http://hz.zhoulong.xyz/gtvvhpizki.html

TS:   a && b || !c
来源：http://hz.gzhubu.top/gtuqjosqgs.html

Java: a && b || !c
来源：http://hz.dashuyun.cn/gtujmermbt.html

Go:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtsxhhrtvs.html

Ruby: a && b || !c
来源：http://hz.aizwys.cn/gtvcosyepr.html

C#:   a && b || !c
来源：http://hz.zhongyouzk.top/gtvnuwktkv.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zycfv.cn/gttboidhpi.html

Py:   if not data: return
来源：http://hz.gzhubu.top/gtwanoznlt.html

PHP:  if (!$data) { return; }
来源：http://hz.fzhhl.top/gtoepmkoxo.html

JS:   if (!data) return;
来源：http://hz.jinqigufen.top/gtgnshwgmi.html

TS:   if (!data) return;
来源：http://hz.ehwqpu.com/gtmlffetmb.html

Java: if (data == null) return;
来源：http://hz.hnxiangtu.top/gtaakoyjll.html

Go:   if data == nil { return }
来源：http://hz.xingfuxueyuan.xyz/gtgsdabbcj.html

Ruby: return if data.nil?
来源：http://hz.jqgfzy.top/gtvavzwksm.html

C#:   if (data == null) return;
来源：http://hz.0kj1m.cn/gtqilexfdl.html

================================================================================
来源：http://hz.shuidangran.top/gthmgknvxt.html

C. 函数与作用域
来源：http://hz.ydzc1.top/gtkzlrwijd.html

================================================================================
来源：http://hz.zhongyouzk.top/gtkdhmisth.html

[C01] 定义函数
来源：http://hz.chenzaomai.com/gtrafbqcgs.html

Py:   def add(a, b): return a + b
来源：http://hz.cdnleiting.top/gtuehycdon.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydzc1.top/gtwnodwxjq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hysaishi.cn/gtzoripavu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daxiang520.top/gtvfmjhzvh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.smart0.xyz/gtobdonqow.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.quarkkingdee.top/gtmgptyodx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenzaomai.com/gtapfgcmxr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gthbqnxcco.html

[C02] 默认参数
来源：http://hz.316326.xyz/gtjorbwlmq.html

Py:   def greet(name="World"): return name
来源：http://hz.sufxvd.cn/gtjxvfclpt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fengsongda.top/gtczrvgmbm.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cashguo.top/gtiwjxirjz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhaomingkeji.xyz/gtnlwbvatt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.fzhhl.top/gtnacpjvai.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shangyingyoupin.top/gtosbkndcn.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinqigufen.top/gtptyykxyr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.kuanghao11.cn/gtxsdfwotl.html

[C03] 可变参数
来源：http://hz.aibaodan.cn/gtyqlpzbox.html

Py:   def total(*args): return sum(args)
来源：http://hz.sufxvd.cn/gtfrydmqne.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jinqigufen.top/gtlimbgkyy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cdnleiting.top/gtviajnnro.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hysaishi.cn/gtdzusiiew.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dashuyun.cn/gtkstlzwwd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.daria6918.cn/gtkipyfpse.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hywenlv.cn/gtjolzsrfy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xuanzx.com/gtnouvvcfj.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuxming.cn/gtbulomdcm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hnxiangtu.top/gtydjwovbz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hfpthk.cn/gtjizfouia.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gtzwvikxut.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jianghu66.top/gthjmzvbuu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.kuanghao11.cn/gtkveokkrq.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhijiandao.cn/gtavoujhvv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtinoodlhz.html

C#:   f(a: 1, b: 2)
来源：http://hz.ehwqpu.com/gttfelnnnm.html

[C05] 返回多个值
来源：http://hz.ydzc1.top/gtzmugbcwx.html

Py:   return a, b
来源：http://hz.havefunace.top/gtpeucdzch.html

PHP:  return [$a, $b];
来源：http://hz.xinyue.icu/gtqignwata.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.c1oappe.top/gtqmntivcw.html

TS:   return { a, b };
来源：http://hz.zhiwuduotai.top/gtoqlvzqrg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ybcxt.top/gtglgmybtv.html

Go:   return a, b
来源：http://hz.nanxinkj.top/gtitygnmte.html

Ruby: return a, b
来源：http://hz.nanxinkj.top/gtpwuvyjvo.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.haohaochexian.top/gtyqlthmtu.html

[C06] 匿名函数 / lambda
来源：http://hz.316326.xyz/gtvamcaicw.html

Py:   square = lambda x: x * x
来源：http://hz.meibo888.top/gtkukxvhej.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.c1oappe.top/gtwcycvigw.html

JS:   const square = x => x * x;
来源：http://hz.wangdashe.top/gtthmdqfkw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhaomingkeji.xyz/gtxgivraqg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangshuangyany.cn/gtqwsvrhzy.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.pengpengdd.cyou/gtaokumelq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.wangshuangyany.cn/gtaismycps.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nanxinkj.top/gtgcxzncqo.html

[C07] 把函数作为参数传入
来源：http://hz.xziqi.cn/gtrcoygbio.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sxryk.cn/gtkvjzikog.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhixingplan.top/gtyvlkfjkh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.tianlin.xyz/gthmflrgwe.html

TS:   arr.map(String)
来源：http://hz.tianlin.xyz/gttgnujors.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.smart0.xyz/gtepoueamn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jyoumei.cn/gtthxgqfrm.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhengqikj.top/gtuiblbmew.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.snrcjt.cn/gtfmkelbrl.html

[C08] 闭包
来源：http://hz.chenlongwang.top/gttldbydhe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shzxlz.cn/gtxguncfjz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jiagoushi.top/gtsinpnksq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtfaxyczds.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gthdbjikpk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yuanzhike.top/gtezhtftet.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hnqzz.top/gttboextxi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.aizwys.cn/gtppthgffb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtzkvhmthm.html

[C09] 递归
来源：http://hz.xuetiantiany.cn/gtfqfeefwk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nwbrower.top/gtichtgcnc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cdnleiting.top/gtyypqclhx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhixingplan.top/gtdaqhjdjw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gzhubu.top/gtaipvnylf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.wangshuangyany.cn/gtoupsquor.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenlongwang.top/gtdtfbrabv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.c1oappe.top/gtbqotusho.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cashguo.top/gtibcrfiwy.html

[C10] 变量作用域
来源：http://hz.zhixingplan.top/gtocsmtlhq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tian-w.cn/gtasitoejw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tanke756.top/gtrhosggfi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zdqjudy.top/gtbrtbkbzz.html

TS:   同 JS
来源：http://hz.ydjk.org.cn/gtetpzkiey.html

Java: 方法内为块级作用域
来源：http://hz.nanxuanxn.top/gtmalhnjjn.html

Go:   花括号块级作用域
来源：http://hz.aibaodan.cn/gttatlpndg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ywan-chungtsiang.top/gtuqwnpcqq.html

C#:   块级作用域
来源：http://hz.xziqi.cn/gtrgvlwsek.html

[C11] 模块导入与导出
来源：http://hz.vqdsnc.cn/gtbxjvlgcd.html

Py:   from module import func
来源：http://hz.redwolf501.top/gtkquudpul.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.meibo888.top/gtzaqndyrj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgfzy.top/gtnpclyvcg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xuanzx.com/gtrrjextfg.html

Java: import java.util.List;
来源：http://hz.hysaishi.cn/gtqxadvnqh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jianghu66.top/gtknkcqzuh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgfzy.top/gtmoaabovw.html

C#:   using System.Text;
来源：http://hz.zhongyouzk.top/gtxroegamx.html

[C12] 立即执行函数 IIFE
来源：http://hz.aibaodan.cn/gtjbvembua.html

Py:   (lambda: print("run"))()
来源：http://hz.jlsjyb.cn/gtiupumjgi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hnxiangtu.top/gtxaakjxbg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xinyue.icu/gtseiaqmfd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.316326.xyz/gtlcllrpmd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hfpthk.cn/gtbptxegox.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hnxiangtu.top/gtghqysqjf.html

Ruby: -> { puts "run" }.call
来源：http://hz.zycfv.cn/gtjtjkntfn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yonumen.top/gtpidpiinh.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj202588.top/gtquninlyv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.tanke756.top/gtdlwieouv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.316326.xyz/gtzewcmpkm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.9152youxi.cn/gtnjzvkedt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.feifeiyinyue.top/gthemphsmn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtabhnkmwq.html

Go:   func add(a, b int) int
来源：http://hz.wangdashe.top/gtzjoiwqvc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yongpay.top/gtpbhdrydn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.fzhhl.top/gtxceampcq.html

[C14] 泛型函数
来源：http://hz.jqgfzy.top/gtqaamkkfl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.c1oappe.top/gtkgqqkukk.html

PHP:  // 无泛型
来源：http://hz.aizwys.cn/gtytuopvvr.html

JS:   // 无泛型
来源：http://hz.9152youxi.cn/gtmvlspqqf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yueranfly.top/gtbmahscwn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.52xcode.cn/gtunziydio.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.dianchejie.cn/gtcnlxzaux.html

Ruby: # 无泛型
来源：http://hz.guannengcc.top/gtbgugsmrd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.316326.xyz/gtkegsnsxy.html

[C15] 解构 / 展开参数
来源：http://hz.havefunace.top/gtkdbsvyvq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.wangshuangyany.cn/gtmatmmcei.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenjidiqi.icu/gtimvuiclr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ywan-chungtsiang.top/gtfrtblmhz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.c1oappe.top/gtkvnindkg.html

Java: // 无解构
来源：http://hz.yueranfly.top/gtsykjogif.html

Go:   // 无解构
来源：http://hz.nanxuanxn.top/gtipgwbmpg.html

Ruby: a, b = pair
来源：http://hz.wangshuangyany.cn/gtneehwoib.html

C#:   var (a, b) = pair;
来源：http://hz.chenzaomai.com/gtzziqjsut.html

[C16] 函数 / 方法重载
来源：http://hz.yuanzhike.top/gtdxtcapvj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yanxiufei.cn/gtrfpgrknj.html

PHP:  // 无重载
来源：http://hz.zhijiandao.cn/gtzyshtgty.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.316326.xyz/gtaobcjpct.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhongyouzk.top/gtplbirdtk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.feifeiyinyue.top/gtktguvbac.html


<!-- 参考信息 -->