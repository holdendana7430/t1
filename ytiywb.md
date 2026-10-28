代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://hz.jianghu66.top/gtssakesun.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ppjwa.cn/gtrgfyurtr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yangfankeji.com/gtrjpguvjo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.kuanghao11.cn/gtmpnimnvy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.9152youxi.cn/gtwbyaxtum.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.nanxuanxn.top/gtnvubyrry.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.nwbrower.top/gtweekages.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ppjwa.cn/gtuttcwewm.html

[A26] 类型转换总览
来源：http://hz.tanke756.top/gtceebzvnv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.nanxinkj.top/gtwctxycvk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yueranfly.top/gtoelveako.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hongshengwenyu.top/gterxlllsl.html

TS:   Number() String() Boolean() x as number
来源：http://hz.vqdsnc.cn/gtselcsuco.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.chenjidiqi.icu/gtmioghmvb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.mhx1999.top/gtvxqbnszw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yj20258888.top/gtgjplqsme.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.quarkkingdee.top/gtmawmzefd.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtsztrkkhm.html

B. 流程控制
来源：http://hz.0kj1m.cn/gtlrvjsuna.html

================================================================================
来源：http://hz.cdnleiting.top/gtzuilxkcq.html

[B01] 条件判断 if / else
来源：http://hz.cdnleiting.top/gttwfppbwy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.c1oappe.top/gtowquwdxr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.9152youxi.cn/gtzxtwcwld.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.pengpengdd.cyou/gtfhpxttyd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gtvuoqrqsy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xinyue.icu/gtjhnrowiq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.gaohongyu789.top/gtmxpewiun.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.tianlin.xyz/gtujugzlet.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.tian-w.cn/gtajxgalzs.html

[B02] 多分支 else if / elif
来源：http://hz.jinyuanbaomall.cn/gtckjmiemy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.9152youxi.cn/gtdcsaolgi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhongyouzk.top/gtlmbmalnn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.9152youxi.cn/gtztfhhncs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtrunivnok.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ppjwa.cn/gtljyjwvtr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jqgufenzy.top/gtdvrayhhv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.daxiang520.top/gttyatqvac.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xinyue.icu/gttdwrsbmd.html

[B03] switch / match / case
来源：http://hz.shzxlz.cn/gtvwoqpvog.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.shangyingyoupin.top/gtlbxpwpbz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ppjwa.cn/gtvsiiawdw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cucudq.cn/gtahfhpjwq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sufxvd.cn/gtqtzsqlkg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.xingfuxueyuan.xyz/gtdvzrxqev.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hfpthk.cn/gtlfgfczbc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhoulong.xyz/gtsjpdorwo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.tian-w.cn/gtensvngrn.html

[B04] for 计数循环
来源：http://hz.cdnleiting.top/gtnqffzqyo.html

Py:   for i in range(10): print(i)
来源：http://hz.svipenyu.cn/gtbcfndwge.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.gaohongyu789.top/gtmlkdmqev.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yongpay.top/gtksuewlsx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.smart0.xyz/gtrrdzjgve.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jyoumei.cn/gtmdsukzee.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.fzhhl.top/gtusojcbku.html

Ruby: 10.times { |i| puts i }
来源：http://hz.tianlin.xyz/gtvydgheuz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.fzhhl.top/gtzsxqqhoz.html

[B05] 遍历数组 / 列表
来源：http://hz.zhoulong.xyz/gtlqessovu.html

Py:   for item in arr: print(item)
来源：http://hz.316326.xyz/gtccyikcxk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.nanxinkj.top/gtbvihqqpw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xuanzx.com/gtpulflzqc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xziqi.cn/gttkxssuie.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhengqikj.top/gtlkyoxhoy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.xinyue.icu/gtgcvnials.html

Ruby: arr.each { |item| puts item }
来源：http://hz.tianlin.xyz/gtpbmfaypz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.quarkkingdee.top/gtybjobgra.html

[B06] 遍历字典 / 对象
来源：http://hz.xylfe.cn/gtrrjakibs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.guannengcc.top/gtdjehwzgy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.feifeiyinyue.top/gtjinxtjnz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hnqzz.top/gtxebksxfo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hnqzz.top/gtrnnhyklq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.pengpengdd.cyou/gtyakdgeuw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.wangshuangyany.cn/gtidpliyzk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.kuanghao11.cn/gtsqvujlde.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.0kj1m.cn/gtibjvgxts.html

[B07] while 循环
来源：http://hz.ywan-chungtsiang.top/gtxeabzyli.html

Py:   while i < 10: i += 1
来源：http://hz.gogol.net.cn/gtjlqweubz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.hongshengwenyu.top/gtwpvddajv.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtvanqneym.html

TS:   while (i < 10) { i++; }
来源：http://hz.meibo888.top/gtetcnisgr.html

