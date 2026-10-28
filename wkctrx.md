代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://hz.hongshengwenyu.top/gtjjfxbyjv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.fengsongda.top/gtozrwzgrh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.shuidangran.top/gtutqgeces.html

[A25] 字符串比较
来源：http://hz.zhengqikj.top/gtjredmxin.html

Py:   s1 == s2; s1 != s2
来源：http://hz.pengpengdd.cyou/gtwazaoiey.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.nanxuanxn.top/gtzvqtkeir.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.wangshuangyany.cn/gtyixispku.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hywenlv.cn/gtwkqztmzd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yuxming.cn/gtnumvtzbe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jlsjyb.cn/gtvdmursyt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yangfankeji.com/gtauqurqxc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.gaohongyu789.top/gtlojaxvhm.html

[A26] 类型转换总览
来源：http://hz.shanyushiyangtech.top/gtwhkaizwr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.chenzaomai.com/gtrnrjvfah.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.redwolf501.top/gtuavxtnvq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.daria6918.cn/gtcjquhmhd.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jyoumei.cn/gtwxrpdzeq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhengqikj.top/gtsivdmvoa.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.hongshengwenyu.top/gtxmacsdrs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.shuidangran.top/gtgwkralov.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ywan-chungtsiang.top/gtjyaquskp.html

================================================================================
来源：http://hz.yj202588.top/gtuamquxwi.html

B. 流程控制
来源：http://hz.chenjidiqi.icu/gttsjcxtjq.html

================================================================================
来源：http://hz.zycfv.cn/gtorzgxtpk.html

[B01] 条件判断 if / else
来源：http://hz.zhijiandao.cn/gtafszoysv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jqgfzy.top/gtipdtegng.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.smart0.xyz/gtdkqmawfd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.dianchejie.cn/gtsbbooydr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.redwolf501.top/gtdbtzpplf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.daxiang520.top/gtllbjvncs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ivvv.top/gtgrhuoawn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hysaishi.cn/gtamtcoxmw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.xziqi.cn/gtpmqarcxr.html

[B02] 多分支 else if / elif
来源：http://hz.guowangkeji.top/gtckxpzffb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.nanxinkj.top/gthirknshs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.gogol.net.cn/gteyivjriy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258.top/gtlchkawpo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinghuilouyu.cn/gtmuxntvgw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.andypj.xyz/gtftrbamzb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.gogol.net.cn/gtooiqhblh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhiwuduotai.top/gtoxtmwbsg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gtsfdtwtef.html

[B03] switch / match / case
来源：http://hz.daria6918.cn/gtkrqolcng.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.redwolf501.top/gtgehylxoi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.mhx1999.top/gtgscnhird.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.quarkkingdee.top/gtszqietie.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hywenlv.cn/gtravxlldw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.sxryk.cn/gtcmqowmln.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhixingplan.top/gtvygwkcrv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ywan-chungtsiang.top/gtqykebkmx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.316326.xyz/gtpwjjvpfh.html

[B04] for 计数循环
来源：http://hz.cqqwz.cn/gtbyxohwwp.html

Py:   for i in range(10): print(i)
来源：http://hz.sufxvd.cn/gtpknbpqsh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.gzhubu.top/gthviydsbl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.nanxinkj.top/gtafljjbfc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xinyue.icu/gtlpwsctps.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.wangdashe.top/gtymnapbub.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hnxiangtu.top/gtcsiwavew.html

Ruby: 10.times { |i| puts i }
来源：http://hz.cashguo.top/gtbnmgpjbq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yuanzhike.top/gtkedjtvdp.html

[B05] 遍历数组 / 列表
来源：http://hz.316326.xyz/gtiqlhmxme.html

Py:   for item in arr: print(item)
来源：http://hz.vqdsnc.cn/gttosrfuvr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.dianchejie.cn/gtfihrdzst.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ywan-chungtsiang.top/gtaizsarmk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zycfv.cn/gtkkkfbgte.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xinyue.icu/gtxgfclflo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.daxiang520.top/gtolvlwyno.html

