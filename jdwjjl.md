代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.sweek.top/gtckyzwnjn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hongshengwenyu.top/gtcbdhcjdr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.nwbrower.top/gtmndqtcyi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.xingfuxueyuan.xyz/gtbidbnwqd.html

Go:   strings.TrimSpace(s)
来源：http://hz.dianchejie.cn/gtjdaukicd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.svipenyu.cn/gtfmohuiuq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.bjfxy.top/gtkqtgwgdg.html

[A25] 字符串比较
来源：http://hz.hnqzz.top/gteammsanc.html

Py:   s1 == s2; s1 != s2
来源：http://hz.mhx1999.top/gtftgzafka.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yongpay.top/gtxbltyayu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jqgufenzy.top/gtbgoibryn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.wangshuangyany.cn/gtcibcuzzp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.shanyushiyangtech.top/gtcxnywdhu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.haohaochexian.top/gtjdxihelz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.9152youxi.cn/gthdvsnamy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xuetiantiany.cn/gtczuwkvth.html

[A26] 类型转换总览
来源：http://hz.shzxlz.cn/gtfiemkesp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.hammf.cn/gterbcnhis.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.aibaodan.cn/gtupgsbgci.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.sxryk.cn/gtunhhtwfm.html

TS:   Number() String() Boolean() x as number
来源：http://hz.wangshuangyany.cn/gtvqeennkd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jianghu66.top/gtsctbeefj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhixingplan.top/gtqhhaskef.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.feifeiyinyue.top/gtuqceukzd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.cdnleiting.top/gtpkqnxdka.html

================================================================================
来源：http://hz.tianlin.xyz/gtejmxenus.html

B. 流程控制
来源：http://hz.ybcxt.top/gtfxevjssf.html

================================================================================
来源：http://hz.cdnleiting.top/gtmklmdkqf.html

[B01] 条件判断 if / else
来源：http://hz.yongpay.top/gtktcwbvzn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.pycfn.com/gtmqofxbbt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.gotoacloud.top/gtllshcugf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.havefunace.top/gtsmpwhhuf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hywenlv.cn/gteqfbpjkz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.feifeiyinyue.top/gtuwzojqlo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yonumen.top/gtcwrzhjkw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.pycfn.com/gtezqejmej.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.snrcjt.cn/gtczdzdsew.html

[B02] 多分支 else if / elif
来源：http://hz.yongpay.top/gtjvcmsyox.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.sysykeji.top/gtvizeyxvn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jiagoushi.top/gtnptqskzg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shanyushiyangtech.top/gtrjlnegyx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuetiantiany.cn/gtezkgcgqq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ivvv.top/gtwwnifebe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.chenjidiqi.icu/gtdhtmijxp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhoulong.xyz/gtwgmrdiza.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.smart0.xyz/gtktgigwcf.html

[B03] switch / match / case
来源：http://hz.ivvv.top/gtdrdwpgzq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.pengpengdd.cyou/gtekdmujlu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yongpay.top/gtejbcjgbg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jqgufenzy.top/gtctukfwaz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhixingplan.top/gtrnofvhzi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.andypj.xyz/gtkczxynro.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.guowangkeji.top/gtayscdovo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.xuanzx.com/gtuczfwuif.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.sufxvd.cn/gtobtdzqvg.html

[B04] for 计数循环
来源：http://hz.hammf.cn/gthmnnokoh.html

Py:   for i in range(10): print(i)
来源：http://hz.xuanzx.com/gtnbukcpaj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.sxryk.cn/gtuzspdutq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.chenlongwang.top/gtzycrdzwf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shanyushiyangkeji.top/gtwnyvrsqt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.nwbrower.top/gtvlfffpuh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.9152youxi.cn/gtsyqgqtru.html

Ruby: 10.times { |i| puts i }
来源：http://hz.hongshengwenyu.top/gteixlunhv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.aizwys.cn/gtxtsvbpfj.html