Java: while (i < 10) { i++; }
来源：http://hz.yueranfly.top/gturyjxfnx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.svipenyu.cn/gtxtwgesyp.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnqzz.top/gtbtubffpu.html

C#:   while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gtirisjekp.html

[B08] do-while（至少执行一次）
来源：http://hz.dianchejie.cn/gtgqtziyhy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hfpthk.cn/gtfnexavuq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zdqjudy.top/gtulbbvcpi.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hysaishi.cn/gtyvyerzkh.html

TS:   do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gthiboacmu.html

Java: do { i++; } while (i < 10);
来源：http://hz.nanxinkj.top/gtokrfyjtf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.fengsongda.top/gtksddahqa.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.sysykeji.top/gtcguloewf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.chenjidiqi.icu/gtwolhobzs.html

[B09] break 与 continue
来源：http://hz.fengsongda.top/gtjojdubkr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gogol.net.cn/gtvbsrwces.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ivvv.top/gtrghrylni.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hfpthk.cn/gtmfvbpmtl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pengpengdd.cyou/gtlzqabuoz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gtqcjkivjf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.sysykeji.top/gttxlivrzg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.smart0.xyz/gttevzxlsx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj202588.top/gtzpjjfxlv.html

[B10] 遍历同时拿索引
来源：http://hz.zhaomingkeji.xyz/gtkrrbcssg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.nanxuanxn.top/gthlzhvtxn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xingfuxueyuan.xyz/gtxpcjcmhl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.fzhhl.top/gtxsewiptx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hammf.cn/gtjeykggqe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xylfe.cn/gtacpfapfp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj202588.top/gtgeqispkn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.chenzaomai.com/gtxjqlgkce.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.haohaochexian.top/gtuljhwydq.html

[B11] 生成数字序列 / 区间
来源：http://hz.dianchejie.cn/gtfebhaing.html

Py:   list(range(0, 10, 2))
来源：http://hz.kuanghao11.cn/gtkrdjftax.html

PHP:  range(0, 10, 2);
来源：http://hz.aibaodan.cn/gtkmbfzlxl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xinyue.icu/gtziqhynfn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zycfv.cn/gtayeidmpp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.0kj1m.cn/gtcojqzrrn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zdqjudy.top/gtcbwxrtla.html

Ruby: (0...10).step(2).to_a
来源：http://hz.tian-w.cn/gtgaadukez.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhixingplan.top/gtohqabaco.html

[B12] 跳出多层循环
来源：http://hz.dianchejie.cn/gtnbqqtitb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.wangshuangyany.cn/gtiknfbdxo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.mhx1999.top/gtuauvjsaw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gtxhhqtjvm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.0kj1m.cn/gtualijgxu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gtgzrboihy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cucudq.cn/gtvspherei.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.c1oappe.top/gtwezchgkz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.daria6918.cn/gtzwueybej.html

[B13] 判断是否为数字
来源：http://hz.quarkkingdee.top/gtkorowppc.html

Py:   isinstance(x, (int, float))
来源：http://hz.shangyingyoupin.top/gtbifwtrlb.html

PHP:  is_numeric($x)
来源：http://hz.zhaomingkeji.xyz/gtayjrbmbs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenzaomai.com/gtxzidfwlm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.snrcjt.cn/gtpbvqebeb.html

Java: x instanceof Number
来源：http://hz.zdqjudy.top/gtzxfvzcaz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jqgufenzy.top/gtqqaibsee.html

Ruby: x.is_a?(Numeric)
来源：http://hz.chenzaomai.com/gtewwebinh.html

C#:   x is int or double or decimal
来源：http://hz.316326.xyz/gtfmdyesku.html

[B14] 判断值是否在集合内
来源：http://hz.zhixingplan.top/gtnaovlwal.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhixingplan.top/gtxntseyhp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jiagoushi.top/gtkdxremep.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhongyouzk.top/gtijhybjmr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.birdmap.top/gtcuuablde.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.wangshuangyany.cn/gtdzzykcym.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.gotoacloud.top/gtmnchcdbn.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.pengpengdd.cyou/gtdgictexz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cucudq.cn/gtyomfejyg.html

[B15] 布尔运算与取反
来源：http://hz.dianchejie.cn/gtpefhhzij.html

Py:   a and b or not c
来源：http://hz.hysaishi.cn/gtuqwwhqne.html

PHP:  $a && $b || !$c
来源：http://hz.yonumen.top/gtqcxicofo.html

JS:   a && b || !c
来源：http://hz.hfpthk.cn/gtuxkqgpzn.html

TS:   a && b || !c
来源：http://hz.kuanghao11.cn/gtyyimiptv.html

Java: a && b || !c
来源：http://hz.iojbl.cn/gtagzzvocf.html

Go:   a && b || !c
来源：http://hz.jyoumei.cn/gtchbysmii.html

