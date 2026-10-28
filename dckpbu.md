代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hywenlv.cn/gtiitrsaqj.html

[B02] 多分支 else if / elif
来源：http://hz.xuanzx.com/gtkezfnzqj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.gotoacloud.top/gtfmulzwws.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jqgufenzy.top/gtapvkthwx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydjk.org.cn/gtxnnhrpkp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xinyue.icu/gtxfngbjnt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daxiang520.top/gtvsqvjezp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jlsjyb.cn/gtwcqscleg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.svipenyu.cn/gtkfwugpik.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtviwcuqsp.html

[B03] switch / match / case
来源：http://hz.9152youxi.cn/gtfaatnofd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.andypj.xyz/gtewmalfup.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yongpay.top/gtqchqdstp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cheryme.top/gtipiojmmx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinqigfzy.top/gtciiuyadx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.iojbl.cn/gtxtyxvfyb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.pengpengdd.cyou/gtlwdqelqj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.dashuyun.cn/gtyxzmqyiq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ivvv.top/gtlqwmcafn.html

[B04] for 计数循环
来源：http://hz.hongshengwenyu.top/gtnhzcshql.html

Py:   for i in range(10): print(i)
来源：http://hz.smart0.xyz/gtisoiuqji.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.bjfxy.top/gtqcsipmtx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.smart0.xyz/gtdjornryo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jiagoushi.top/gtodegdjqe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.sufxvd.cn/gtjxkqrypp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.xylfe.cn/gtnwkprwmp.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yanxiufei.cn/gtkenyjtbu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.feifeiyinyue.top/gthoiyuqyp.html

[B05] 遍历数组 / 列表
来源：http://hz.nwbrower.top/gtcnktelza.html

Py:   for item in arr: print(item)
来源：http://hz.yuxming.cn/gtdcywmyhn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jinghuilouyu.cn/gtbgjhbwih.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ybcxt.top/gtdmbhulan.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.ybcxt.top/gtekzeedub.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.gotoacloud.top/gtbjhqfimb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinghuilouyu.cn/gtktvkixak.html

Ruby: arr.each { |item| puts item }
来源：http://hz.xinyue.icu/gtppvsggyi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.wangdashe.top/gtqslkclwi.html

[B06] 遍历字典 / 对象
来源：http://hz.daria6918.cn/gtsdeaqqoj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.wangshuangyany.cn/gtyemdtgvh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.mhx1999.top/gttulruyna.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cqqwz.cn/gtxmdjgrwx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.tianlin.xyz/gtdswprinb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhengqikj.top/gtozuqouuq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ppjwa.cn/gtvnijqwim.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hywenlv.cn/gtaoeuonkh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.9152youxi.cn/gtvhdvvkvb.html

[B07] while 循环
来源：http://hz.zhiwuduotai.top/gtwmkapely.html

Py:   while i < 10: i += 1
来源：http://hz.0kj1m.cn/gtrovqwcsa.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yongpay.top/gtavtgxwty.html

JS:   while (i < 10) { i++; }
来源：http://hz.redwolf501.top/gtqadopdtt.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhaomingkeji.xyz/gtagfhojef.html

Java: while (i < 10) { i++; }
来源：http://hz.fengsongda.top/gtedtinpyd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.wangshuangyany.cn/gtjgffzcqk.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yvedp.cn/gtzaxfaglr.html

C#:   while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtykdhqbqi.html

[B08] do-while（至少执行一次）
来源：http://hz.ydzc1.top/gtgntzxxwy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xinyue.icu/gtgxaoxfxg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.daxiang520.top/gtfazngocf.html

JS:   do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gtvsaolrxh.html

TS:   do { i++; } while (i < 10);
来源：http://hz.cdnleiting.top/gtygatgumj.html

Java: do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gtsbiaysju.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zdqjudy.top/gtcbhqmrsu.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zdqjudy.top/gtqnngmwaq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gtlglggcna.html

