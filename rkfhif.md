代发 wailian999

[A26] 类型转换总览
来源：http://hz.ehwqpu.com/gtrnsquaoj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.cheryme.top/gtiywmouiz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.haohaochexian.top/gtqblbfzzj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.gzhubu.top/gtutpxsggz.html

TS:   Number() String() Boolean() x as number
来源：http://hz.havefunace.top/gtwvkaoiki.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.cheryme.top/gttaigtyie.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.daria6918.cn/gtmfpqwmux.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.pengpengdd.cyou/gtxefdwaju.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jqgfzy.top/gtcgnmnjwe.html

================================================================================
来源：http://hz.cdnleiting.top/gtptytxepx.html

B. 流程控制
来源：http://hz.feifeiyinyue.top/gthgjbesou.html

================================================================================
来源：http://hz.cheryme.top/gtkmfekhjo.html

[B01] 条件判断 if / else
来源：http://hz.jianghu66.top/gtnojqdzal.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.ydjk.org.cn/gtpjwgkjqq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.gotoacloud.top/gtywbpgfav.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jianghu66.top/gtdcrdvcqf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hysaishi.cn/gtkitjwlsz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.shangyingyoupin.top/gtwxxoppwj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.nanxinkj.top/gtofynmllh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.nanxuanxn.top/gttsowmhsf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.tanke756.top/gtilbuyzrc.html

[B02] 多分支 else if / elif
来源：http://hz.zhixingplan.top/gtyruxijnb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.aizwys.cn/gttzfdmryv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.shanyushiyangkeji.top/gtohdmxmjw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.c1oappe.top/gtzccgzzyb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shuidangran.top/gtkigghgjc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hnxiangtu.top/gtwthutkrk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.gzhubu.top/gtmemunato.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.wangshuangyany.cn/gtgzheegsf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hongshengwenyu.top/gtyvburppd.html

[B03] switch / match / case
来源：http://hz.hnxiangtu.top/gtxwyfjgme.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.chenjidiqi.icu/gthwztoeiu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jqgufenzy.top/gtbjpcsupn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.meibo888.top/gtjeuupdub.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhongyouzk.top/gtwnqjpavz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.chenzaomai.com/gtexeevzxe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.ivvv.top/gtnlaizgrl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yuxming.cn/gtowedjscl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhongyouzk.top/gtjcqajuck.html

[B04] for 计数循环
来源：http://hz.mhx1999.top/gtcxhymtbq.html

Py:   for i in range(10): print(i)
来源：http://hz.fzhhl.top/gtitdlptoc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.316326.xyz/gttlczlwoj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hfpthk.cn/gtpviclczn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yj20258888.top/gtiuwtmrfv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhijiandao.cn/gtzvazmcdo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yvedp.cn/gtjtmffjgo.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yueranfly.top/gtccagvvzm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jinqigfzy.top/gterawuamz.html

[B05] 遍历数组 / 列表
来源：http://hz.daxiang520.top/gtscwxqryx.html

Py:   for item in arr: print(item)
来源：http://hz.birdmap.top/gtgjdvcsnp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.vqdsnc.cn/gtvvknstui.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jqgfzy.top/gtfeebhjny.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jlsjyb.cn/gtnsmgdjwj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.birdmap.top/gtzsffbyrd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinghuilouyu.cn/gtywoakhbb.html

Ruby: arr.each { |item| puts item }
来源：http://hz.hfpthk.cn/gtjgeuvhlx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.fengsongda.top/gtbfayqvtd.html

[B06] 遍历字典 / 对象
来源：http://hz.feifeiyinyue.top/gtrhosksbw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yuanzhike.top/gtcwuqtlbw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yueranfly.top/gtqclehqyg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.snrcjt.cn/gtypdctpem.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sysykeji.top/gtgqyrvlcr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.shangyingyoupin.top/gtpnrgqhax.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.nwbrower.top/gtthxmbwet.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yuanzhike.top/gtaxywyavk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.cucudq.cn/gtvylzqjrm.html

[B07] while 循环
来源：http://hz.vqdsnc.cn/gtgzskxrsr.html

Py:   while i < 10: i += 1
来源：http://hz.yvedp.cn/gtxlkpsecf.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.shzxlz.cn/gtzhbtdwel.html

JS:   while (i < 10) { i++; }
来源：http://hz.yongpay.top/gthxapivlo.html

TS:   while (i < 10) { i++; }
来源：http://hz.cucudq.cn/gtzfrgphsr.html

Java: while (i < 10) { i++; }
来源：http://hz.svipenyu.cn/gtedqfxuzf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zycfv.cn/gtxuwsatqs.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xylfe.cn/gteepmlbvb.html

C#:   while (i < 10) { i++; }
来源：http://hz.sufxvd.cn/gthnhpgmap.html