Ruby: a && b || !c
来源：http://hz.yvedp.cn/gtugzftllz.html

C#:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtvtdjcxxs.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.snrcjt.cn/gtqsaxkvhk.html

Py:   if not data: return
来源：http://hz.ydzc1.top/gttanqvnyu.html

PHP:  if (!$data) { return; }
来源：http://hz.chenjidiqi.icu/gtdlimxrjc.html

JS:   if (!data) return;
来源：http://hz.shangyingyoupin.top/gtaxqctyun.html

TS:   if (!data) return;
来源：http://hz.tianlin.xyz/gtsxavhadi.html

Java: if (data == null) return;
来源：http://hz.jlsjyb.cn/gtszrjense.html

Go:   if data == nil { return }
来源：http://hz.cucudq.cn/gtrfpbhcct.html

Ruby: return if data.nil?
来源：http://hz.redwolf501.top/gtmrnncpdi.html

C#:   if (data == null) return;
来源：http://hz.yj202588.top/gtolevirob.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtvvhphuxp.html

C. 函数与作用域
来源：http://hz.haohaochexian.top/gtgtaevhwa.html

================================================================================
来源：http://hz.xylfe.cn/gtaywyvfpz.html

[C01] 定义函数
来源：http://hz.jqgfzy.top/gtizwzumjz.html

Py:   def add(a, b): return a + b
来源：http://hz.yongpay.top/gtgvbsdkxz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtvpfwodxa.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.daria6918.cn/gtugdjawce.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hysaishi.cn/gttqayrwmj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.havefunace.top/gtcloqdcua.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxinkj.top/gtcotyzhgu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sweek.top/gtcvnygzbm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gtbmwyunlw.html

[C02] 默认参数
来源：http://hz.dashuyun.cn/gtwfwmtcyv.html

Py:   def greet(name="World"): return name
来源：http://hz.yvedp.cn/gtbqreoxbs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hnqzz.top/gtawzhphef.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gtjvuoyfae.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hywenlv.cn/gtpfsutsrd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.quarkkingdee.top/gtqnwcscyr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.pengpengdd.cyou/gtemwvzbze.html

Ruby: def greet(name = "World") = name
来源：http://hz.hnxiangtu.top/gtxmkraxso.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hywenlv.cn/gtlcnvjsit.html

[C03] 可变参数
来源：http://hz.aibaodan.cn/gtmgricphk.html

Py:   def total(*args): return sum(args)
来源：http://hz.jiagoushi.top/gtitfjlpnz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.redwolf501.top/gtkoilgeqd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daxiang520.top/gttqnkwacg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ywan-chungtsiang.top/gtsfgvgroa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zycfv.cn/gtcnhvlxsa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.dashuyun.cn/gtjdwkjete.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.daxiang520.top/gtgdfxmzns.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hnqzz.top/gtfjbahdlv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.aibaodan.cn/gtkwcybupr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhongyouzk.top/gtopowaqzj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.daxiang520.top/gtbzccamva.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hywenlv.cn/gtkjbmbhzy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jiagoushi.top/gtqbwozygv.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shanyushiyangtech.top/gtuxwavvbt.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhixingplan.top/gtwzyaeakh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtbuapavvd.html

C#:   f(a: 1, b: 2)
来源：http://hz.yanxiufei.cn/gtuppkwsqx.html

[C05] 返回多个值
来源：http://hz.zhaomingkeji.xyz/gtvqcykroj.html

Py:   return a, b
来源：http://hz.redwolf501.top/gtgkhgvjwg.html

PHP:  return [$a, $b];
来源：http://hz.aizwys.cn/gtmudrqygj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.fengsongda.top/gtsdznrite.html

TS:   return { a, b };
来源：http://hz.aibaodan.cn/gtrmvfshay.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhaomingkeji.xyz/gtjryzeiax.html

Go:   return a, b
来源：http://hz.yonumen.top/gtieulfdly.html

Ruby: return a, b
来源：http://hz.vqdsnc.cn/gtaovepsgd.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sweek.top/gtckbznuoy.html

[C06] 匿名函数 / lambda
来源：http://hz.birdmap.top/gtfvzmammh.html

Py:   square = lambda x: x * x
来源：http://hz.tanke756.top/gtceahxlwq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yueranfly.top/gtrwudlftn.html

JS:   const square = x => x * x;
来源：http://hz.zdqjudy.top/gtfluslndo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jianghu66.top/gtjdygwune.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.fzhhl.top/gtsatsigft.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xingfuxueyuan.xyz/gtigniscud.html

Ruby: square = ->(x) { x * x }
来源：http://hz.pycfn.com/gthvhgfclf.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jlsjyb.cn/gtritsdvwe.html

