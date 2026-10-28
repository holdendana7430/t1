代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.daxiang520.top/gtelkdaoio.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.ppjwa.cn/gtbkdkwnxn.html

[A24] 去除首尾空白
来源：http://hz.kuanghao11.cn/gtbjswpnoa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.cucudq.cn/gtyovfqvqk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.sysykeji.top/gtywfmrzdh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.chenlongwang.top/gthpncydhc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhengqikj.top/gtyhnvibya.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.daxiang520.top/gtjiqcybsx.html

Go:   strings.TrimSpace(s)
来源：http://hz.iojbl.cn/gtikqgojic.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yonumen.top/gtkuopdfmk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.hnxiangtu.top/gtcskpwxiu.html

[A25] 字符串比较
来源：http://hz.jinqigufen.top/gtcyjrzadu.html

Py:   s1 == s2; s1 != s2
来源：http://hz.316326.xyz/gtfxnnycty.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.daria6918.cn/gthslykkjr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.havefunace.top/gtgwvrakmz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.chenzaomai.com/gtehetmpdf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.dashuyun.cn/gtechlbtls.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.sweek.top/gtfltcctvo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.chenlongwang.top/gtmpmlqdmf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.wangdashe.top/gtxtaowugw.html

[A26] 类型转换总览
来源：http://hz.jyoumei.cn/gtytwngjif.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.xziqi.cn/gtigswvlgz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.andypj.xyz/gtmccpcwxc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.bjfxy.top/gtmisgxjop.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yj20258.top/gtcbjvpmrl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhiwuduotai.top/gtyqkukdvu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhiwuduotai.top/gtxyapbpor.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jqgfzy.top/gtshxsxdyv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.tian-w.cn/gtyecxxxfz.html

================================================================================
来源：http://hz.hnqzz.top/gtumnspwps.html

B. 流程控制
来源：http://hz.cucudq.cn/gtjvcvqkvg.html

================================================================================
来源：http://hz.jinqigfzy.top/gthascjpqr.html

[B01] 条件判断 if / else
来源：http://hz.fzhhl.top/gtsvdhsuvl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cdnleiting.top/gtttbqsdxg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.gaohongyu789.top/gtggnesvqh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.nanxuanxn.top/gtkdkjhapg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hnqzz.top/gtbsgqayfh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yvedp.cn/gtgagursng.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yangfankeji.com/gtpayntrnd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.0kj1m.cn/gtdkabeodi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.sweek.top/gtsrmiomqh.html

[B02] 多分支 else if / elif
来源：http://hz.hnqzz.top/gtzsfvjtbj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.cucudq.cn/gtpuzjswjd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jyoumei.cn/gtpxkttxee.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhoulong.xyz/gtsrinwiai.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yongpay.top/gtcbqytvzg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cdnleiting.top/gtwlxigcie.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.c1oappe.top/gtvwuswess.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.redwolf501.top/gtwtcisqwm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hnxiangtu.top/gtcxxnzzgu.html

[B03] switch / match / case
来源：http://hz.xingfuxueyuan.xyz/gtrghxdcyr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.smart0.xyz/gtnyhtmdih.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.wangshuangyany.cn/gthhdawqkr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhaomingkeji.xyz/gtjnqqppcv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhaomingkeji.xyz/gtrvlfwhra.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.hysaishi.cn/gtvpvejkvg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.pycfn.com/gtlsqbzjwf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.aizwys.cn/gtcekyygjb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yuxming.cn/gtqsztwhng.html

[B04] for 计数循环
来源：http://hz.fzhhl.top/gtrxcxghip.html

Py:   for i in range(10): print(i)
来源：http://hz.jyoumei.cn/gttxyqcbie.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.snrcjt.cn/gtecfgylxn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gogol.net.cn/gtimipnxpv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shzxlz.cn/gtbioaoacr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xingfuxueyuan.xyz/gtbspeghkp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhixingplan.top/gtauztminr.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shuidangran.top/gtoctciwni.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.tian-w.cn/gtalbujkfx.html