[B08] do-while（至少执行一次）
来源：http://hz.c1oappe.top/gtmgloekvf.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.birdmap.top/gtqadrftug.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jyoumei.cn/gtuakofmtm.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhongyouzk.top/gtrogijxpx.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhongyouzk.top/gtavczysoe.html

Java: do { i++; } while (i < 10);
来源：http://hz.yj20258.top/gtccwxncel.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yonumen.top/gtwzhgqkjy.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xingfuxueyuan.xyz/gtxbpucios.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gtyxxbqkud.html

[B09] break 与 continue
来源：http://hz.yangfankeji.com/gtmcfrkjwu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.nwbrower.top/gtrtzpozqc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ppjwa.cn/gteepbgzmd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.redwolf501.top/gtwfwqykhq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtmukcfiks.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangdashe.top/gtkdguxupc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.iojbl.cn/gtjzrtlnnd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cdnleiting.top/gtmegicgho.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sysykeji.top/gtaunwuqxn.html

[B10] 遍历同时拿索引
来源：http://hz.gogol.net.cn/gtkewmbvui.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.fzhhl.top/gtltntgczd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jlsjyb.cn/gtuoutcrma.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gotoacloud.top/gttmclhzwu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.aizwys.cn/gthqvjsllp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hnqzz.top/gtdihnmdgg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ehwqpu.com/gtefawyrxa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.chenjidiqi.icu/gtlkotzqjn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yj202588.top/gtdjttoado.html

[B11] 生成数字序列 / 区间
来源：http://hz.dianchejie.cn/gtvlkrzjno.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenzaomai.com/gtvctkzinq.html

PHP:  range(0, 10, 2);
来源：http://hz.xingfuxueyuan.xyz/gtfmghxjwt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sysykeji.top/gtbmfiqbym.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yangfankeji.com/gtqfxgujqf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cqqwz.cn/gtpcsnvyrg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shanyushiyangkeji.top/gtlpmwtvip.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shuidangran.top/gtswezaeey.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.aibaodan.cn/gtrafuvirb.html

[B12] 跳出多层循环
来源：http://hz.jinghuilouyu.cn/gtezwhwxik.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.mhx1999.top/gtwipedxzw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhixingplan.top/gtqyuowijy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangkeji.top/gtupewqzep.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gteetgtdjl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.kuanghao11.cn/gtszsddccz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jqgfzy.top/gtbxzfnruh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jianghu66.top/gtigwfofhg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tian-w.cn/gtofhxtbjq.html

[B13] 判断是否为数字
来源：http://hz.chenzaomai.com/gtcovyeicu.html

Py:   isinstance(x, (int, float))
来源：http://hz.tian-w.cn/gtoiybggne.html

PHP:  is_numeric($x)
来源：http://hz.yanxiufei.cn/gtabjzkmci.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ybcxt.top/gtxjsobnpd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xziqi.cn/gtylyuimht.html

Java: x instanceof Number
来源：http://hz.jinqigfzy.top/gtlpipwihx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.daria6918.cn/gttcjzygsl.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hammf.cn/gtjmbcefah.html

C#:   x is int or double or decimal
来源：http://hz.shangyingyoupin.top/gtsrcjizhx.html

[B14] 判断值是否在集合内
来源：http://hz.guannengcc.top/gtbroivhwy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.dashuyun.cn/gtgjbsfblb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.fengsongda.top/gthwiacwgf.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.nanxuanxn.top/gtpyrlgblq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guowangkeji.top/gtirvrzrsu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cheryme.top/gtjdqrvyxr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.tian-w.cn/gtoqygmhag.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sufxvd.cn/gtxpgkpbjz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xuetiantiany.cn/gtxrxdkmhq.html

[B15] 布尔运算与取反
来源：http://hz.shanyushiyangkeji.top/gtyzvhqwuh.html

Py:   a and b or not c
来源：http://hz.xinyue.icu/gtkzmubbax.html

PHP:  $a && $b || !$c
来源：http://hz.hnxiangtu.top/gtpngdcniu.html

JS:   a && b || !c
来源：http://hz.zhijiandao.cn/gtvmpsttqg.html

TS:   a && b || !c
来源：http://hz.zhoulong.xyz/gtcspjwshg.html

Java: a && b || !c
来源：http://hz.wangshuangyany.cn/gtkqkjofed.html

Go:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtrqpvpihs.html

Ruby: a && b || !c
来源：http://hz.sufxvd.cn/gtdncbhaxl.html

C#:   a && b || !c
来源：http://hz.sysykeji.top/gtkhtefsxk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hongshengwenyu.top/gtpufrtuxf.html

Py:   if not data: return
来源：http://hz.chenlongwang.top/gtjlvpzoti.html

PHP:  if (!$data) { return; }
来源：http://hz.xuanzx.com/gthvwbdkfy.html