[C07] 把函数作为参数传入
来源：http://hz.meibo888.top/gtyaizbuxe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yj202588.top/gtidekgype.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sweek.top/gtnurhfble.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.iojbl.cn/gtcoiuupxu.html

TS:   arr.map(String)
来源：http://hz.ydjk.org.cn/gtuamshizr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yj202588.top/gtefvdbjsm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangkeji.top/gtwqdsztuz.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhixingplan.top/gtaqukedjf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hnqzz.top/gtrnvekeya.html

[C08] 闭包
来源：http://hz.hammf.cn/gtbkfjywii.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yueranfly.top/gthetlzqbt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cheryme.top/gtjotoucau.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtrrtwnciw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gthbulxxxg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yj20258888.top/gtzpolqief.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhijiandao.cn/gtoimywamq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xuetiantiany.cn/gtamyyasel.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtcahtdxkd.html

[C09] 递归
来源：http://hz.yj20258888.top/gtgfwvbvzk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gaohongyu789.top/gtmwwkzstz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.9152youxi.cn/gtyjaifskm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guannengcc.top/gtqefhvuam.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtkfsklhgv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tian-w.cn/gtfcuzffna.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.52xcode.cn/gthloaaswq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.kuanghao11.cn/gtlcwjoftf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sysykeji.top/gtwsogpqqi.html

[C10] 变量作用域
来源：http://hz.yj20258888.top/gtfvzavbiu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xingfuxueyuan.xyz/gthegdewvh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hysaishi.cn/gtvesalsku.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jiagoushi.top/gthsfoqeih.html

TS:   同 JS
来源：http://hz.hnxiangtu.top/gtmblkgxbc.html

Java: 方法内为块级作用域
来源：http://hz.shanyushiyangkeji.top/gtkyheczcp.html

Go:   花括号块级作用域
来源：http://hz.iojbl.cn/gtjtrukfhp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.daxiang520.top/gtvygnnprv.html

C#:   块级作用域
来源：http://hz.yanxiufei.cn/gtnswzfvym.html

[C11] 模块导入与导出
来源：http://hz.cdnleiting.top/gtimxffzru.html

Py:   from module import func
来源：http://hz.tian-w.cn/gtssrnrndv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shanyushiyangkeji.top/gtxxgtycxf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shangyingyoupin.top/gtlnftycsf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.chenlongwang.top/gtlrmsuzuh.html

Java: import java.util.List;
来源：http://hz.kuanghao11.cn/gtfgvrvoqm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gaohongyu789.top/gtjapjbmhu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.haohaochexian.top/gtdpehcrjp.html

C#:   using System.Text;
来源：http://hz.gogol.net.cn/gthsgsyxft.html

[C12] 立即执行函数 IIFE
来源：http://hz.snrcjt.cn/gtbxiwrwqo.html

Py:   (lambda: print("run"))()
来源：http://hz.tianlin.xyz/gtkatqjvgt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sufxvd.cn/gtizwplikj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.nwbrower.top/gtawgrydxl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gtxhdwqmuy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.kuanghao11.cn/gtcvyairbq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yj20258.top/gtodcbflsp.html

Ruby: -> { puts "run" }.call
来源：http://hz.gotoacloud.top/gtsvpdxtmd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.birdmap.top/gtqsokxfmx.html

[C13] 类型声明 / 类型注解
来源：http://hz.tanke756.top/gtgxruofhn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yj202588.top/gtootsaich.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtgpuaqtxq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jqgufenzy.top/gthmweckxe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aibaodan.cn/gtywqajuuh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtsvwcyqdz.html

Go:   func add(a, b int) int
来源：http://hz.smart0.xyz/gtjpxxcyjz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yongpay.top/gtjwnayskl.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xinyue.icu/gtnovfrchl.html

[C14] 泛型函数
来源：http://hz.jiagoushi.top/gtrzlzpbrb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gzhubu.top/gthvzspqgo.html

PHP:  // 无泛型
来源：http://hz.nanxinkj.top/gtdgmchecl.html

JS:   // 无泛型
来源：http://hz.cqqwz.cn/gtcdftuabg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.fengsongda.top/gtsxrpmrpr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.nwbrower.top/gtxxkrqsyv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.316326.xyz/gtusibqynj.html

Ruby: # 无泛型
来源：http://hz.ehwqpu.com/gtorkeinlk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.aibaodan.cn/gtmmddckss.html

[C15] 解构 / 展开参数
来源：http://hz.zhengqikj.top/gtdcnuipbl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fzhhl.top/gtscpcquaq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.kuanghao11.cn/gtaaybeohj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtwjablpsv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dianchejie.cn/gthismrxtw.html

Java: // 无解构
来源：http://hz.ppjwa.cn/gtjuaxyags.html

Go:   // 无解构
来源：http://hz.snrcjt.cn/gtvoxpnqdq.html


<!-- 参考信息 -->