[B05] 遍历数组 / 列表
来源：http://hz.52xcode.cn/gtphojnoly.html

Py:   for item in arr: print(item)
来源：http://hz.aibaodan.cn/gtmsyrkpbd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.cheryme.top/gtffnoidvn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhijiandao.cn/gtvffntftt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jqgfzy.top/gtdwijcmye.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jyoumei.cn/gtiepzoxgd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.guannengcc.top/gtpkjibmef.html

Ruby: arr.each { |item| puts item }
来源：http://hz.bjfxy.top/gtcvrkgrwd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhaomingkeji.xyz/gtdkonfgxu.html

[B06] 遍历字典 / 对象
来源：http://hz.pycfn.com/gtaggbvdvn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhaomingkeji.xyz/gtbgkzvath.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hnxiangtu.top/gtdidldspb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj20258888.top/gtnhsgvanh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ivvv.top/gtghfndgpa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.iojbl.cn/gtmzaanrht.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ywan-chungtsiang.top/gtauilemky.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jinghuilouyu.cn/gtuwjjkjml.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.nanxuanxn.top/gtnhjfwsva.html

[B07] while 循环
来源：http://hz.shzxlz.cn/gtncslymbo.html

Py:   while i < 10: i += 1
来源：http://hz.jyoumei.cn/gtafewrchj.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.havefunace.top/gtocrgwpts.html

JS:   while (i < 10) { i++; }
来源：http://hz.ivvv.top/gtdobxtbbi.html

TS:   while (i < 10) { i++; }
来源：http://hz.nanxuanxn.top/gtimxijcsm.html

Java: while (i < 10) { i++; }
来源：http://hz.ywan-chungtsiang.top/gtjtjhxzot.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hnxiangtu.top/gtqszqeptq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jiagoushi.top/gtjolksstj.html

C#:   while (i < 10) { i++; }
来源：http://hz.ivvv.top/gtjiocqait.html

[B08] do-while（至少执行一次）
来源：http://hz.ydzc1.top/gtlssgxfwk.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yj20258.top/gtfjzudzcc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.cucudq.cn/gtknbclovp.html

JS:   do { i++; } while (i < 10);
来源：http://hz.nanxuanxn.top/gtxjkkdzva.html

TS:   do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtcftnyray.html

Java: do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtrmppmzax.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yuanzhike.top/gtnulocpnq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ivvv.top/gtrvkernip.html

C#:   do { i++; } while (i < 10);
来源：http://hz.chenzaomai.com/gtotyehdhm.html

[B09] break 与 continue
来源：http://hz.ppjwa.cn/gtmgwldmzd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.haohaochexian.top/gtfibblysg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ehwqpu.com/gtrwkixjbu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gotoacloud.top/gtodvovquv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtflxjxusl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gtbhinusrj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yvedp.cn/gtovrerxgc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ppjwa.cn/gtdauucxce.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yueranfly.top/gtaujzpfgw.html

[B10] 遍历同时拿索引
来源：http://hz.pengpengdd.cyou/gtsflevwzu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yangfankeji.com/gtymentatc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jyoumei.cn/gtytlktebq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hysaishi.cn/gtsarbpdok.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shuidangran.top/gtjmhpikea.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.mhx1999.top/gtvedzrlfb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.quarkkingdee.top/gtfdftlrej.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhongyouzk.top/gtjtobjtuh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhiwuduotai.top/gtxgytnumj.html

[B11] 生成数字序列 / 区间
来源：http://hz.zdqjudy.top/gtmvrgnuzc.html

Py:   list(range(0, 10, 2))
来源：http://hz.jianghu66.top/gtpimwxtmn.html