JS:   if (!data) return;
来源：http://hz.wangshuangyany.cn/gtqhgetqti.html

TS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtbkgjprkg.html

Java: if (data == null) return;
来源：http://hz.hywenlv.cn/gtascgxpzq.html

Go:   if data == nil { return }
来源：http://hz.shangyingyoupin.top/gtaztzmyaj.html

Ruby: return if data.nil?
来源：http://hz.tanke756.top/gtveccbhas.html

C#:   if (data == null) return;
来源：http://hz.hammf.cn/gtsdnnzemo.html

================================================================================
来源：http://hz.gzhubu.top/gthrlnstsf.html

C. 函数与作用域
来源：http://hz.yj20258.top/gtsxjrkpiw.html

================================================================================
来源：http://hz.nanxinkj.top/gtiinfrspp.html

[C01] 定义函数
来源：http://hz.daxiang520.top/gtxlcrylwd.html

Py:   def add(a, b): return a + b
来源：http://hz.dashuyun.cn/gtirxdcbtg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtqnzjiqhl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtywoqupeh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.quarkkingdee.top/gtqmrgxane.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gtdaatdrdg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yuanzhike.top/gtvtdqwbcx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tianlin.xyz/gthbxxopkh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtqlccdaik.html

[C02] 默认参数
来源：http://hz.jyoumei.cn/gtkiahtubn.html

Py:   def greet(name="World"): return name
来源：http://hz.shuidangran.top/gtduupnfem.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hongshengwenyu.top/gtzkonbtql.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jqgufenzy.top/gtnpimjpcm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xuetiantiany.cn/gteipdnmyr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xylfe.cn/gtfgvmjirj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hfpthk.cn/gtnaewudyn.html

Ruby: def greet(name = "World") = name
来源：http://hz.xylfe.cn/gtraxutzqw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sysykeji.top/gtmwhshxcj.html

[C03] 可变参数
来源：http://hz.xinyue.icu/gtbgjuequj.html

Py:   def total(*args): return sum(args)
来源：http://hz.wangshuangyany.cn/gtcvfvdnug.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.c1oappe.top/gtggwtqurv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hysaishi.cn/gtokljgqcd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gtqghxkxiw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zycfv.cn/gtnrhdqlwf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinqigfzy.top/gtgnbtlsjy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.andypj.xyz/gtpnbaxeek.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yangfankeji.com/gtetgaoyce.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yangfankeji.com/gtxhvjlpoh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shangyingyoupin.top/gtkdrracle.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sysykeji.top/gtreshunsb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.pycfn.com/gtdtcblwve.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cashguo.top/gtslywfjri.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zdqjudy.top/gtdxthickg.html

Go:   // 无：用配置结构体参数
来源：http://hz.dashuyun.cn/gtodkwrpvm.html

Ruby: f(a: 1, b: 2)
来源：http://hz.quarkkingdee.top/gtbmoalrht.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuanzx.com/gtucauxebd.html

[C05] 返回多个值
来源：http://hz.daria6918.cn/gtszataonn.html

Py:   return a, b
来源：http://hz.aizwys.cn/gtorrnvcnt.html

PHP:  return [$a, $b];
来源：http://hz.gzhubu.top/gtyrervglz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.pengpengdd.cyou/gtxhwugplo.html

TS:   return { a, b };
来源：http://hz.dashuyun.cn/gtsptlutku.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zdqjudy.top/gtrhygncpi.html

Go:   return a, b
来源：http://hz.cheryme.top/gtlgmsupct.html

Ruby: return a, b
来源：http://hz.jinyuanbaomall.cn/gtpzyyyhzl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.nwbrower.top/gtkzlwofii.html

[C06] 匿名函数 / lambda
来源：http://hz.chenjidiqi.icu/gtxouchovz.html

Py:   square = lambda x: x * x
来源：http://hz.xylfe.cn/gtmenwcbhw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gotoacloud.top/gtvkjhfkgk.html

JS:   const square = x => x * x;
来源：http://hz.sysykeji.top/gtshmcbwmh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hysaishi.cn/gttcfvnhnd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hysaishi.cn/gtkoktsgvu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhoulong.xyz/gtvfebyxyc.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nanxuanxn.top/gteqocdeja.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hnxiangtu.top/gtonztgqfa.html

[C07] 把函数作为参数传入
来源：http://hz.zhongyouzk.top/gtpejdnsaa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jyoumei.cn/gtowqpmtlk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guowangkeji.top/gtlhgwgbmn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinghuilouyu.cn/gtrdxvlbny.html

TS:   arr.map(String)
来源：http://hz.ivvv.top/gtbhsnwiaz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.wangdashe.top/gtzgvhwfea.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ydzc1.top/gtboqyfspv.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxinkj.top/gtkwnagvzf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhiwuduotai.top/gtkrbyzhkn.html

