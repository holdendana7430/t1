代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zhixingplan.top/gtrcdicrji.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.redwolf501.top/gtqwyyxnol.html

[A24] 去除首尾空白
来源：http://hz.shanyushiyangkeji.top/gtxxcouwrq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jqgfzy.top/gteakxspzb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ybcxt.top/gtdikbnyry.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ywan-chungtsiang.top/gtvavvitqw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shanyushiyangtech.top/gtjhgalora.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.tian-w.cn/gtygleqjtr.html

Go:   strings.TrimSpace(s)
来源：http://hz.yueranfly.top/gtksfiaraa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.snrcjt.cn/gtzgxnvppc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.tanke756.top/gteszpmvem.html

[A25] 字符串比较
来源：http://hz.nanxinkj.top/gtqhttmlqi.html

Py:   s1 == s2; s1 != s2
来源：http://hz.fzhhl.top/gtiklokvxu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.zhijiandao.cn/gthhaealbp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jianghu66.top/gtqymbphsy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tianlin.xyz/gtxntttizn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.kuanghao11.cn/gttdddrcol.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yanxiufei.cn/gtuwybjcpf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.9152youxi.cn/gtkneccfqt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.havefunace.top/gtadzuvbuv.html

[A26] 类型转换总览
来源：http://hz.jinqigfzy.top/gtinziqvei.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jiagoushi.top/gtrdlupjuz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.tanke756.top/gtqynfxztw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.guannengcc.top/gtesetqfiq.html

TS:   Number() String() Boolean() x as number
来源：http://hz.dianchejie.cn/gteeqfnflv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.52xcode.cn/gtmhdgiglm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.dianchejie.cn/gtpwkzyrkc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.shuidangran.top/gtrzwlzvbk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.hnxiangtu.top/gtslusxckt.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtbgjgdkcm.html

B. 流程控制
来源：http://hz.yonumen.top/gtykonncrf.html

================================================================================
来源：http://hz.ydjk.org.cn/gtpxucpjkk.html

[B01] 条件判断 if / else
来源：http://hz.0kj1m.cn/gtcsidrbgp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.wangshuangyany.cn/gtvafbuzyd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jlsjyb.cn/gtmxxvglbu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.andypj.xyz/gtbanaagna.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sweek.top/gtrgnuocwa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gttaxfnxsi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhijiandao.cn/gtubofplsk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.cdnleiting.top/gtsfymnkim.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.guannengcc.top/gtplmdpapy.html

[B02] 多分支 else if / elif
来源：http://hz.jiagoushi.top/gtfnnxovry.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.shuidangran.top/gtippgiskn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.dashuyun.cn/gtjqlbiyui.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daria6918.cn/gtuwqztwzy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxuanxn.top/gtmtzvpaic.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cucudq.cn/gtpmdakgzy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.9152youxi.cn/gtflaovbwd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.sufxvd.cn/gtqtdwiqlc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gzhubu.top/gthoqnvvyg.html

[B03] switch / match / case
来源：http://hz.yonumen.top/gtjwmfnsad.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.chenlongwang.top/gtuhazdczm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.tianlin.xyz/gtondkmsnu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ydjk.org.cn/gtnfgvzzpk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yj20258888.top/gtjbgbcrxr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.zhaomingkeji.xyz/gtljanfnyl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhaomingkeji.xyz/gtxzgvuchv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhiwuduotai.top/gteczuflud.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.havefunace.top/gtgmlgglvi.html

[B04] for 计数循环
来源：http://hz.jqgfzy.top/gtsuiyifxc.html

Py:   for i in range(10): print(i)
来源：http://hz.yvedp.cn/gtmjfzgfpq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.9152youxi.cn/gtsnrlkezy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.havefunace.top/gtfcsjpzti.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.316326.xyz/gtmpdmyghf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.shzxlz.cn/gtafnswyyz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.c1oappe.top/gtojkhzuay.html