Ruby: arr.each { |item| puts item }
来源：http://hz.nanxuanxn.top/gtrflszhly.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xylfe.cn/gtyaozkqbh.html

[B06] 遍历字典 / 对象
来源：http://hz.iojbl.cn/gtrksxowoe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yj20258888.top/gtgggsynxn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.zhixingplan.top/gtesnfufiu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinyuanbaomall.cn/gtwgxdcxmm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydzc1.top/gtmhhmkztx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.sysykeji.top/gtxwbupyui.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.9152youxi.cn/gtuzhgnuqg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ydzc1.top/gtezspvrnw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.ivvv.top/gtpktyprou.html

[B07] while 循环
来源：http://hz.kuanghao11.cn/gtkmfxcqjm.html

Py:   while i < 10: i += 1
来源：http://hz.yongpay.top/gtskiakacc.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.hysaishi.cn/gtgyirejpp.html

JS:   while (i < 10) { i++; }
来源：http://hz.jinqigfzy.top/gthpeoswvb.html

TS:   while (i < 10) { i++; }
来源：http://hz.jqgfzy.top/gtjhzrbswt.html

Java: while (i < 10) { i++; }
来源：http://hz.vqdsnc.cn/gtuleblijf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yanxiufei.cn/gtjwoyuqcb.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ywan-chungtsiang.top/gtxeutughz.html

C#:   while (i < 10) { i++; }
来源：http://hz.dashuyun.cn/gttaxdptzm.html

[B08] do-while（至少执行一次）
来源：http://hz.andypj.xyz/gthxtrawnc.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.sysykeji.top/gtywpqndsi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jqgfzy.top/gtmlhjxncj.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gaohongyu789.top/gtbgtgdtcp.html

TS:   do { i++; } while (i < 10);
来源：http://hz.mhx1999.top/gtqorvjwds.html

Java: do { i++; } while (i < 10);
来源：http://hz.shanyushiyangtech.top/gttgfzdxtl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.daxiang520.top/gtkqmmykhy.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.sufxvd.cn/gtlkwgxgnl.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gtjnaqbenh.html

[B09] break 与 continue
来源：http://hz.ehwqpu.com/gtvruovoii.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.fzhhl.top/gtbxuajbxj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtbrctmssm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.meibo888.top/gtxqjpsfvz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtqmyzuufv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tianlin.xyz/gtqiuhoiyq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.9152youxi.cn/gtdlwzuijo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhixingplan.top/gtiaevxmsv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtcamndgbb.html

[B10] 遍历同时拿索引
来源：http://hz.tian-w.cn/gthclyugnw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.9152youxi.cn/gtbuyggvmz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.shanyushiyangtech.top/gtwtjghgnz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xuetiantiany.cn/gtnvaezcuu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.pengpengdd.cyou/gtnhysukdm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.kuanghao11.cn/gtgahtnnnm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.havefunace.top/gtpnhjzipr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yj20258.top/gtvsrbjvnm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ydjk.org.cn/gtpjehfzwq.html

[B11] 生成数字序列 / 区间
来源：http://hz.ywan-chungtsiang.top/gtilfgjucn.html

Py:   list(range(0, 10, 2))
来源：http://hz.hysaishi.cn/gttjnbwxgl.html

PHP:  range(0, 10, 2);
来源：http://hz.fengsongda.top/gtnqqqfjns.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cashguo.top/gtckfjomzb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangdashe.top/gtfwiywxiv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.snrcjt.cn/gtibjafbpp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.snrcjt.cn/gtmvtrgksr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sufxvd.cn/gtrzxorpuq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.guowangkeji.top/gtuaqavvdf.html