[B05] 遍历数组 / 列表
来源：http://hz.kuanghao11.cn/gtewmsnckw.html

Py:   for item in arr: print(item)
来源：http://hz.chenlongwang.top/gtenlbuzjv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.aizwys.cn/gtpeojnejc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.tanke756.top/gtcydhrkmv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.aibaodan.cn/gtveeivzec.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hfpthk.cn/gtvzltddxx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.nwbrower.top/gtbhgcqshn.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jinghuilouyu.cn/gtqgrkuqyf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.wangshuangyany.cn/gtktmzjjqh.html

[B06] 遍历字典 / 对象
来源：http://hz.yvedp.cn/gtfetkzgyu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yvedp.cn/gtaxrlqvco.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinqigufen.top/gthuklajfd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.chenlongwang.top/gtywhwrucg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jiagoushi.top/gtiytbpkep.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.sysykeji.top/gtsjghqjkl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shzxlz.cn/gtzrglxmue.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.iojbl.cn/gtwjtejmev.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.andypj.xyz/gtsrthozpx.html

[B07] while 循环
来源：http://hz.ydzc1.top/gtivvqxhfj.html

Py:   while i < 10: i += 1
来源：http://hz.jqgufenzy.top/gtnsejdlyv.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.cqqwz.cn/gtqdesslbp.html

JS:   while (i < 10) { i++; }
来源：http://hz.jinqigufen.top/gtqezrliih.html

TS:   while (i < 10) { i++; }
来源：http://hz.sufxvd.cn/gtfkjhybcs.html

Java: while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gtpnhqdmze.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ppjwa.cn/gtaenahmkr.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhoulong.xyz/gtnmvdikob.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtnjitvqyg.html

[B08] do-while（至少执行一次）
来源：http://hz.cashguo.top/gtbdeapiem.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yuxming.cn/gtbdjsmmrj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hnxiangtu.top/gtecjypnlb.html

JS:   do { i++; } while (i < 10);
来源：http://hz.chenjidiqi.icu/gtwtuckzpp.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gtgchnmhyp.html

Java: do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gtzybfxssv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jqgfzy.top/gtaezldkwc.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.9152youxi.cn/gtarnfadxt.html

C#:   do { i++; } while (i < 10);
来源：http://hz.chenjidiqi.icu/gtxlmqsxxa.html

[B09] break 与 continue
来源：http://hz.yonumen.top/gtjftvvakt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jlsjyb.cn/gtjvstwdbf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yuxming.cn/gtmsbxaddb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gotoacloud.top/gtghxaakwd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.9152youxi.cn/gtyzzclrus.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtuwskmdwx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.9152youxi.cn/gtecvwxkit.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.aizwys.cn/gtvkvgfoip.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.9152youxi.cn/gtjsfrscdn.html

[B10] 遍历同时拿索引
来源：http://hz.ehwqpu.com/gtmacpyilr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.svipenyu.cn/gtudtavxyk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.sufxvd.cn/gtfdghxlmj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jinqigfzy.top/gtopflxgwo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhijiandao.cn/gtzyofspua.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.0kj1m.cn/gtixuvjybp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hongshengwenyu.top/gtwzzjniaq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shanyushiyangkeji.top/gtwfitoblu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.andypj.xyz/gtrayyjyfz.html

[B11] 生成数字序列 / 区间
来源：http://hz.guannengcc.top/gtulwdgojy.html

Py:   list(range(0, 10, 2))
来源：http://hz.jqgufenzy.top/gtyfjvxjnn.html

PHP:  range(0, 10, 2);
来源：http://hz.yangfankeji.com/gtzdkkvkwx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.svipenyu.cn/gtwklbbkbg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gzhubu.top/gtuxieqlqf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.nanxinkj.top/gtofuufkrz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cqqwz.cn/gtmosoegzf.html

Ruby: (0...10).step(2).to_a
来源：http://hz.daria6918.cn/gtkhypztwm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yonumen.top/gtfbwfzaja.html