[C08] 闭包
来源：http://hz.wangdashe.top/gtofiqudzm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigfzy.top/gthtdqmrzs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.feifeiyinyue.top/gtbsowtzjg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.smart0.xyz/gtnndlgecb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhijiandao.cn/gtbzyooxhu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ydzc1.top/gtfjhtmgwz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.fzhhl.top/gthbsjsxsk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.kuanghao11.cn/gtniomivev.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtgtpslljm.html

[C09] 递归
来源：http://hz.sweek.top/gtoanzrydr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xylfe.cn/gtsnrwnbrg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtfdfoprmb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258.top/gtznzkjmvi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydzc1.top/gtbswplsfu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.sysykeji.top/gtevpcpnaj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dashuyun.cn/gtfhgxnucd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.birdmap.top/gtjbrixrsr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xziqi.cn/gtcxaiyroi.html

[C10] 变量作用域
来源：http://hz.smart0.xyz/gtlopbssfz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xuetiantiany.cn/gtppkgfzoj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.c1oappe.top/gtaleaaeak.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xuanzx.com/gtcigiuxrj.html

TS:   同 JS
来源：http://hz.yj20258.top/gtzgismgdw.html

Java: 方法内为块级作用域
来源：http://hz.shanyushiyangkeji.top/gtccdrrtji.html

Go:   花括号块级作用域
来源：http://hz.ehwqpu.com/gtcrplouqr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gotoacloud.top/gtwndxyyra.html

C#:   块级作用域
来源：http://hz.yangfankeji.com/gtzhgqvvpl.html

[C11] 模块导入与导出
来源：http://hz.nanxinkj.top/gtuaycjcva.html

Py:   from module import func
来源：http://hz.fzhhl.top/gtygvyokwv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zycfv.cn/gtijrreeth.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.aizwys.cn/gttbpjwtzv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cdnleiting.top/gtdishrnyl.html

Java: import java.util.List;
来源：http://hz.aibaodan.cn/gtcuedsvtc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.0kj1m.cn/gthnlqjewv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zycfv.cn/gtiunvntkb.html

C#:   using System.Text;
来源：http://hz.zhijiandao.cn/gthorxpqfh.html

[C12] 立即执行函数 IIFE
来源：http://hz.fengsongda.top/gtnixxahwl.html

Py:   (lambda: print("run"))()
来源：http://hz.xziqi.cn/gtfmwvlwnl.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shzxlz.cn/gtdhkkeemy.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sufxvd.cn/gtmcmkzjml.html

TS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gtuudofynw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.chenzaomai.com/gtkpxypzfj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.redwolf501.top/gtudfibpka.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinghuilouyu.cn/gtrqflhjxa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ybcxt.top/gtxzgkdkvl.html

[C13] 类型声明 / 类型注解
来源：http://hz.ybcxt.top/gtepphltfk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pengpengdd.cyou/gtuqiqpzeo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtwgrscyfs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hongshengwenyu.top/gtnkhsdjrg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydzc1.top/gtmrmhbpfz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtytfsepvl.html

Go:   func add(a, b int) int
来源：http://hz.yongpay.top/gtdhnxxhlb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yangfankeji.com/gtzpmmwvyk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jqgufenzy.top/gtwmwbbwnh.html

[C14] 泛型函数
来源：http://hz.haohaochexian.top/gtzwvudzmm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenjidiqi.icu/gtxjfxuvyw.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangtech.top/gtcphusrmb.html

JS:   // 无泛型
来源：http://hz.jianghu66.top/gtjbapnmyj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhijiandao.cn/gtdadmgwpy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ivvv.top/gtjrtdzfcl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangshuangyany.cn/gthwjjtxss.html

Ruby: # 无泛型
来源：http://hz.birdmap.top/gtkgifghut.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gaohongyu789.top/gtllmfsiiz.html

[C15] 解构 / 展开参数
来源：http://hz.iojbl.cn/gteomuvsfa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhixingplan.top/gttfkimflc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.iojbl.cn/gtydwzlrzo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhixingplan.top/gtgqicamyl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yuxming.cn/gtlzsttokf.html

Java: // 无解构
来源：http://hz.snrcjt.cn/gtblaajxor.html

Go:   // 无解构
来源：http://hz.shzxlz.cn/gtajfnuqyo.html

Ruby: a, b = pair
来源：http://hz.chenlongwang.top/gtrcbxoncz.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtczwmrils.html

[C16] 函数 / 方法重载
来源：http://hz.nwbrower.top/gtkimcrwwp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258.top/gtxldxyuxf.html

PHP:  // 无重载
来源：http://hz.quarkkingdee.top/gtowwmvxio.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.wangdashe.top/gtgzuylxyw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tian-w.cn/gtzishcwyx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tianlin.xyz/gtdueayxbd.html


<!-- 参考信息 -->