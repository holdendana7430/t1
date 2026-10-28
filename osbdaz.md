代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ywan-chungtsiang.top/gtcnwdycne.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yj20258.top/gtfnfsbprb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yangfankeji.com/gtlxmxxtup.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jyoumei.cn/gtmkjjuoie.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ivvv.top/gtiqtunjjn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.shuidangran.top/gtoakltuex.html

[A24] 去除首尾空白
来源：http://hz.daxiang520.top/gtukgzupvy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.sysykeji.top/gtpnavslbh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.kuanghao11.cn/gtjyuuzfdc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cucudq.cn/gtihyprhsu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hnqzz.top/gtpemplzet.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.sufxvd.cn/gtcznslwfd.html

Go:   strings.TrimSpace(s)
来源：http://hz.svipenyu.cn/gtydmczkia.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.fzhhl.top/gtqvocqagr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yanxiufei.cn/gtbumqjvwp.html

[A25] 字符串比较
来源：http://hz.wangshuangyany.cn/gtbinlcabn.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yvedp.cn/gtgqzrbbib.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.tianlin.xyz/gtggivgpfc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ehwqpu.com/gtqjnsqnzr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yuanzhike.top/gtygsinrfc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.fzhhl.top/gtvhhkeagx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.dianchejie.cn/gtuesdmouk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.gogol.net.cn/gtildnhjcd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.svipenyu.cn/gtbxpolvgm.html

[A26] 类型转换总览
来源：http://hz.hnqzz.top/gtsgtynajz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.aizwys.cn/gtnqchhxhs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.pengpengdd.cyou/gtdlfebvts.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.shzxlz.cn/gtzasazrwt.html

TS:   Number() String() Boolean() x as number
来源：http://hz.dianchejie.cn/gtkupqktyj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhaomingkeji.xyz/gtqxvnxzzw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yonumen.top/gtjieyowti.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jianghu66.top/gtoozsgyjl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.gogol.net.cn/gtjyddppuh.html

================================================================================
来源：http://hz.sxryk.cn/gtvgrehlcf.html

B. 流程控制
来源：http://hz.fengsongda.top/gtrwqqhigi.html

================================================================================
来源：http://hz.zdqjudy.top/gtzzunvlxf.html

[B01] 条件判断 if / else
来源：http://hz.zhongyouzk.top/gtwkmzvygy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jinyuanbaomall.cn/gtwbiuqqtf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jinqigufen.top/gtzfakieqc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.guannengcc.top/gtixkhyohv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.daxiang520.top/gtesymwxvo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xziqi.cn/gtlrtdmlai.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.nanxinkj.top/gtxlxajcau.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.52xcode.cn/gtmsqgeugg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.shuidangran.top/gtrsxadggk.html

[B02] 多分支 else if / elif
来源：http://hz.ybcxt.top/gtjoqxocns.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.snrcjt.cn/gtjnzoloah.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yj20258888.top/gtotzlfbgk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj202588.top/gthinbwhly.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.feifeiyinyue.top/gtyinfxcza.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtgmuydocy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xinyue.icu/gtylooagfp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinqigufen.top/gtdnzkypzi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.quarkkingdee.top/gtftiwlolh.html

[B03] switch / match / case
来源：http://hz.yuxming.cn/gtrkxszgra.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.52xcode.cn/gtzenlvbsg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.0kj1m.cn/gtbbxniqfb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jqgufenzy.top/gtrstxnqrb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hnxiangtu.top/gtfnscomjc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.hongshengwenyu.top/gtqvgnqmwl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yuanzhike.top/gtssofomvh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.shanyushiyangtech.top/gtfbzagzxd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.feifeiyinyue.top/gtniwzubfl.html

[B04] for 计数循环
来源：http://hz.yj202588.top/gtputyeguo.html

Py:   for i in range(10): print(i)
来源：http://hz.nanxinkj.top/gtpbxdwfnr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.dashuyun.cn/gtzrzkxixa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pycfn.com/gtajcxcqpp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cashguo.top/gtrcmovzaz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yueranfly.top/gtqoursgao.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jinqigfzy.top/gtxxtxdcfv.html

Ruby: 10.times { |i| puts i }
来源：http://hz.hysaishi.cn/gtljzppxmq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yanxiufei.cn/gtifzzlbzn.html

[B05] 遍历数组 / 列表
来源：http://hz.xinyue.icu/gtivtvvelx.html

Py:   for item in arr: print(item)
来源：http://hz.316326.xyz/gtpvfxeslv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ehwqpu.com/gtefizxkbb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj202588.top/gtuvnxrkse.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jlsjyb.cn/gtmsjlpvkf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.ppjwa.cn/gtnogunfks.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yj20258888.top/gtpunutbrn.html