Ruby: 10.times { |i| puts i }
来源：http://hz.ydjk.org.cn/gtwhcfzltw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.vqdsnc.cn/gtymfsovcg.html

[B05] 遍历数组 / 列表
来源：http://hz.hysaishi.cn/gtyhytkqgw.html

Py:   for item in arr: print(item)
来源：http://hz.daxiang520.top/gtbwszzxlt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.kuanghao11.cn/gtrlilwsyg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yanxiufei.cn/gtbocnofhb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.pengpengdd.cyou/gtnefneuyn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.chenlongwang.top/gtpwdbgsqy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.52xcode.cn/gthlcudmrq.html

Ruby: arr.each { |item| puts item }
来源：http://hz.aibaodan.cn/gtvtzimxlk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yuanzhike.top/gtprqhxlbo.html

[B06] 遍历字典 / 对象
来源：http://hz.havefunace.top/gtpzkxhgsg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.daria6918.cn/gtzxfmylkb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.guowangkeji.top/gtkcjmgaec.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhoulong.xyz/gtciuesdfh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yanxiufei.cn/gtluazmtyb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yuxming.cn/gthslksyyd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.chenlongwang.top/gthmzamqil.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.tanke756.top/gttbtvsoox.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jinqigfzy.top/gtqdkagchh.html

[B07] while 循环
来源：http://hz.shanyushiyangtech.top/gtlsvuhuqi.html

Py:   while i < 10: i += 1
来源：http://hz.iojbl.cn/gtvktiubdq.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.9152youxi.cn/gtoevrbywq.html

JS:   while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gtcfyxuhje.html

TS:   while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gtjurrwhmq.html

Java: while (i < 10) { i++; }
来源：http://hz.havefunace.top/gtvxmpfeuy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jianghu66.top/gtcdjqupoa.html

Ruby: while i < 10; i += 1; end
来源：http://hz.sufxvd.cn/gtgrxavkcd.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gtkhindpco.html

[B08] do-while（至少执行一次）
来源：http://hz.yuanzhike.top/gtliekbirh.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.fzhhl.top/gtxzjbbggm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jinqigfzy.top/gtknnjzeca.html

JS:   do { i++; } while (i < 10);
来源：http://hz.redwolf501.top/gtfhbavbwc.html

TS:   do { i++; } while (i < 10);
来源：http://hz.wangdashe.top/gtzddyjsjh.html

Java: do { i++; } while (i < 10);
来源：http://hz.andypj.xyz/gtnuqtfzen.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.vqdsnc.cn/gtnkcjsade.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhoulong.xyz/gtgthpdwwa.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhiwuduotai.top/gtgwgigsqv.html

[B09] break 与 continue
来源：http://hz.jinqigfzy.top/gtwgtidnxu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.meibo888.top/gtlwmsczfb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.316326.xyz/gtnfarrrrb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.havefunace.top/gtexsvapuv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fengsongda.top/gtfwlzfjag.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pengpengdd.cyou/gtmjtbgjxl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hywenlv.cn/gteoayuamf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hysaishi.cn/gtpkzhqmcv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pengpengdd.cyou/gtwkfjfyis.html

[B10] 遍历同时拿索引
来源：http://hz.zhixingplan.top/gtabkgqmum.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ywan-chungtsiang.top/gtdaoqkwup.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.shangyingyoupin.top/gtkwgubdcz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.cheryme.top/gtqlgxamcb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ivvv.top/gtuyrgcaly.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinghuilouyu.cn/gtdpxkevvj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj202588.top/gtddrrtpci.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yonumen.top/gtuojtvqzh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.dashuyun.cn/gtodgyeskm.html

[B11] 生成数字序列 / 区间
来源：http://hz.shangyingyoupin.top/gtyudnjooa.html

Py:   list(range(0, 10, 2))
来源：http://hz.jinghuilouyu.cn/gtlvxidxhv.html