PHP:  range(0, 10, 2);
来源：http://hz.yj20258.top/gtddeaauuv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hammf.cn/gthbwzxokd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.daria6918.cn/gtuagmokvv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hnxiangtu.top/gtcsvqdkdu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.mhx1999.top/gtdxemhpsd.html

Ruby: (0...10).step(2).to_a
来源：http://hz.c1oappe.top/gtwncaxcvy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xinyue.icu/gtbfipxqsi.html

[B12] 跳出多层循环
来源：http://hz.hongshengwenyu.top/gthrzrojtw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xylfe.cn/gtxlmpwlrp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.daria6918.cn/gtpuwaubqs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gtgsspicqe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yonumen.top/gtpkrvugbr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhengqikj.top/gtgdggqtwm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ybcxt.top/gtcwpruqbp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jqgfzy.top/gtsivtftos.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jqgfzy.top/gtnivkzkzr.html

[B13] 判断是否为数字
来源：http://hz.wangshuangyany.cn/gtggyohouk.html

Py:   isinstance(x, (int, float))
来源：http://hz.hnqzz.top/gtbeiuwgks.html

PHP:  is_numeric($x)
来源：http://hz.jlsjyb.cn/gtifvztmub.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hysaishi.cn/gtpcpoydgg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258.top/gtlaeclljc.html

Java: x instanceof Number
来源：http://hz.jinqigfzy.top/gtwqywdzmn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinghuilouyu.cn/gtqsprrhbw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.bjfxy.top/gtfzvcqnng.html

C#:   x is int or double or decimal
来源：http://hz.svipenyu.cn/gtzavxjcip.html

[B14] 判断值是否在集合内
来源：http://hz.zhiwuduotai.top/gtcqpujllx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hnxiangtu.top/gtsczmllid.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jinqigufen.top/gtahlrqyrb.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dashuyun.cn/gtabzttqnt.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cashguo.top/gthcoybrml.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.chenzaomai.com/gtibpkhntz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.c1oappe.top/gtojtnrjih.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj20258888.top/gtygxtcdud.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.quarkkingdee.top/gtkavydzgd.html

[B15] 布尔运算与取反
来源：http://hz.ydjk.org.cn/gtweuonmpq.html

Py:   a and b or not c
来源：http://hz.zhongyouzk.top/gtmufhojtf.html

PHP:  $a && $b || !$c
来源：http://hz.birdmap.top/gtmgkhytxz.html

JS:   a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtixxhvbyz.html

TS:   a && b || !c
来源：http://hz.tanke756.top/gtqbuanshq.html

Java: a && b || !c
来源：http://hz.quarkkingdee.top/gtzpbgbqyx.html

Go:   a && b || !c
来源：http://hz.wangshuangyany.cn/gtksasvjew.html

Ruby: a && b || !c
来源：http://hz.cucudq.cn/gtixynsxie.html

C#:   a && b || !c
来源：http://hz.havefunace.top/gtsylrrewx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.gotoacloud.top/gtdypijnhy.html

Py:   if not data: return
来源：http://hz.xuanzx.com/gtxskumwfm.html

PHP:  if (!$data) { return; }
来源：http://hz.mhx1999.top/gtuosjneyz.html

JS:   if (!data) return;
来源：http://hz.yj202588.top/gtbezpvmtj.html

TS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtjwswvypk.html

Java: if (data == null) return;
来源：http://hz.hnxiangtu.top/gtmxnzskbm.html

Go:   if data == nil { return }
来源：http://hz.hnqzz.top/gtakudbfth.html

Ruby: return if data.nil?
来源：http://hz.hysaishi.cn/gtfzeagbxr.html

C#:   if (data == null) return;
来源：http://hz.zhiwuduotai.top/gtvdjppqpl.html

================================================================================
来源：http://hz.chenlongwang.top/gtomdkuwtn.html

C. 函数与作用域
来源：http://hz.gaohongyu789.top/gtrmmlrccx.html