[B09] break 与 continue
来源：http://hz.daxiang520.top/gtgdeppeik.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zhengqikj.top/gthgsrmhpu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ppjwa.cn/gtbzyobpdo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.c1oappe.top/gtcvusmlok.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gotoacloud.top/gtndhdzlam.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtcbfvxelw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zycfv.cn/gthsaptynb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shangyingyoupin.top/gtxkiaebow.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nwbrower.top/gttqcqzfpx.html

[B10] 遍历同时拿索引
来源：http://hz.jinghuilouyu.cn/gtqdzblaag.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.wangdashe.top/gtdfafalek.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.nanxinkj.top/gtnhqqbifk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.wangshuangyany.cn/gtifxehvgs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hysaishi.cn/gtslcproev.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.vqdsnc.cn/gtgihallvn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.guannengcc.top/gtjgxkggbc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.chenjidiqi.icu/gtvbsgzjed.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.bjfxy.top/gtquuqdljo.html

[B11] 生成数字序列 / 区间
来源：http://hz.wangdashe.top/gtkqehzhlp.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenlongwang.top/gttqfpmgnt.html

PHP:  range(0, 10, 2);
来源：http://hz.cashguo.top/gtwerfruxo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guowangkeji.top/gtkwvzpegb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xziqi.cn/gtgzqfmznn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hnqzz.top/gtpnwnqiif.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.snrcjt.cn/gtsklduipc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.haohaochexian.top/gtgmnkrwjv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinyuanbaomall.cn/gtxzhowils.html

[B12] 跳出多层循环
来源：http://hz.shangyingyoupin.top/gtllpkansm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nanxuanxn.top/gtmhcgdupw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhijiandao.cn/gtzihowsox.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ybcxt.top/gtxvexftzq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhongyouzk.top/gtrgarlxvm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hysaishi.cn/gtlgzyyvpd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hammf.cn/gttlvwnmks.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.wangdashe.top/gthwhgblvz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.daria6918.cn/gtojscwlxv.html

[B13] 判断是否为数字
来源：http://hz.dianchejie.cn/gtresemmum.html

Py:   isinstance(x, (int, float))
来源：http://hz.gogol.net.cn/gtucjjpozy.html

PHP:  is_numeric($x)
来源：http://hz.gotoacloud.top/gtafdnrhcf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhiwuduotai.top/gtizbvlyog.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zdqjudy.top/gtyeblefib.html

Java: x instanceof Number
来源：http://hz.sweek.top/gtehuqwbeo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinqigufen.top/gtphzltqrt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shangyingyoupin.top/gtvzugkwdj.html

C#:   x is int or double or decimal
来源：http://hz.sysykeji.top/gtthlypyxa.html

[B14] 判断值是否在集合内
来源：http://hz.hysaishi.cn/gtdvnvnmuv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hnqzz.top/gtcpgqsvne.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sxryk.cn/gtxelrjhqi.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.redwolf501.top/gtqyabvpxn.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jyoumei.cn/gtanowewpt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.pengpengdd.cyou/gtqhtuwqfg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.tanke756.top/gtidjztbiu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ywan-chungtsiang.top/gtvfvzdwyt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.bjfxy.top/gtytinagqi.html

[B15] 布尔运算与取反
来源：http://hz.yonumen.top/gthwfaseuy.html

Py:   a and b or not c
来源：http://hz.jianghu66.top/gtlusqlnfx.html

PHP:  $a && $b || !$c
来源：http://hz.vqdsnc.cn/gtrzqtarut.html

JS:   a && b || !c
来源：http://hz.yj20258888.top/gtdjuvvdwh.html

TS:   a && b || !c
来源：http://hz.xinyue.icu/gtrfesurqo.html

Java: a && b || !c
来源：http://hz.zhengqikj.top/gteuliblzd.html

Go:   a && b || !c
来源：http://hz.gotoacloud.top/gtunshqqok.html

Ruby: a && b || !c
来源：http://hz.hnxiangtu.top/gtyvtkvdru.html