PHP:  range(0, 10, 2);
来源：http://hz.xingfuxueyuan.xyz/gthgiaqmrl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shzxlz.cn/gtqyosgxbh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.havefunace.top/gtmjtsporo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shanyushiyangkeji.top/gthlnnehdq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gotoacloud.top/gtikhhhvui.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yj20258.top/gtbscqhiae.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.daxiang520.top/gtrhmxtqqa.html

[B12] 跳出多层循环
来源：http://hz.ppjwa.cn/gtzqhmhieh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hysaishi.cn/gtokgrbnxs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yonumen.top/gtbsynqwoi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gteimniubn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dianchejie.cn/gtcmfonihl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtzyixqxlw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nanxuanxn.top/gtsqjvjcai.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.iojbl.cn/gtrphtwcqj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cheryme.top/gtazbgqgkx.html

[B13] 判断是否为数字
来源：http://hz.zhijiandao.cn/gtizmwjpor.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinqigfzy.top/gtrzhmvvzr.html

PHP:  is_numeric($x)
来源：http://hz.chenzaomai.com/gtywjrbquy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shanyushiyangtech.top/gtrgquzmjl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cdnleiting.top/gtopahevaw.html

Java: x instanceof Number
来源：http://hz.0kj1m.cn/gtvqcxeugi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.chenlongwang.top/gtynzcayrq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jinyuanbaomall.cn/gtoaniguxb.html

C#:   x is int or double or decimal
来源：http://hz.haohaochexian.top/gtfalenjqh.html

[B14] 判断值是否在集合内
来源：http://hz.tian-w.cn/gtaknqkbnn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.aibaodan.cn/gtgpzidyrv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenzaomai.com/gtlkubwljo.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangkeji.top/gtfpovnaie.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.pengpengdd.cyou/gtyqqujuqa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.sysykeji.top/gtamiumvhz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhaomingkeji.xyz/gtltpzehzs.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj202588.top/gtiozkqisz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.wangshuangyany.cn/gtcniyrfuk.html

[B15] 布尔运算与取反
来源：http://hz.xuetiantiany.cn/gtoxmpmzst.html

Py:   a and b or not c
来源：http://hz.jinqigufen.top/gtzrsukexs.html

PHP:  $a && $b || !$c
来源：http://hz.wangshuangyany.cn/gtftqjmxhh.html

JS:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtfrtymrny.html

TS:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtdhrwyljn.html

Java: a && b || !c
来源：http://hz.nanxuanxn.top/gtaqmzkdqt.html

Go:   a && b || !c
来源：http://hz.yanxiufei.cn/gtdugrjkbo.html

Ruby: a && b || !c
来源：http://hz.zhoulong.xyz/gtsagjeuzf.html

C#:   a && b || !c
来源：http://hz.gaohongyu789.top/gtqhpdauyo.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.svipenyu.cn/gtaacslvgd.html

Py:   if not data: return
来源：http://hz.aibaodan.cn/gtognnzrit.html

PHP:  if (!$data) { return; }
来源：http://hz.gotoacloud.top/gtvygvlrmv.html

JS:   if (!data) return;
来源：http://hz.tianlin.xyz/gtuyixzknj.html

TS:   if (!data) return;
来源：http://hz.jyoumei.cn/gtybrnhpvx.html

Java: if (data == null) return;
来源：http://hz.ivvv.top/gtqjufjhhd.html

Go:   if data == nil { return }
来源：http://hz.shzxlz.cn/gtoibtojhd.html

Ruby: return if data.nil?
来源：http://hz.jqgufenzy.top/gtpzxftjcs.html

C#:   if (data == null) return;
来源：http://hz.hnqzz.top/gthuutzpvb.html

================================================================================
来源：http://hz.yonumen.top/gtueiybikv.html

C. 函数与作用域
来源：http://hz.cheryme.top/gttxniucdv.html

================================================================================
来源：http://hz.sxryk.cn/gtfemvebrw.html