[B12] 跳出多层循环
来源：http://hz.gotoacloud.top/gtfmvjqgfk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hongshengwenyu.top/gtcrdkoqzs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sufxvd.cn/gtqoyjhzgq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.andypj.xyz/gtjffjwvci.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fengsongda.top/gtnqzztxvd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.dashuyun.cn/gtjyqlwzry.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.9152youxi.cn/gtgfrzpvjy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jqgfzy.top/gtintxygsv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.sysykeji.top/gtrztjghnf.html

[B13] 判断是否为数字
来源：http://hz.gaohongyu789.top/gtitfsqbkb.html

Py:   isinstance(x, (int, float))
来源：http://hz.yuanzhike.top/gtqcvzxlvg.html

PHP:  is_numeric($x)
来源：http://hz.jqgfzy.top/gtdyadybte.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aibaodan.cn/gtcndflyel.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.birdmap.top/gtimsjfoao.html

Java: x instanceof Number
来源：http://hz.yj202588.top/gtsuqclazd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuanzx.com/gtuihkayue.html

Ruby: x.is_a?(Numeric)
来源：http://hz.sweek.top/gtxvfexqru.html

C#:   x is int or double or decimal
来源：http://hz.yuxming.cn/gtqxhfzjax.html

[B14] 判断值是否在集合内
来源：http://hz.yueranfly.top/gtyfnixewc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xingfuxueyuan.xyz/gtgerhpktb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hywenlv.cn/gtpcliraxo.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhiwuduotai.top/gtqwcbqrmf.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.nwbrower.top/gtgnrusfqw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgfzy.top/gtervcylez.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jiagoushi.top/gtyfcnduir.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xingfuxueyuan.xyz/gtljbwyqbl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tanke756.top/gtajtsmqit.html

[B15] 布尔运算与取反
来源：http://hz.gotoacloud.top/gtcsbziysd.html

Py:   a and b or not c
来源：http://hz.shzxlz.cn/gttzuarvkz.html

PHP:  $a && $b || !$c
来源：http://hz.shuidangran.top/gtzzgowykp.html

JS:   a && b || !c
来源：http://hz.vqdsnc.cn/gtczepxyyg.html

TS:   a && b || !c
来源：http://hz.fengsongda.top/gtyasrmfrb.html

Java: a && b || !c
来源：http://hz.jianghu66.top/gtqdjqsyic.html

Go:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtvlojwbwn.html

Ruby: a && b || !c
来源：http://hz.kuanghao11.cn/gtypdfmjzw.html

C#:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtmqsaromr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.0kj1m.cn/gtydsnkxhu.html

Py:   if not data: return
来源：http://hz.gotoacloud.top/gtcqjkirml.html

PHP:  if (!$data) { return; }
来源：http://hz.jyoumei.cn/gtkathstfl.html

JS:   if (!data) return;
来源：http://hz.jinqigufen.top/gtyojxhxgl.html

TS:   if (!data) return;
来源：http://hz.nanxuanxn.top/gtugbjlfbb.html

Java: if (data == null) return;
来源：http://hz.jinghuilouyu.cn/gtokqnzqvu.html

Go:   if data == nil { return }
来源：http://hz.yongpay.top/gtzbgmlaiv.html

Ruby: return if data.nil?
来源：http://hz.shzxlz.cn/gtxadelxpk.html

C#:   if (data == null) return;
来源：http://hz.guowangkeji.top/gtmyoakjrn.html

================================================================================
来源：http://hz.gogol.net.cn/gtnxshuljr.html

C. 函数与作用域
来源：http://hz.jlsjyb.cn/gtyyhfqtgf.html

================================================================================
来源：http://hz.yangfankeji.com/gttcawvwsq.html

[C01] 定义函数
来源：http://hz.iojbl.cn/gtvccnntxx.html

Py:   def add(a, b): return a + b
来源：http://hz.zhoulong.xyz/gtmhdptwma.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daxiang520.top/gtwrskdulh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.0kj1m.cn/gtsoajrdhw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jianghu66.top/gtqjtksetw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jianghu66.top/gtuvmiirsl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxinkj.top/gtzalxmdsf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sweek.top/gtirvjtqes.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtumuuvsvg.html