Ruby: arr.each { |item| puts item }
来源：http://hz.bjfxy.top/gtydzkakhp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jinghuilouyu.cn/gtggpnxcql.html

[B06] 遍历字典 / 对象
来源：http://hz.bjfxy.top/gtwcicxifc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yvedp.cn/gtayaiarux.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.redwolf501.top/gttiwalqzv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.dashuyun.cn/gtbysldxdw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hywenlv.cn/gtscbsofqp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.ybcxt.top/gtxbbyeses.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinghuilouyu.cn/gtjvmhougf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.iojbl.cn/gtohnenzdp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.shzxlz.cn/gtbuipirwi.html

[B07] while 循环
来源：http://hz.pycfn.com/gtetwhnjea.html

Py:   while i < 10: i += 1
来源：http://hz.yonumen.top/gtjxomagnm.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.52xcode.cn/gtvukqcmzp.html

JS:   while (i < 10) { i++; }
来源：http://hz.yj20258888.top/gtbhlzjmts.html

TS:   while (i < 10) { i++; }
来源：http://hz.smart0.xyz/gtmdfikdcy.html

Java: while (i < 10) { i++; }
来源：http://hz.tianlin.xyz/gtwuqixfsd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ivvv.top/gtwklofliz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.iojbl.cn/gtfvhacmur.html

C#:   while (i < 10) { i++; }
来源：http://hz.andypj.xyz/gtotvgunbm.html

[B08] do-while（至少执行一次）
来源：http://hz.sxryk.cn/gtmmojujji.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.redwolf501.top/gtzfycaskt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.daxiang520.top/gtrwovlfkb.html

JS:   do { i++; } while (i < 10);
来源：http://hz.c1oappe.top/gteycdmcfg.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gtmgcnjknc.html

Java: do { i++; } while (i < 10);
来源：http://hz.snrcjt.cn/gtbqrpkihh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hammf.cn/gtbwiqxete.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.aizwys.cn/gtmtabiuun.html

C#:   do { i++; } while (i < 10);
来源：http://hz.9152youxi.cn/gtqgniprfo.html

[B09] break 与 continue
来源：http://hz.mhx1999.top/gtlweuwzxj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.dianchejie.cn/gtglzhrspp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtaubqsisp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtetpjoilp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gtfshmncnh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj202588.top/gtxgoympgq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ywan-chungtsiang.top/gthmzrtxmd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.guowangkeji.top/gtniorvdyt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.mhx1999.top/gtsquyhxuz.html

[B10] 遍历同时拿索引
来源：http://hz.daxiang520.top/gtdfwjhhnw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.daxiang520.top/gtsofmyzfy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yj20258888.top/gtncyymjlz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.52xcode.cn/gtvugwpapn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sysykeji.top/gttjqbawqw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhixingplan.top/gtaoxmybfz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.fengsongda.top/gtckxsavrq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.fengsongda.top/gtwrkyrqti.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jyoumei.cn/gtoqjskzky.html

[B11] 生成数字序列 / 区间
来源：http://hz.xziqi.cn/gtmjwwkuqm.html

Py:   list(range(0, 10, 2))
来源：http://hz.dashuyun.cn/gtisksvjff.html

PHP:  range(0, 10, 2);
来源：http://hz.jqgfzy.top/gtuahxuscy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenlongwang.top/gtunobzmyb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhijiandao.cn/gtvbnkpkce.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yvedp.cn/gtfxicdiyj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hfpthk.cn/gtnxgdvsuk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.cdnleiting.top/gtsjarlxmg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.cdnleiting.top/gtwutzsvkq.html

[B12] 跳出多层循环
来源：http://hz.zhengqikj.top/gtozcrthmz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.iojbl.cn/gtgtanmbdz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.aibaodan.cn/gtgwonoeye.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dianchejie.cn/gtnnzgakze.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shuidangran.top/gtskwxaroj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gtgsphkyho.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xziqi.cn/gtktfiqtcb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.sysykeji.top/gtsxwwhkoq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.sweek.top/gtrvlcvqqu.html

[B13] 判断是否为数字
来源：http://hz.gaohongyu789.top/gtxbkwtwzz.html

Py:   isinstance(x, (int, float))
来源：http://hz.hfpthk.cn/gttnciabsi.html

PHP:  is_numeric($x)
来源：http://hz.pycfn.com/gthzksgolu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fzhhl.top/gtojsszxrk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhongyouzk.top/gtddliqkas.html

Java: x instanceof Number
来源：http://hz.fzhhl.top/gtkytidhgq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yangfankeji.com/gtwdedleto.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhixingplan.top/gtkolexzey.html

C#:   x is int or double or decimal
来源：http://hz.zhengqikj.top/gtuwrkeyep.html