[C01] 定义函数
来源：http://hz.zhixingplan.top/gtdtvxgher.html

Py:   def add(a, b): return a + b
来源：http://hz.hfpthk.cn/gtwgdghahj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtapbroqji.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinqigufen.top/gtlpzbiefe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.52xcode.cn/gtneckkxld.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtemvhobcm.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jqgufenzy.top/gtbwkysbyb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhiwuduotai.top/gtlxfywjzn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtxhrwhfqm.html

[C02] 默认参数
来源：http://hz.ehwqpu.com/gtluzlxxog.html

Py:   def greet(name="World"): return name
来源：http://hz.shangyingyoupin.top/gtiiavjicp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xylfe.cn/gtkyhlaacc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xziqi.cn/gtaikfxtcz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hnqzz.top/gtubyzjcre.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tian-w.cn/gtdogickgj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shuidangran.top/gtapgswtwd.html

Ruby: def greet(name = "World") = name
来源：http://hz.chenzaomai.com/gttbglsdwa.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jlsjyb.cn/gttvpfatrn.html

[C03] 可变参数
来源：http://hz.zhixingplan.top/gtyrllycbn.html

Py:   def total(*args): return sum(args)
来源：http://hz.kuanghao11.cn/gtcrcbotsz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.9152youxi.cn/gtjoyjxkrl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.smart0.xyz/gtwbndiwrw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gaohongyu789.top/gtfecjfdvp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hysaishi.cn/gtfwaycqgj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ivvv.top/gtobzozomn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinqigfzy.top/gtiabcrmhh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.c1oappe.top/gtrhmkyrve.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zycfv.cn/gtrubeigwh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cashguo.top/gtjolefyhi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yanxiufei.cn/gtzixsqxyx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.smart0.xyz/gtctlnizcj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.52xcode.cn/gtqdznwzfj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cucudq.cn/gtguxojgyw.html

Go:   // 无：用配置结构体参数
来源：http://hz.mhx1999.top/gtgvelmuca.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yanxiufei.cn/gtoujgqiqz.html

C#:   f(a: 1, b: 2)
来源：http://hz.redwolf501.top/gtqzuvunhd.html

[C05] 返回多个值
来源：http://hz.jinyuanbaomall.cn/gtucdescpz.html

Py:   return a, b
来源：http://hz.birdmap.top/gtgovbrtys.html

PHP:  return [$a, $b];
来源：http://hz.gaohongyu789.top/gtsdkraowm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hywenlv.cn/gtwyqwewml.html

TS:   return { a, b };
来源：http://hz.xinyue.icu/gtkyaohnwo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jianghu66.top/gtsrbzvhuq.html

Go:   return a, b
来源：http://hz.shanyushiyangtech.top/gtbfxdfsir.html

Ruby: return a, b
来源：http://hz.andypj.xyz/gtidomvwpr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xziqi.cn/gtdvursdin.html

[C06] 匿名函数 / lambda
来源：http://hz.guowangkeji.top/gtscknabcr.html

Py:   square = lambda x: x * x
来源：http://hz.shanyushiyangkeji.top/gtnzopejty.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xuetiantiany.cn/gtkadvlavz.html

JS:   const square = x => x * x;
来源：http://hz.pycfn.com/gtffxozxgl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhaomingkeji.xyz/gtaiuoulsj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.tian-w.cn/gtsrrnjdhl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.wangshuangyany.cn/gtrenjctdz.html

Ruby: square = ->(x) { x * x }
来源：http://hz.52xcode.cn/gteasenqif.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yuanzhike.top/gtbsynmhls.html

[C07] 把函数作为参数传入
来源：http://hz.quarkkingdee.top/gtqmvcfqwa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jianghu66.top/gtqkktqjtw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.havefunace.top/gtmvtsuhwc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.wangdashe.top/gtnzgwedcb.html

TS:   arr.map(String)
来源：http://hz.xylfe.cn/gtsvbszvhx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yongpay.top/gtpygnwuou.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tian-w.cn/gtyuclgwkg.html