[C02] 默认参数
来源：http://hz.sweek.top/gteljnagdv.html

Py:   def greet(name="World"): return name
来源：http://hz.yj202588.top/gtfiljmfqq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nwbrower.top/gtogjrodrp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.havefunace.top/gtmbsadmqj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yueranfly.top/gtbsgabvft.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.birdmap.top/gtqmljyvvb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yanxiufei.cn/gtowxglbuz.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinghuilouyu.cn/gtosgcytnp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ywan-chungtsiang.top/gthotxsykg.html

[C03] 可变参数
来源：http://hz.ydzc1.top/gtnivkffpf.html

Py:   def total(*args): return sum(args)
来源：http://hz.dashuyun.cn/gtuourlnym.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.fengsongda.top/gtioapabay.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydjk.org.cn/gtevicyolh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj202588.top/gtercjezwa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.smart0.xyz/gtgcogxyld.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.9152youxi.cn/gtrcsgvfpe.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sxryk.cn/gtxnzcigfy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.mhx1999.top/gttkuzbzgj.html

[C04] 命名参数 / 关键字参数
来源：http://hz.316326.xyz/gtpxonirud.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shanyushiyangtech.top/gtyhgnghxe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tanke756.top/gtfaasxqms.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jyoumei.cn/gtrsjlyply.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jlsjyb.cn/gtwqsbkspk.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.dashuyun.cn/gtffvofxpt.html

Go:   // 无：用配置结构体参数
来源：http://hz.ywan-chungtsiang.top/gtyurwwggd.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cashguo.top/gtvhlzpypx.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuanzx.com/gtlbxoaghv.html

[C05] 返回多个值
来源：http://hz.aibaodan.cn/gtlphmnmlv.html

Py:   return a, b
来源：http://hz.hywenlv.cn/gtsjtiafhj.html

PHP:  return [$a, $b];
来源：http://hz.hysaishi.cn/gtoowbtokr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zycfv.cn/gtzsrkepnt.html

TS:   return { a, b };
来源：http://hz.jinyuanbaomall.cn/gtlsojrwtx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.havefunace.top/gtcniknspv.html

Go:   return a, b
来源：http://hz.chenjidiqi.icu/gtfbotztiz.html

Ruby: return a, b
来源：http://hz.aizwys.cn/gtottuijoz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gotoacloud.top/gtyqqvtczr.html

[C06] 匿名函数 / lambda
来源：http://hz.xingfuxueyuan.xyz/gtilrnhtyj.html

Py:   square = lambda x: x * x
来源：http://hz.jiagoushi.top/gtxotzvbka.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hnqzz.top/gteukudnxi.html

JS:   const square = x => x * x;
来源：http://hz.cdnleiting.top/gtfgqcvrjh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hfpthk.cn/gtchgyashk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ydzc1.top/gtlvsioazk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gaohongyu789.top/gtzkzubyij.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hnqzz.top/gtjdohblvq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.wangdashe.top/gtjdyfqxja.html

[C07] 把函数作为参数传入
来源：http://hz.shuidangran.top/gtnygzlfng.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.svipenyu.cn/gtcyruwljj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dashuyun.cn/gtntrklojm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ivvv.top/gtgjenztvt.html

TS:   arr.map(String)
来源：http://hz.yonumen.top/gtwacswmov.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.quarkkingdee.top/gtvojxamud.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ppjwa.cn/gthnwoxkem.html

Ruby: arr.map(&:upcase)
来源：http://hz.52xcode.cn/gtsidrdjgx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.cdnleiting.top/gtufszzkid.html

[C08] 闭包
来源：http://hz.havefunace.top/gtoaywpncm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hammf.cn/gtdhehimpa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gogol.net.cn/gtasaujtwn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtlhjmblfk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gthxnscnck.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yanxiufei.cn/gtillpytgw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.wangshuangyany.cn/gtaloagigs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shangyingyoupin.top/gtkptzabho.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gtrbfvmtmr.html