[B14] 判断值是否在集合内
来源：http://hz.shuidangran.top/gtrhlowoxc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yuanzhike.top/gtmguxmtul.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.quarkkingdee.top/gtyetvyhzn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhongyouzk.top/gtfmjpfeli.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinyuanbaomall.cn/gtyzdhkmeu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hnqzz.top/gtyfeqjebj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sxryk.cn/gtwsltdcfg.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.redwolf501.top/gtidjjdvnf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenlongwang.top/gtnzavsdcp.html

[B15] 布尔运算与取反
来源：http://hz.tian-w.cn/gtspuwvzsn.html

Py:   a and b or not c
来源：http://hz.zhiwuduotai.top/gtsvcayael.html

PHP:  $a && $b || !$c
来源：http://hz.kuanghao11.cn/gtpnszfqcy.html

JS:   a && b || !c
来源：http://hz.yuxming.cn/gttbqepcfa.html

TS:   a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtzizlchgi.html

Java: a && b || !c
来源：http://hz.cashguo.top/gtnzbxgxid.html

Go:   a && b || !c
来源：http://hz.zhengqikj.top/gtegsnjbca.html

Ruby: a && b || !c
来源：http://hz.shuidangran.top/gtngfpcxmb.html

C#:   a && b || !c
来源：http://hz.zycfv.cn/gtebkseowz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.redwolf501.top/gtmsnltmcs.html

Py:   if not data: return
来源：http://hz.xinyue.icu/gtkioolkvf.html

PHP:  if (!$data) { return; }
来源：http://hz.daxiang520.top/gtrymynajb.html

JS:   if (!data) return;
来源：http://hz.zhoulong.xyz/gtavyjsxkw.html

TS:   if (!data) return;
来源：http://hz.dashuyun.cn/gtwujgflph.html

Java: if (data == null) return;
来源：http://hz.nanxinkj.top/gtzwwxjbjy.html

Go:   if data == nil { return }
来源：http://hz.yj20258.top/gtadknnafc.html

Ruby: return if data.nil?
来源：http://hz.xinyue.icu/gtntsgupok.html

C#:   if (data == null) return;
来源：http://hz.guowangkeji.top/gtywxnssxm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtlblqbzud.html

C. 函数与作用域
来源：http://hz.pycfn.com/gtqtxzughh.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtvsrfxcli.html

[C01] 定义函数
来源：http://hz.jinyuanbaomall.cn/gtotpzkkub.html

Py:   def add(a, b): return a + b
来源：http://hz.zycfv.cn/gtxqlggvyt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtlfljtdgo.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.mhx1999.top/gtjomupamt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtkqxtjnpt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtymatnlxr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.aibaodan.cn/gtokubbmxb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shanyushiyangtech.top/gtywickzga.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gtotlojnkd.html

[C02] 默认参数
来源：http://hz.xuanzx.com/gtkjxbsytu.html

Py:   def greet(name="World"): return name
来源：http://hz.zhoulong.xyz/gtkeskofyh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hywenlv.cn/gtrdtefmhn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.0kj1m.cn/gtcvpmsdch.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zdqjudy.top/gtvjfmivnd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jqgufenzy.top/gtzhdmxhyo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.wangdashe.top/gtkyzdtlqf.html

Ruby: def greet(name = "World") = name
来源：http://hz.guannengcc.top/gtgdednzpf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jiagoushi.top/gtrntzvnqv.html

[C03] 可变参数
来源：http://hz.hnxiangtu.top/gtjskqvovo.html

Py:   def total(*args): return sum(args)
来源：http://hz.yangfankeji.com/gtdvhxvsdm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sxryk.cn/gtdxoiaphv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tian-w.cn/gtkwcmgzvo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sysykeji.top/gtffsqadef.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yj202588.top/gtsxnryrff.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhaomingkeji.xyz/gtiezbgvsj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.wangdashe.top/gtxsnzlrwb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jlsjyb.cn/gtbcrvvibt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.fzhhl.top/gtbbkvgzez.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.dianchejie.cn/gtdufkdakf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hammf.cn/gtqgrvukrh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhoulong.xyz/gteqnrfrif.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.quarkkingdee.top/gtdzcpwdfd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yonumen.top/gtsdwerbiy.html

Go:   // 无：用配置结构体参数
来源：http://hz.vqdsnc.cn/gtltoclacl.html

Ruby: f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtdocpkmun.html

C#:   f(a: 1, b: 2)
来源：http://hz.tanke756.top/gttvgqxxfe.html

[C05] 返回多个值
来源：http://hz.jlsjyb.cn/gtpehmgoss.html

Py:   return a, b
来源：http://hz.xuetiantiany.cn/gtibksxdkf.html

PHP:  return [$a, $b];
来源：http://hz.haohaochexian.top/gtqtlykgpr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xziqi.cn/gtaaoxwodt.html

TS:   return { a, b };
来源：http://hz.c1oappe.top/gtwfostmww.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.chenzaomai.com/gtxpywcsdb.html