C#:   a && b || !c
来源：http://hz.vqdsnc.cn/gtkiogiget.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.havefunace.top/gtfdvcmlxt.html

Py:   if not data: return
来源：http://hz.dashuyun.cn/gtenqiomxv.html

PHP:  if (!$data) { return; }
来源：http://hz.andypj.xyz/gtuwzdbugh.html

JS:   if (!data) return;
来源：http://hz.yueranfly.top/gtphjnrxop.html

TS:   if (!data) return;
来源：http://hz.yvedp.cn/gtneokeowt.html

Java: if (data == null) return;
来源：http://hz.0kj1m.cn/gthpwsdrpw.html

Go:   if data == nil { return }
来源：http://hz.haohaochexian.top/gtnkfikyxn.html

Ruby: return if data.nil?
来源：http://hz.hnqzz.top/gtbpdqprfm.html

C#:   if (data == null) return;
来源：http://hz.c1oappe.top/gtjksxtbgj.html

================================================================================
来源：http://hz.meibo888.top/gtgigtxwke.html

C. 函数与作用域
来源：http://hz.meibo888.top/gtzpcdazlu.html

================================================================================
来源：http://hz.tanke756.top/gttyvgqhjc.html

[C01] 定义函数
来源：http://hz.wangdashe.top/gtxdsuxscj.html

Py:   def add(a, b): return a + b
来源：http://hz.zhixingplan.top/gtywrctexx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhoulong.xyz/gtdiymyjbn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.andypj.xyz/gtfuwywqpq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sxryk.cn/gtrxougvsv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtbfwduaaj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pycfn.com/gtegulutyr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gogol.net.cn/gtqglfgdko.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtsvwduvgl.html

[C02] 默认参数
来源：http://hz.cucudq.cn/gtvraqegjf.html

Py:   def greet(name="World"): return name
来源：http://hz.sufxvd.cn/gtkrhsrlou.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tanke756.top/gtpszpfcnt.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jqgfzy.top/gtabwjysxw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.c1oappe.top/gtshsafjet.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ydjk.org.cn/gtrylytxpz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yongpay.top/gtuqyokyqu.html

Ruby: def greet(name = "World") = name
来源：http://hz.xinyue.icu/gtbicyaxuo.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xylfe.cn/gtkxjaatvq.html

[C03] 可变参数
来源：http://hz.hongshengwenyu.top/gtgpczqiai.html

Py:   def total(*args): return sum(args)
来源：http://hz.cdnleiting.top/gtvshhpkqd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.daria6918.cn/gtsautetfn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.smart0.xyz/gtxjoxzunn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guowangkeji.top/gtgtgtjyne.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.andypj.xyz/gtgljmtzjr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xuanzx.com/gtakehvvdi.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.daria6918.cn/gtwdtwxjho.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.wangdashe.top/gtxhkrwgfb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinyuanbaomall.cn/gtpgrapupj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shanyushiyangkeji.top/gtusxwhmbh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.havefunace.top/gtumicftum.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yanxiufei.cn/gtniuivhed.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.dianchejie.cn/gtcyrpbrwe.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sufxvd.cn/gtclhnxgaj.html

Go:   // 无：用配置结构体参数
来源：http://hz.nanxinkj.top/gtmokdnwct.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj20258.top/gtmuoiiveq.html

C#:   f(a: 1, b: 2)
来源：http://hz.redwolf501.top/gturowokzn.html

[C05] 返回多个值
来源：http://hz.kuanghao11.cn/gtcojqcdgm.html

Py:   return a, b
来源：http://hz.jlsjyb.cn/gtkfpgecyg.html

PHP:  return [$a, $b];
来源：http://hz.ydzc1.top/gtttcfyjfv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.0kj1m.cn/gthmoajrdw.html

TS:   return { a, b };
来源：http://hz.andypj.xyz/gtlvskbnqq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.guannengcc.top/gtruknkoll.html

Go:   return a, b
来源：http://hz.sysykeji.top/gtpvmivtlz.html