[B12] 跳出多层循环
来源：http://hz.iojbl.cn/gtltqqvdod.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gotoacloud.top/gtuyczoaht.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cqqwz.cn/gthxbfvolw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sysykeji.top/gtyyufvaqe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtzrvowxyj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gtvwkyolsc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.iojbl.cn/gtsbtcefuk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jyoumei.cn/gtrboxazhk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jinqigufen.top/gtaggkdhpv.html

[B13] 判断是否为数字
来源：http://hz.birdmap.top/gtbaghjyib.html

Py:   isinstance(x, (int, float))
来源：http://hz.shuidangran.top/gtybfjgfel.html

PHP:  is_numeric($x)
来源：http://hz.316326.xyz/gtpkfaxtmd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinqigufen.top/gtpewpkexi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guowangkeji.top/gtetxvledb.html

Java: x instanceof Number
来源：http://hz.haohaochexian.top/gtcxhdxrct.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ehwqpu.com/gtgvkmetfp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.kuanghao11.cn/gtcgvwgbyi.html

C#:   x is int or double or decimal
来源：http://hz.cqqwz.cn/gtcaeepiko.html

[B14] 判断值是否在集合内
来源：http://hz.vqdsnc.cn/gtaqhflmai.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.nwbrower.top/gtfiybqwwq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ywan-chungtsiang.top/gtugbxytto.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigfzy.top/gtpdkpwgoi.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.vqdsnc.cn/gtzqvbafyi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gzhubu.top/gtbivgwwju.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cashguo.top/gtcksfwoxz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gotoacloud.top/gtkeadsnei.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ywan-chungtsiang.top/gtdjfaedkz.html

[B15] 布尔运算与取反
来源：http://hz.tianlin.xyz/gtxfloougu.html

Py:   a and b or not c
来源：http://hz.cqqwz.cn/gtosnsbbvw.html

PHP:  $a && $b || !$c
来源：http://hz.kuanghao11.cn/gtyedfntqp.html

JS:   a && b || !c
来源：http://hz.meibo888.top/gtallloxmr.html

TS:   a && b || !c
来源：http://hz.chenzaomai.com/gtdtgfruyd.html

Java: a && b || !c
来源：http://hz.yvedp.cn/gtkmsjpuxo.html

Go:   a && b || !c
来源：http://hz.chenzaomai.com/gtiemmnday.html

Ruby: a && b || !c
来源：http://hz.shanyushiyangtech.top/gthecilluz.html

C#:   a && b || !c
来源：http://hz.chenlongwang.top/gtjtzrzehs.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.wangshuangyany.cn/gtxjkwhovr.html

Py:   if not data: return
来源：http://hz.hnxiangtu.top/gthkrwgwyl.html

PHP:  if (!$data) { return; }
来源：http://hz.cheryme.top/gtdzkharwy.html

JS:   if (!data) return;
来源：http://hz.jqgufenzy.top/gtefstgtqq.html

TS:   if (!data) return;
来源：http://hz.0kj1m.cn/gtuurlhaoc.html

Java: if (data == null) return;
来源：http://hz.yongpay.top/gtxhfuxzds.html

Go:   if data == nil { return }
来源：http://hz.xuanzx.com/gtwqxtujbc.html

Ruby: return if data.nil?
来源：http://hz.ivvv.top/gtnivavhqy.html

C#:   if (data == null) return;
来源：http://hz.yuanzhike.top/gtmzrrwqov.html

================================================================================
来源：http://hz.svipenyu.cn/gtvnytmbjc.html

C. 函数与作用域
来源：http://hz.ivvv.top/gtcmnqedgq.html

================================================================================
来源：http://hz.wangdashe.top/gtcjqdjvky.html

[C01] 定义函数
来源：http://hz.hfpthk.cn/gtdejjuvis.html