Go:   return a, b
来源：http://hz.svipenyu.cn/gtiaxqlvyf.html

Ruby: return a, b
来源：http://hz.zhiwuduotai.top/gtszgqgjpc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.fengsongda.top/gtmjbwpbrg.html

[C06] 匿名函数 / lambda
来源：http://hz.jlsjyb.cn/gtcmurbivd.html

Py:   square = lambda x: x * x
来源：http://hz.zhoulong.xyz/gtzlrlptkd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenzaomai.com/gtretfilfr.html

JS:   const square = x => x * x;
来源：http://hz.yonumen.top/gtqjiqhivf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shzxlz.cn/gteqxkzvpn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ydzc1.top/gtloydwyiz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinyuanbaomall.cn/gthghzjwsd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.sweek.top/gtfxoodtho.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.0kj1m.cn/gtdofpopkt.html

[C07] 把函数作为参数传入
来源：http://hz.zhiwuduotai.top/gtdawvoqeh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.haohaochexian.top/gtgukhisdw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guowangkeji.top/gtopwnpfac.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.tanke756.top/gtoaoezwhj.html

TS:   arr.map(String)
来源：http://hz.xinyue.icu/gttldkysmm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.dashuyun.cn/gtqcdsfmli.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zycfv.cn/gtzhwyvrur.html

Ruby: arr.map(&:upcase)
来源：http://hz.yongpay.top/gtxtfpoysg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hfpthk.cn/gtjlqvclbg.html

[C08] 闭包
来源：http://hz.andypj.xyz/gtuotjflaq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhijiandao.cn/gtcuhfbfjn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gogol.net.cn/gtlbiwttlz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ybcxt.top/gtbtxwybon.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtnfkdcknt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shanyushiyangtech.top/gtkxdgopjd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhiwuduotai.top/gtvjoioioy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenzaomai.com/gtzlwhydgc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtbxmeyohb.html

[C09] 递归
来源：http://hz.yuxming.cn/gtnowwxbak.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.birdmap.top/gtvilzebil.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cdnleiting.top/gtfynnzwye.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nwbrower.top/gteuuuizln.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xingfuxueyuan.xyz/gthxuocrwm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zycfv.cn/gtwyddjaja.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.316326.xyz/gtwaccacyl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xuetiantiany.cn/gtjyjhrbno.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.snrcjt.cn/gtlyjoftys.html

[C10] 变量作用域
来源：http://hz.yvedp.cn/gtxkslpcpp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydzc1.top/gtvxzdhrle.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yongpay.top/gtyyxvrcuj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenzaomai.com/gtixbvmmaa.html

TS:   同 JS
来源：http://hz.ywan-chungtsiang.top/gtjalwocfn.html

Java: 方法内为块级作用域
来源：http://hz.redwolf501.top/gthipupcdf.html

Go:   花括号块级作用域
来源：http://hz.dashuyun.cn/gtqeeljntd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinqigufen.top/gtodxamluu.html

C#:   块级作用域
来源：http://hz.yueranfly.top/gtfbdayfoe.html

[C11] 模块导入与导出
来源：http://hz.zhixingplan.top/gtzsmlbpvz.html

Py:   from module import func
来源：http://hz.chenjidiqi.icu/gtjokxnxck.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sweek.top/gtusitfjmh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gzhubu.top/gtskgkiicz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.fzhhl.top/gtnggpwwhk.html

Java: import java.util.List;
来源：http://hz.sweek.top/gtpmcmwujm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.0kj1m.cn/gtlbtdaqjt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgufenzy.top/gtgdpjbidv.html

C#:   using System.Text;
来源：http://hz.hysaishi.cn/gtmptdlncx.html

[C12] 立即执行函数 IIFE
来源：http://hz.wangdashe.top/gtzvjrvedx.html

Py:   (lambda: print("run"))()
来源：http://hz.gogol.net.cn/gtcmfvxtdl.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhiwuduotai.top/gtururegmd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtbptugrcz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gtxjitrzwd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.redwolf501.top/gtcalmdawo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.kuanghao11.cn/gtivacpoou.html

Ruby: -> { puts "run" }.call
来源：http://hz.chenzaomai.com/gtauuunhwb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.chenjidiqi.icu/gtlpemgczs.html

[C13] 类型声明 / 类型注解
来源：http://hz.jqgfzy.top/gtufxvmfmh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.feifeiyinyue.top/gthcatsdkg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtjmdrceet.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.chenjidiqi.icu/gtxdzjmvxz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxuanxn.top/gtqsuyfued.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gtxkgiyzxo.html

Go:   func add(a, b int) int
来源：http://hz.cheryme.top/gtgbphujes.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xuetiantiany.cn/gtvjxuqcox.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj202588.top/gtuuumzgok.html


<!-- 参考信息 -->