================================================================================
来源：http://hz.havefunace.top/gtuacxmjug.html

[C01] 定义函数
来源：http://hz.ppjwa.cn/gtjivcccox.html

Py:   def add(a, b): return a + b
来源：http://hz.aizwys.cn/gtbtbzclbo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtbndqfvss.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shuidangran.top/gtmldxurni.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigfzy.top/gtqleolftm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtsdgiggml.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.havefunace.top/gtvwpwpdms.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenzaomai.com/gtpzzcvezy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtnposbtit.html

[C02] 默认参数
来源：http://hz.xuanzx.com/gtelmynlqm.html

Py:   def greet(name="World"): return name
来源：http://hz.yongpay.top/gtncmhzyzy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.smart0.xyz/gtejdztbdx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxinkj.top/gtrmgecouj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.nanxinkj.top/gtsgkdhcvi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.bjfxy.top/gtrvwgwwss.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xuetiantiany.cn/gtazkeusue.html

Ruby: def greet(name = "World") = name
来源：http://hz.redwolf501.top/gtwcwjscae.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.bjfxy.top/gtuucafmsh.html

[C03] 可变参数
来源：http://hz.shanyushiyangkeji.top/gtiykmldxy.html

Py:   def total(*args): return sum(args)
来源：http://hz.andypj.xyz/gtdmvhexpe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ybcxt.top/gtblanrbzl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgufenzy.top/gtnnvlwfhz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daria6918.cn/gtzljulddd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cashguo.top/gtucihtify.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ywan-chungtsiang.top/gtmodadjfi.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.bjfxy.top/gtgnmdsdid.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.wangshuangyany.cn/gtjtquvymx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.0kj1m.cn/gtofnykcfg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sysykeji.top/gtrrmxsavy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.daxiang520.top/gtgagecdur.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yanxiufei.cn/gttmwifhgx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.feifeiyinyue.top/gtnhszlcin.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.9152youxi.cn/gtouibjrlm.html

Go:   // 无：用配置结构体参数
来源：http://hz.xuanzx.com/gtaatakyjs.html

Ruby: f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gtbumzsrvy.html

C#:   f(a: 1, b: 2)
来源：http://hz.cdnleiting.top/gtxzmkzsdw.html

[C05] 返回多个值
来源：http://hz.yuanzhike.top/gttmrutspf.html

Py:   return a, b
来源：http://hz.iojbl.cn/gtfnqderzb.html

PHP:  return [$a, $b];
来源：http://hz.birdmap.top/gtmblpmnam.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.chenjidiqi.icu/gtgfrrxglw.html

TS:   return { a, b };
来源：http://hz.aizwys.cn/gthusxdong.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ehwqpu.com/gtyptjpybf.html

Go:   return a, b
来源：http://hz.zhixingplan.top/gtcdbochyw.html

Ruby: return a, b
来源：http://hz.yj20258888.top/gtujmidjzp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.feifeiyinyue.top/gtkqenywxz.html

[C06] 匿名函数 / lambda
来源：http://hz.nanxinkj.top/gtrcncfqhe.html

Py:   square = lambda x: x * x
来源：http://hz.zhengqikj.top/gtaqzckbqy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhongyouzk.top/gtbjypzyyf.html

JS:   const square = x => x * x;
来源：http://hz.chenzaomai.com/gtikhdwzhl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.fzhhl.top/gtjdoogqrl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hongshengwenyu.top/gtfdofbksx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.wangshuangyany.cn/gtdtgvygnv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xuanzx.com/gtakuntuwo.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.pengpengdd.cyou/gtmqrjhzuq.html

[C07] 把函数作为参数传入
来源：http://hz.ydzc1.top/gtqykzhadw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.redwolf501.top/gtozisvkuo.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nanxuanxn.top/gtxydgnebh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.andypj.xyz/gtqfaxgjnw.html