Ruby: return a, b
来源：http://hz.hammf.cn/gtyzkklmsf.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.9152youxi.cn/gtlnzeqzqz.html

[C06] 匿名函数 / lambda
来源：http://hz.pycfn.com/gtaabfwqww.html

Py:   square = lambda x: x * x
来源：http://hz.jiagoushi.top/gthtndalpp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jinyuanbaomall.cn/gtgjsalnwv.html

JS:   const square = x => x * x;
来源：http://hz.pycfn.com/gtneadakca.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jyoumei.cn/gtwmfrrzkv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.nwbrower.top/gtklwkcvau.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shuidangran.top/gtgweddgdx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jqgfzy.top/gtjcqpnvle.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shuidangran.top/gtdnoawbom.html

[C07] 把函数作为参数传入
来源：http://hz.sysykeji.top/gtdtfdeokt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenzaomai.com/gtfrpbjnfx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sweek.top/gtkpbkwkey.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yonumen.top/gtjhbiocjt.html

TS:   arr.map(String)
来源：http://hz.daxiang520.top/gtpibismxj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.c1oappe.top/gtynyvbcap.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhixingplan.top/gtorvuzjkh.html

Ruby: arr.map(&:upcase)
来源：http://hz.iojbl.cn/gtxlzsxwwi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ivvv.top/gtutjrdrpa.html

[C08] 闭包
来源：http://hz.jinyuanbaomall.cn/gtdgwcvcun.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.tian-w.cn/gtnmmfajds.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.snrcjt.cn/gtstjilfmp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.52xcode.cn/gtfdbfyfrz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yanxiufei.cn/gtmzasmijw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.quarkkingdee.top/gtaolcsjyt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hnqzz.top/gtmoihdaes.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.wangshuangyany.cn/gtmibeubvs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gtmmrkctdx.html

[C09] 递归
来源：http://hz.ybcxt.top/gtcdwdwxwf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shanyushiyangtech.top/gtqmmmogff.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.vqdsnc.cn/gtvhbyuxim.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guannengcc.top/gtdtubmkgz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ywan-chungtsiang.top/gthsjxowew.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258.top/gtlzruuohr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.smart0.xyz/gtsyvhegws.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ywan-chungtsiang.top/gthbfwtowm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.tanke756.top/gtwszkdnem.html

[C10] 变量作用域
来源：http://hz.shzxlz.cn/gtzlgjzhml.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhijiandao.cn/gtcuflqsdd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tanke756.top/gtmaywidln.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhongyouzk.top/gtbqkjchcs.html

TS:   同 JS
来源：http://hz.hnxiangtu.top/gtrcwrsqol.html

Java: 方法内为块级作用域
来源：http://hz.fengsongda.top/gtjyzcfvae.html

Go:   花括号块级作用域
来源：http://hz.yangfankeji.com/gtsfahqyua.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yueranfly.top/gtpgzvzbtq.html

C#:   块级作用域
来源：http://hz.shanyushiyangtech.top/gtlbsvgqpx.html

[C11] 模块导入与导出
来源：http://hz.hnxiangtu.top/gtcvzqedzz.html

Py:   from module import func
来源：http://hz.sufxvd.cn/gtgmlsayuk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhoulong.xyz/gtpoqrnlvn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.9152youxi.cn/gtckczatkn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gaohongyu789.top/gtxrrstbhz.html

Java: import java.util.List;
来源：http://hz.kuanghao11.cn/gthqdrooam.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jiagoushi.top/gtsmtxowob.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nwbrower.top/gtmsxbkhrj.html

C#:   using System.Text;
来源：http://hz.9152youxi.cn/gtzrssvydr.html

[C12] 立即执行函数 IIFE
来源：http://hz.9152youxi.cn/gtdwvojcyk.html

Py:   (lambda: print("run"))()
来源：http://hz.gogol.net.cn/gtpvukjwct.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxuanxn.top/gtzolixyuv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.gaohongyu789.top/gtshqbgnqc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.meibo888.top/gtwisnaymj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj20258888.top/gtkawnfwbq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.haohaochexian.top/gtalcgkjmv.html