[C09] 递归
来源：http://hz.jqgufenzy.top/gtgmwjimou.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gtxpmvzmzj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.dianchejie.cn/gtllxlzpjz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jiagoushi.top/gtbgskjvfo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ivvv.top/gtuafidsmy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gzhubu.top/gtadbysqob.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cheryme.top/gtaheurapq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hywenlv.cn/gtyfmtzqwz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yonumen.top/gtpxxorvdu.html

[C10] 变量作用域
来源：http://hz.chenzaomai.com/gtlkcypegp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yuxming.cn/gtxphcedak.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sysykeji.top/gtddytkmrc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xuanzx.com/gtxekiyiph.html

TS:   同 JS
来源：http://hz.shzxlz.cn/gtjantazgz.html

Java: 方法内为块级作用域
来源：http://hz.jinyuanbaomall.cn/gteetzmnir.html

Go:   花括号块级作用域
来源：http://hz.chenjidiqi.icu/gtikqszutz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.pengpengdd.cyou/gtvigxwhxd.html

C#:   块级作用域
来源：http://hz.shangyingyoupin.top/gtkfjiutir.html

[C11] 模块导入与导出
来源：http://hz.hywenlv.cn/gtzqwyvsgq.html

Py:   from module import func
来源：http://hz.aizwys.cn/gtngczbarn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shuidangran.top/gtkhzzdvwg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.pycfn.com/gtfpjrscxt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ywan-chungtsiang.top/gtmxjljald.html

Java: import java.util.List;
来源：http://hz.yvedp.cn/gtudfoloaw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hongshengwenyu.top/gtcfcabtal.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.andypj.xyz/gtdrpntsrc.html

C#:   using System.Text;
来源：http://hz.chenlongwang.top/gtwqnfhhle.html

[C12] 立即执行函数 IIFE
来源：http://hz.redwolf501.top/gthjibgjxe.html

Py:   (lambda: print("run"))()
来源：http://hz.c1oappe.top/gtdqykamga.html

PHP:  (function () { echo "run"; })();
来源：http://hz.mhx1999.top/gtvqrgbtie.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cqqwz.cn/gtgwoyhugj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhiwuduotai.top/gtfqdqztyq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj202588.top/gtxuekhpdo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sweek.top/gtjffjtqka.html

Ruby: -> { puts "run" }.call
来源：http://hz.smart0.xyz/gtjmhurdqi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sxryk.cn/gthilherhb.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuetiantiany.cn/gtpryzazfr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ydzc1.top/gtzkgbqcbz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gttnshrfhp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuxming.cn/gtvtxugcvg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuxming.cn/gtpqaikdhl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gtxihqkfhk.html

Go:   func add(a, b int) int
来源：http://hz.aibaodan.cn/gtvpgkfmep.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hongshengwenyu.top/gtdxeuazgn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cheryme.top/gtwmxadipi.html

[C14] 泛型函数
来源：http://hz.cqqwz.cn/gtahcuaguc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.52xcode.cn/gtendehelb.html

PHP:  // 无泛型
来源：http://hz.yonumen.top/gtbmbqmvde.html

JS:   // 无泛型
来源：http://hz.yuanzhike.top/gtygxlkdrw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.52xcode.cn/gthzshariz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cdnleiting.top/gtfsaeqaaj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hywenlv.cn/gtezvwvyiz.html

Ruby: # 无泛型
来源：http://hz.zhongyouzk.top/gtmzubnazc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhoulong.xyz/gttesdlpqu.html

[C15] 解构 / 展开参数
来源：http://hz.zycfv.cn/gtqwzrkjla.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.c1oappe.top/gtibftmgsr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aibaodan.cn/gtnsuuqqew.html


<!-- 参考信息 -->