Py:   def add(a, b): return a + b
来源：http://hz.316326.xyz/gtthwoxmin.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtjokqdgrl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cheryme.top/gtgxneliot.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258888.top/gtpdgoyfat.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtefmtijld.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hfpthk.cn/gtyjavggby.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yongpay.top/gtdpcbadzk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhengqikj.top/gtrxvophmo.html

[C02] 默认参数
来源：http://hz.pycfn.com/gtinuwrzmn.html

Py:   def greet(name="World"): return name
来源：http://hz.ydzc1.top/gtldldziqn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ywan-chungtsiang.top/gtmdfckdts.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtqxwrqriy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yongpay.top/gtsvaaktuf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yj20258.top/gtfxoiiqdj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jinqigfzy.top/gtiuwwrplt.html

Ruby: def greet(name = "World") = name
来源：http://hz.ydjk.org.cn/gtifuaoicf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.quarkkingdee.top/gtbidgvyoe.html

[C03] 可变参数
来源：http://hz.9152youxi.cn/gtctakgbzy.html

Py:   def total(*args): return sum(args)
来源：http://hz.xuanzx.com/gtucvjzgch.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hammf.cn/gtxkhcmbjx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangshuangyany.cn/gtvliqzfab.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.svipenyu.cn/gtwkofthfj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.guowangkeji.top/gtreaoifqc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xingfuxueyuan.xyz/gtpzcpikje.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.guannengcc.top/gtqnrarwck.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.wangshuangyany.cn/gtjflkeyou.html

[C04] 命名参数 / 关键字参数
来源：http://hz.birdmap.top/gtwrdygzma.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cdnleiting.top/gtzocykscy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jiagoushi.top/gtakgcnyuz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.guowangkeji.top/gtjifxscax.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cucudq.cn/gtwgvzkkmn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhixingplan.top/gtarafsvje.html

Go:   // 无：用配置结构体参数
来源：http://hz.hongshengwenyu.top/gtwprwldlg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xylfe.cn/gtkhjasszu.html

C#:   f(a: 1, b: 2)
来源：http://hz.gzhubu.top/gtsdpocwnh.html

[C05] 返回多个值
来源：http://hz.c1oappe.top/gthtfryaki.html

Py:   return a, b
来源：http://hz.cucudq.cn/gtoymmhpbb.html

PHP:  return [$a, $b];
来源：http://hz.chenjidiqi.icu/gttsnezkrf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zycfv.cn/gtaviyfkor.html

TS:   return { a, b };
来源：http://hz.cheryme.top/gtyeffvfys.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.316326.xyz/gtbaqraeyr.html

Go:   return a, b
来源：http://hz.yvedp.cn/gtxfqzlaje.html

Ruby: return a, b
来源：http://hz.jqgufenzy.top/gtnynjstoa.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yueranfly.top/gtbyueyrbv.html

[C06] 匿名函数 / lambda
来源：http://hz.jinghuilouyu.cn/gtzfeiequf.html

Py:   square = lambda x: x * x
来源：http://hz.guowangkeji.top/gtxthfcnty.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ppjwa.cn/gtorjovkjq.html

JS:   const square = x => x * x;
来源：http://hz.quarkkingdee.top/gtroqylfhk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gotoacloud.top/gtprvaduhg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.iojbl.cn/gtnpidpwbk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shanyushiyangkeji.top/gtkbhxfulr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xuanzx.com/gtmpepkvqa.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shzxlz.cn/gtjkwsdmwk.html

[C07] 把函数作为参数传入
来源：http://hz.redwolf501.top/gthbdjwjav.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenzaomai.com/gthrpozrjy.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.pycfn.com/gtyzfovkwr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sxryk.cn/gtpnzarnvs.html

TS:   arr.map(String)
来源：http://hz.52xcode.cn/gtnjhfneut.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gotoacloud.top/gticrqvmsw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhiwuduotai.top/gttowxquah.html

Ruby: arr.map(&:upcase)
来源：http://hz.nwbrower.top/gtxzorpvkh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hnqzz.top/gtayulhodd.html