Ruby: -> { puts "run" }.call
来源：http://hz.c1oappe.top/gtswrcqhzv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.fengsongda.top/gtnmjhjgve.html

[C13] 类型声明 / 类型注解
来源：http://hz.sweek.top/gtwwywmahy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ywan-chungtsiang.top/gthqjtkqnx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtdqdfphng.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinghuilouyu.cn/gtrouzljth.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cdnleiting.top/gtylqarcnd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.smart0.xyz/gtnenavbzh.html

Go:   func add(a, b int) int
来源：http://hz.hongshengwenyu.top/gtswpqtfgo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gogol.net.cn/gtpcjpjqen.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hysaishi.cn/gtdyaybqcg.html

[C14] 泛型函数
来源：http://hz.daxiang520.top/gtbijyhybl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.quarkkingdee.top/gtgnzzblhp.html

PHP:  // 无泛型
来源：http://hz.52xcode.cn/gtwlucsfct.html

JS:   // 无泛型
来源：http://hz.meibo888.top/gtixuxkani.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gaohongyu789.top/gtcxbgfmqo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenjidiqi.icu/gtutkkjhux.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ydjk.org.cn/gtajexigsi.html

Ruby: # 无泛型
来源：http://hz.jinqigufen.top/gtcngnzreg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenzaomai.com/gtpinqtofv.html

[C15] 解构 / 展开参数
来源：http://hz.jinqigfzy.top/gtolwgecrk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgfzy.top/gtmobazadw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shuidangran.top/gtredevhzl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.guannengcc.top/gtpwaiskpn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tian-w.cn/gtzfudvrkm.html

Java: // 无解构
来源：http://hz.yj20258888.top/gtjmefyolc.html

Go:   // 无解构
来源：http://hz.xuanzx.com/gtxxoihfyc.html

Ruby: a, b = pair
来源：http://hz.ehwqpu.com/gtzbxiaxtg.html

C#:   var (a, b) = pair;
来源：http://hz.nwbrower.top/gtnqogsshb.html

[C16] 函数 / 方法重载
来源：http://hz.chenjidiqi.icu/gtvknpigem.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.birdmap.top/gtudpknggv.html

PHP:  // 无重载
来源：http://hz.jinghuilouyu.cn/gtdwcrzvsr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cdnleiting.top/gtfimvenla.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258.top/gtzeatwfoe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.vqdsnc.cn/gtiztrfobd.html

Go:   // 无重载：用不同函数名
来源：http://hz.cheryme.top/gtpevupzoz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ivvv.top/gtzgpffzuc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sufxvd.cn/gtrowozrrh.html

================================================================================
来源：http://hz.cqqwz.cn/gtvyemhvtt.html

D. 数组 / 列表 / 集合
来源：http://hz.xuanzx.com/gtathrqxrz.html

================================================================================
来源：http://hz.hywenlv.cn/gtsublmxgw.html

[D01] 创建数组 / 列表
来源：http://hz.ivvv.top/gtjpgvqnpk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yanxiufei.cn/gtnntyvqfz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yangfankeji.com/gtdpwyvgrj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.fengsongda.top/gtbsocplpw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yuxming.cn/gtaxgxogqq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.fzhhl.top/gtilvrofpm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xuetiantiany.cn/gtvzffwavc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jqgufenzy.top/gtnchlxhnb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hywenlv.cn/gtzolmazwu.html

[D02] 追加元素到末尾
来源：http://hz.jianghu66.top/gtnfzzdnsf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shzxlz.cn/gtxlfrxpxy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.daxiang520.top/gtsdawcblq.html

JS:   arr.push(4);
来源：http://hz.hammf.cn/gtvbvjnehq.html

TS:   arr.push(4);
来源：http://hz.jqgfzy.top/gtbzvzspxq.html


<!-- 参考信息 -->