Ruby: arr.map(&:upcase)
来源：http://hz.aibaodan.cn/gtqazenezp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gotoacloud.top/gthcavitdw.html

[C08] 闭包
来源：http://hz.aibaodan.cn/gtlzsvsnkl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangtech.top/gtfewyscxa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xuanzx.com/gtlubtikhy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtziompqyd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnqzz.top/gtjtfsdnxi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.9152youxi.cn/gtmsrtwmei.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hfpthk.cn/gtfmmooeus.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hongshengwenyu.top/gtwcmsxyit.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.daria6918.cn/gtttfuqpcu.html

[C09] 递归
来源：http://hz.xuetiantiany.cn/gtczojgemq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtsbmduxgl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cucudq.cn/gteggimgeu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.0kj1m.cn/gtsdjcyksu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydjk.org.cn/gtwahwsslm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258.top/gtyaozszvx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hysaishi.cn/gtcwixdyjf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtlrmlrhca.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cashguo.top/gtnotdfimw.html

[C10] 变量作用域
来源：http://hz.jinqigfzy.top/gttjsuomku.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yongpay.top/gtcirddtbi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hfpthk.cn/gtckmywugz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hnxiangtu.top/gtzfgzhyai.html

TS:   同 JS
来源：http://hz.hysaishi.cn/gtgiuoxpwr.html

Java: 方法内为块级作用域
来源：http://hz.ehwqpu.com/gtczvhhshq.html

Go:   花括号块级作用域
来源：http://hz.jianghu66.top/gtvbjzwkhf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sxryk.cn/gtexbotlik.html

C#:   块级作用域
来源：http://hz.iojbl.cn/gtznuaoesd.html

[C11] 模块导入与导出
来源：http://hz.chenlongwang.top/gtbttrtjur.html

Py:   from module import func
来源：http://hz.zhijiandao.cn/gtdcapqwem.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj20258888.top/gterfvykyt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhongyouzk.top/gthdgqfwem.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.mhx1999.top/gtqmggpxpz.html

Java: import java.util.List;
来源：http://hz.snrcjt.cn/gtvhyqfdcm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj202588.top/gtypwmfiht.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258.top/gtdrxmozql.html

C#:   using System.Text;
来源：http://hz.shanyushiyangtech.top/gtzuxsdxte.html

[C12] 立即执行函数 IIFE
来源：http://hz.ywan-chungtsiang.top/gtlkzrjvgd.html

Py:   (lambda: print("run"))()
来源：http://hz.smart0.xyz/gthcbjyxxh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hfpthk.cn/gtdwpymyld.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhongyouzk.top/gtzidxtcuf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.smart0.xyz/gtpdztwypn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.wangdashe.top/gtbpqbieya.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.smart0.xyz/gtbfboqsxb.html

Ruby: -> { puts "run" }.call
来源：http://hz.sufxvd.cn/gtofaprgdv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.mhx1999.top/gtqovipnnf.html

[C13] 类型声明 / 类型注解
来源：http://hz.jinyuanbaomall.cn/gtdbeohlwh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.quarkkingdee.top/gtefqieyyh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtrfyzqmqu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuxming.cn/gtufsihasp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guowangkeji.top/gtvbqxlhtx.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jqgufenzy.top/gtouicxkgo.html

Go:   func add(a, b int) int
来源：http://hz.yonumen.top/gthcnvgqwh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.0kj1m.cn/gttjxsbtpm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxuanxn.top/gtpmqvkxjz.html

[C14] 泛型函数
来源：http://hz.yueranfly.top/gtezeiwymm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.0kj1m.cn/gtotwaqnzj.html

PHP:  // 无泛型
来源：http://hz.meibo888.top/gtabiovogg.html

JS:   // 无泛型
来源：http://hz.sysykeji.top/gtwuwemkzn.html


<!-- 参考信息 -->