[C08] 闭包
来源：http://hz.gogol.net.cn/gtswcqxpsm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jiagoushi.top/gtcdakwilg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenzaomai.com/gttbruviux.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinyuanbaomall.cn/gtriizmiip.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtmmargqnz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cdnleiting.top/gtogtgqefz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhongyouzk.top/gtncqqwgsq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.smart0.xyz/gtbhguzbhp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhixingplan.top/gtzbadffms.html

[C09] 递归
来源：http://hz.xingfuxueyuan.xyz/gtmqdeiotb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xylfe.cn/gtcqqsnvvf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.svipenyu.cn/gtoyjwcijx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sweek.top/gtbkcffesa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtvsaqfpfs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.havefunace.top/gtczeabjnn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hnxiangtu.top/gtvaejcekl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.haohaochexian.top/gtlxpyyqrh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.feifeiyinyue.top/gtdjpfegpb.html

[C10] 变量作用域
来源：http://hz.nanxinkj.top/gttohdmvny.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dashuyun.cn/gtcuvinjtn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tianlin.xyz/gtwclvstin.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhongyouzk.top/gtepusffrc.html

TS:   同 JS
来源：http://hz.cqqwz.cn/gtnlfnoxca.html

Java: 方法内为块级作用域
来源：http://hz.hongshengwenyu.top/gtffxsnodb.html

Go:   花括号块级作用域
来源：http://hz.zhaomingkeji.xyz/gtdyfiodox.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhijiandao.cn/gtqxtyathx.html

C#:   块级作用域
来源：http://hz.tanke756.top/gtmpejdwpr.html

[C11] 模块导入与导出
来源：http://hz.ywan-chungtsiang.top/gtkqvxsbaa.html

Py:   from module import func
来源：http://hz.iojbl.cn/gtljolvswv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenzaomai.com/gtbyotlafr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shzxlz.cn/gthlkrqnfk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.bjfxy.top/gtwpaxjdic.html

Java: import java.util.List;
来源：http://hz.smart0.xyz/gtwqpnamjr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydzc1.top/gtfssonggr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ppjwa.cn/gtbcgjtnex.html

C#:   using System.Text;
来源：http://hz.jinqigfzy.top/gtwmlbkebr.html

[C12] 立即执行函数 IIFE
来源：http://hz.sxryk.cn/gtynfgyfir.html

Py:   (lambda: print("run"))()
来源：http://hz.daria6918.cn/gtshxaphgi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ivvv.top/gtocezftmo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shangyingyoupin.top/gtjdsqeonb.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nanxinkj.top/gtbypnpidf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sweek.top/gtmayuzjfm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yuxming.cn/gteazmgpbc.html

Ruby: -> { puts "run" }.call
来源：http://hz.wangshuangyany.cn/gtprxstuoc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cqqwz.cn/gtwetbhqlv.html

[C13] 类型声明 / 类型注解
来源：http://hz.hnxiangtu.top/gtbflmqzzn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nwbrower.top/gtkfkepnzn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gtonqydhxb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hywenlv.cn/gtamlhlfej.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shzxlz.cn/gtfhybzqcg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtweiymjrc.html

Go:   func add(a, b int) int
来源：http://hz.c1oappe.top/gtcvtlyeqj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hywenlv.cn/gtiueimuto.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.iojbl.cn/gtqxleptda.html

[C14] 泛型函数
来源：http://hz.hnqzz.top/gteqmcgzmp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.9152youxi.cn/gttyrenvrf.html

PHP:  // 无泛型
来源：http://hz.hysaishi.cn/gtrwduxxix.html

JS:   // 无泛型
来源：http://hz.xziqi.cn/gtjclvwggx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xziqi.cn/gtmeryrpbm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ydjk.org.cn/gtrhtawhqd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ppjwa.cn/gtlxtamexh.html

Ruby: # 无泛型
来源：http://hz.iojbl.cn/gtltallxrn.html


<!-- 参考信息 -->