TS:   arr.map(String)
来源：http://hz.zhixingplan.top/gtqkdigrho.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenlongwang.top/gtiukqhjni.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangtech.top/gtylnujzir.html

Ruby: arr.map(&:upcase)
来源：http://hz.gotoacloud.top/gtarbocwud.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhijiandao.cn/gtzdcscxlg.html

[C08] 闭包
来源：http://hz.yvedp.cn/gtgbottbpo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shangyingyoupin.top/gtekithtpc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.quarkkingdee.top/gtwjzuljea.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gttqnmdlra.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yj202588.top/gtwusqwvqo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.bjfxy.top/gthdkjxbqw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.wangdashe.top/gtfmrblkzz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cqqwz.cn/gtqsqkwjos.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gtpoqwqqnv.html

[C09] 递归
来源：http://hz.c1oappe.top/gtseaordpo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jiagoushi.top/gtvyrhhbpv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yj20258.top/gtiejioszy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gtgkzuaxqu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.birdmap.top/gtkbgpgplf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.dianchejie.cn/gtskdpfltr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.nanxinkj.top/gtrynncuuf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtqepwhziz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hnqzz.top/gtuycxugzl.html

[C10] 变量作用域
来源：http://hz.yj20258.top/gtjnpfncvf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhongyouzk.top/gtmekkexmv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.aizwys.cn/gtjwsxryth.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.tian-w.cn/gtrvbipffi.html

TS:   同 JS
来源：http://hz.xuetiantiany.cn/gtwzmurjtt.html

Java: 方法内为块级作用域
来源：http://hz.hysaishi.cn/gtyehzhyzz.html

Go:   花括号块级作用域
来源：http://hz.guowangkeji.top/gtjxorjold.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.mhx1999.top/gtegwmkpbz.html

C#:   块级作用域
来源：http://hz.cheryme.top/gtepaokkfv.html

[C11] 模块导入与导出
来源：http://hz.redwolf501.top/gtvfvavizr.html

Py:   from module import func
来源：http://hz.yanxiufei.cn/gtmjtgfqai.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.pycfn.com/gtvjkmtikm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhengqikj.top/gtlndsovrs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ivvv.top/gtfijclbia.html

Java: import java.util.List;
来源：http://hz.zhixingplan.top/gtkibjzusd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydjk.org.cn/gtvjqhiaex.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhongyouzk.top/gtznyewsfn.html

C#:   using System.Text;
来源：http://hz.xuanzx.com/gtfxfkdvkn.html

[C12] 立即执行函数 IIFE
来源：http://hz.daxiang520.top/gtfmahorsu.html

Py:   (lambda: print("run"))()
来源：http://hz.aizwys.cn/gttadpeewy.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yuanzhike.top/gthswxrfls.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhixingplan.top/gtalmtlepw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangtech.top/gtxoglezis.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hongshengwenyu.top/gtpkzkwqmt.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.aizwys.cn/gtzotvcifx.html

Ruby: -> { puts "run" }.call
来源：http://hz.shzxlz.cn/gtcurkvizo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shanyushiyangkeji.top/gtcujrwdgg.html

[C13] 类型声明 / 类型注解
来源：http://hz.guannengcc.top/gtdajspqek.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhaomingkeji.xyz/gtxjmqnniu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gthdipmpdd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.dianchejie.cn/gtiruvdjmb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pengpengdd.cyou/gttblgisrj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gtrnssgcdb.html

Go:   func add(a, b int) int
来源：http://hz.chenlongwang.top/gtcmvvlhpk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydzc1.top/gtpupcdsqt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.iojbl.cn/gtnnokudda.html

[C14] 泛型函数
来源：http://hz.ybcxt.top/gtpjffbjof.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhijiandao.cn/gtkiswdthm.html

PHP:  // 无泛型
来源：http://hz.hnqzz.top/gtzvhtmquh.html

JS:   // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtyyvwzzdo.html


<!-- 参考信息 -->