代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.cdnleiting.top/gtknftkqwd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.hysaishi.cn/gtmaqnhunz.html

[A24] 去除首尾空白
来源：http://hz.aizwys.cn/gtmxsctrqu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.mhx1999.top/gtyizprnbg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.birdmap.top/gtghfhlous.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.meibo888.top/gtrmwtecfd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tianlin.xyz/gtoamumarg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.xuetiantiany.cn/gtkskzukod.html

Go:   strings.TrimSpace(s)
来源：http://hz.gotoacloud.top/gthjdovriy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hywenlv.cn/gtxrwduiid.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.ydzc1.top/gtsfuwirku.html

[A25] 字符串比较
来源：http://hz.chenzaomai.com/gteemtaahd.html

Py:   s1 == s2; s1 != s2
来源：http://hz.guowangkeji.top/gtyfpbpzhy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ydjk.org.cn/gtyrsaqjta.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhiwuduotai.top/gtxmvtgfnn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinqigfzy.top/gtxnwqaxgp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yanxiufei.cn/gtjclvkhqc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zhongyouzk.top/gtkboxmkhv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.tianlin.xyz/gtefjhnwko.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xziqi.cn/gtrgnamdiv.html

[A26] 类型转换总览
来源：http://hz.ehwqpu.com/gtihanzqaz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.sxryk.cn/gttsksoefg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zhijiandao.cn/gtwvejrxuz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.nwbrower.top/gtoznxfsen.html

TS:   Number() String() Boolean() x as number
来源：http://hz.cdnleiting.top/gtcduwaclv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.haohaochexian.top/gtpqndoynr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yongpay.top/gtyflnpaeu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.gotoacloud.top/gtudcwrkyh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.daria6918.cn/gteztzyrkv.html

================================================================================
来源：http://hz.yueranfly.top/gtzlolzjdp.html

B. 流程控制
来源：http://hz.ydzc1.top/gtlpaukacv.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtssgqwcsi.html

[B01] 条件判断 if / else
来源：http://hz.shuidangran.top/gtvyceetqy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jyoumei.cn/gtuvdzxmlr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.tianlin.xyz/gtkyhbdbso.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhoulong.xyz/gtbbwzlons.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sxryk.cn/gtsrjizdxz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yuanzhike.top/gtgsibuknu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ywan-chungtsiang.top/gtajvcmrcv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yanxiufei.cn/gtcvgeajec.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.daxiang520.top/gtreiyloaa.html

[B02] 多分支 else if / elif
来源：http://hz.jianghu66.top/gtmwlmqrib.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.hammf.cn/gteblunnfg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.andypj.xyz/gtmbqkofkk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.meibo888.top/gtoqyruahh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuanzx.com/gtfhtuxneb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hysaishi.cn/gtpptlnilx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.fzhhl.top/gtxwtcqxkv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.redwolf501.top/gtlqcsttzd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cheryme.top/gtetuzmqmx.html

[B03] switch / match / case
来源：http://hz.yj20258.top/gtouwxqfvi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.kuanghao11.cn/gtatpgycwy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.daxiang520.top/gtfzeackei.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.tanke756.top/gtggpvfwex.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.wangdashe.top/gtqdlbfujf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.smart0.xyz/gtbeleensp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.guannengcc.top/gtlpoyiwyl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ywan-chungtsiang.top/gtdeqyukym.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.shanyushiyangkeji.top/gthegnmgoz.html

[B04] for 计数循环
来源：http://hz.smart0.xyz/gtjfgwoydn.html

Py:   for i in range(10): print(i)
来源：http://hz.xingfuxueyuan.xyz/gtvkdltbvk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.fzhhl.top/gttmmjythz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.tian-w.cn/gtufcrxcek.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinghuilouyu.cn/gtnkwkqlep.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ppjwa.cn/gtmlvrmrbt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.vqdsnc.cn/gtkcbvouuf.html

Ruby: 10.times { |i| puts i }
来源：http://hz.chenlongwang.top/gtexxwntus.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xinyue.icu/gtutvlwlld.html

[B05] 遍历数组 / 列表
来源：http://hz.xuetiantiany.cn/gtohxtonsv.html

Py:   for item in arr: print(item)
来源：http://hz.ydzc1.top/gtwswhrhnv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jianghu66.top/gtsknjmfmp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenzaomai.com/gtxtiakkpm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jinqigufen.top/gtofgcslwc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jqgufenzy.top/gtingkrajj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cashguo.top/gtdrinhwlh.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jinyuanbaomall.cn/gtfbfrjmgm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.316326.xyz/gtodqxoicz.html

[B06] 遍历字典 / 对象
来源：http://hz.dashuyun.cn/gtiuraukjb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yueranfly.top/gtrtkwjooz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.guowangkeji.top/gtlkqjygcq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinqigufen.top/gtiowpxzsz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj20258.top/gtznvvebki.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.aibaodan.cn/gtjwibowqu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ppjwa.cn/gtkikgmvax.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.gzhubu.top/gteplsjpuf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.ybcxt.top/gtvocnagdk.html

[B07] while 循环
来源：http://hz.yj20258.top/gtlfamhpvl.html

Py:   while i < 10: i += 1
来源：http://hz.zhijiandao.cn/gtiqgpmefu.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xziqi.cn/gtpcnvsjpt.html

JS:   while (i < 10) { i++; }
来源：http://hz.pycfn.com/gteokedlde.html

TS:   while (i < 10) { i++; }
来源：http://hz.sxryk.cn/gtmsqlrhei.html

Java: while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtmlobabpf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.aibaodan.cn/gtrbyhcbcx.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhaomingkeji.xyz/gtfmclzvvn.html

C#:   while (i < 10) { i++; }
来源：http://hz.gogol.net.cn/gtzcilhqqv.html

[B08] do-while（至少执行一次）
来源：http://hz.nanxinkj.top/gtmrlhdjdu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ppjwa.cn/gtcmkbrgwh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.wangshuangyany.cn/gtgeboshrd.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gtwankpmip.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yanxiufei.cn/gtrbgkbrrk.html

Java: do { i++; } while (i < 10);
来源：http://hz.vqdsnc.cn/gtmtqyevhw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.sysykeji.top/gtupvpiakg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yongpay.top/gtiksvwxgt.html

C#:   do { i++; } while (i < 10);
来源：http://hz.daria6918.cn/gtfpgwpwxf.html

[B09] break 与 continue
来源：http://hz.nanxuanxn.top/gtgbmyxheq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.tian-w.cn/gtrxdsuvuh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtdfzolfre.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yonumen.top/gtunmsorlk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.svipenyu.cn/gturjnmgij.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gttnifflqf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhijiandao.cn/gtvhfekkjw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xziqi.cn/gtfbudklwz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.andypj.xyz/gtrbdhoiou.html

[B10] 遍历同时拿索引
来源：http://hz.zhongyouzk.top/gtmscnlgad.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinghuilouyu.cn/gtrrruisjz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zycfv.cn/gtfoseylzi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ydzc1.top/gtsihosbhg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.nwbrower.top/gtghovymdt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.chenjidiqi.icu/gtunxzhisk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ivvv.top/gtnrnpcmqi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.9152youxi.cn/gtshbqepeg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gzhubu.top/gtspsasucv.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhengqikj.top/gtjxmsrdwz.html

Py:   list(range(0, 10, 2))
来源：http://hz.mhx1999.top/gtqauumetv.html

PHP:  range(0, 10, 2);
来源：http://hz.ivvv.top/gtutcspeyr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jiagoushi.top/gtwxhbcipl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.havefunace.top/gtvmjwhaps.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shangyingyoupin.top/gttxqmagyj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hammf.cn/gtpsnlqdpf.html

Ruby: (0...10).step(2).to_a
来源：http://hz.dianchejie.cn/gtmxctudsc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.c1oappe.top/gtixnrphho.html

[B12] 跳出多层循环
来源：http://hz.andypj.xyz/gtloourmfv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhaomingkeji.xyz/gtlvoklmyl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yuxming.cn/gtrisrcwzb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinghuilouyu.cn/gtzrhwcqfj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.52xcode.cn/gtteofjhcp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhongyouzk.top/gtwlpijukf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yangfankeji.com/gtezfnxwcj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cdnleiting.top/gtprzzpyuz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cheryme.top/gtxfanqpmm.html

[B13] 判断是否为数字
来源：http://hz.c1oappe.top/gtyzghjxzi.html

Py:   isinstance(x, (int, float))
来源：http://hz.yuanzhike.top/gthlcdpasd.html

PHP:  is_numeric($x)
来源：http://hz.redwolf501.top/gtcbhhwfin.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daxiang520.top/gtuxcldpya.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cqqwz.cn/gthuspqnrg.html

Java: x instanceof Number
来源：http://hz.cheryme.top/gtbebuphnj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.daria6918.cn/gtjwibujgd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hfpthk.cn/gtofcwyaft.html

C#:   x is int or double or decimal
来源：http://hz.bjfxy.top/gtcfrikevw.html

[B14] 判断值是否在集合内
来源：http://hz.ywan-chungtsiang.top/gttcxtfoib.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yuxming.cn/gtpqshxhfy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jinghuilouyu.cn/gtdeegikas.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xinyue.icu/gtxhyzkdlf.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.chenzaomai.com/gtfehyrjgq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.snrcjt.cn/gtregklqtn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yonumen.top/gtrazxicnl.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cashguo.top/gtapznjgqf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ppjwa.cn/gtvfjxxbtw.html

[B15] 布尔运算与取反
来源：http://hz.smart0.xyz/gthalngsid.html

Py:   a and b or not c
来源：http://hz.birdmap.top/gthqbvvpms.html

PHP:  $a && $b || !$c
来源：http://hz.c1oappe.top/gtssartgmp.html

JS:   a && b || !c
来源：http://hz.yvedp.cn/gtswogolkt.html

TS:   a && b || !c
来源：http://hz.sweek.top/gtiqzvtosl.html

Java: a && b || !c
来源：http://hz.hfpthk.cn/gtpgzhwbqb.html

Go:   a && b || !c
来源：http://hz.yangfankeji.com/gtkrjcezby.html

Ruby: a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtlylbfves.html

C#:   a && b || !c
来源：http://hz.svipenyu.cn/gttrjbisyk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhixingplan.top/gtfjhewdzw.html

Py:   if not data: return
来源：http://hz.iojbl.cn/gthedolmlt.html

PHP:  if (!$data) { return; }
来源：http://hz.cucudq.cn/gthjkaiuii.html

JS:   if (!data) return;
来源：http://hz.zhiwuduotai.top/gtrxmucmyd.html

TS:   if (!data) return;
来源：http://hz.aibaodan.cn/gtdvgownua.html

Java: if (data == null) return;
来源：http://hz.ydjk.org.cn/gtvuzglmoi.html

Go:   if data == nil { return }
来源：http://hz.jinyuanbaomall.cn/gtwqgneqkt.html

Ruby: return if data.nil?
来源：http://hz.ehwqpu.com/gtzpfcbyzr.html

C#:   if (data == null) return;
来源：http://hz.nanxuanxn.top/gtfuifcjxm.html

================================================================================
来源：http://hz.jianghu66.top/gtlgtiygra.html

C. 函数与作用域
来源：http://hz.yongpay.top/gthmnqxskx.html

================================================================================
来源：http://hz.fzhhl.top/gtrvbwoajk.html

[C01] 定义函数
来源：http://hz.gotoacloud.top/gtwataevfk.html

Py:   def add(a, b): return a + b
来源：http://hz.kuanghao11.cn/gtabgvthek.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtjwoyjzhu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.c1oappe.top/gtwkelrozs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtngylssxj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtxwwnsags.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ivvv.top/gthpldbwaa.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yonumen.top/gtqmznlmsi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtrpmgfwzh.html

[C02] 默认参数
来源：http://hz.wangshuangyany.cn/gtvkfrklzl.html

Py:   def greet(name="World"): return name
来源：http://hz.sweek.top/gtvinzuepb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jqgfzy.top/gtgdheiheh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jqgfzy.top/gtynlspwte.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtcbpysubk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xuetiantiany.cn/gtnmzphhxy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sxryk.cn/gtllpjouej.html

Ruby: def greet(name = "World") = name
来源：http://hz.jiagoushi.top/gtkcwxmcje.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.wangdashe.top/gtoctpozvz.html

[C03] 可变参数
来源：http://hz.daria6918.cn/gtzatuybqe.html

Py:   def total(*args): return sum(args)
来源：http://hz.jyoumei.cn/gtfxhwfoxe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yueranfly.top/gtxexbqumt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gtuvlqykdd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.smart0.xyz/gtyhjgitvf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.smart0.xyz/gtpjzcuftr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhengqikj.top/gtxmuajntu.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxinkj.top/gttonqoaua.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.aizwys.cn/gtxcrbcukt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhaomingkeji.xyz/gtchdilivf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tian-w.cn/gtefuvazyc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hfpthk.cn/gtkjnznrhi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cqqwz.cn/gtercxuetu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.quarkkingdee.top/gtaicxeupx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.wangdashe.top/gtzvqooqjg.html

Go:   // 无：用配置结构体参数
来源：http://hz.pengpengdd.cyou/gtlvseymkm.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yuxming.cn/gtasfwckxi.html

C#:   f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtwcbkajwk.html

[C05] 返回多个值
来源：http://hz.vqdsnc.cn/gtkichjqrr.html

Py:   return a, b
来源：http://hz.havefunace.top/gtrazpsbqs.html

PHP:  return [$a, $b];
来源：http://hz.svipenyu.cn/gtzkmtkohn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jlsjyb.cn/gteyqtuwqt.html

TS:   return { a, b };
来源：http://hz.pengpengdd.cyou/gtfhuhuete.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.guannengcc.top/gtpxzvgzxe.html

Go:   return a, b
来源：http://hz.meibo888.top/gtmocddefb.html

Ruby: return a, b
来源：http://hz.zhiwuduotai.top/gtrfyqxsdm.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhoulong.xyz/gtgpoaeivq.html

[C06] 匿名函数 / lambda
来源：http://hz.nwbrower.top/gtygeyxdex.html

Py:   square = lambda x: x * x
来源：http://hz.jqgufenzy.top/gtqxkpnxkj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xylfe.cn/gtfqubsmzf.html

JS:   const square = x => x * x;
来源：http://hz.yonumen.top/gtamqbbsvo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhoulong.xyz/gtpbevbugk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hongshengwenyu.top/gtwqoytrom.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.sweek.top/gtvcyijyyv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hywenlv.cn/gthsfgplgk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ivvv.top/gteespmklr.html

[C07] 把函数作为参数传入
来源：http://hz.zhongyouzk.top/gthbddofex.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sxryk.cn/gtgxlrpftb.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj202588.top/gtsvabfmlk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shangyingyoupin.top/gtjdcummtg.html

TS:   arr.map(String)
来源：http://hz.zhaomingkeji.xyz/gtiiexcmzo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.wangshuangyany.cn/gtwrkhlswr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinqigfzy.top/gtvnxfeikk.html

Ruby: arr.map(&:upcase)
来源：http://hz.hysaishi.cn/gtqmphxpwo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jlsjyb.cn/gttfnrsehf.html

[C08] 闭包
来源：http://hz.kuanghao11.cn/gtgmsbzfem.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhongyouzk.top/gtgciqgoxv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangkeji.top/gtizeccigq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gtqjmtuhzv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtnpxyjkmq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinghuilouyu.cn/gtktddalfk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ywan-chungtsiang.top/gtopdbzumg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.0kj1m.cn/gtimnmwexl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtrdjvgepi.html

[C09] 递归
来源：http://hz.ydzc1.top/gtoewhlixj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nanxuanxn.top/gtghkuqhao.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhixingplan.top/gtyjheynzz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.0kj1m.cn/gteefxnykv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dianchejie.cn/gtjbsgmowh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.haohaochexian.top/gtenashnmc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tanke756.top/gtkwzfjzaj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtooxducce.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.pycfn.com/gtcnbzhwak.html

[C10] 变量作用域
来源：http://hz.jqgfzy.top/gtjcbjhsxa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jianghu66.top/gtxwbfopcc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jianghu66.top/gthyutrpum.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinqigufen.top/gttfbovtna.html

TS:   同 JS
来源：http://hz.xuanzx.com/gtzdxofrzq.html

Java: 方法内为块级作用域
来源：http://hz.ydzc1.top/gtpvupbgze.html

Go:   花括号块级作用域
来源：http://hz.jqgfzy.top/gttklncchk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhijiandao.cn/gtftunzajk.html

C#:   块级作用域
来源：http://hz.meibo888.top/gtekfnpagm.html

[C11] 模块导入与导出
来源：http://hz.yonumen.top/gtvaiuzmaa.html

Py:   from module import func
来源：http://hz.316326.xyz/gtqkaiumhz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinghuilouyu.cn/gtmchuzzeq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shanyushiyangkeji.top/gtkqlhvdwr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.c1oappe.top/gttndcaplp.html

Java: import java.util.List;
来源：http://hz.shuidangran.top/gtdctwsctg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yvedp.cn/gtuermgwia.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xuetiantiany.cn/gtlhaoplbq.html

C#:   using System.Text;
来源：http://hz.yvedp.cn/gtlbvwcvhb.html

[C12] 立即执行函数 IIFE
来源：http://hz.haohaochexian.top/gtxrlernkx.html

Py:   (lambda: print("run"))()
来源：http://hz.jlsjyb.cn/gthumxmmqr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jianghu66.top/gtroxmoidx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yonumen.top/gtfchmhzbr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sufxvd.cn/gtwxtuzsjn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgufenzy.top/gtmncjvmxr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.fengsongda.top/gtqbpseswv.html

Ruby: -> { puts "run" }.call
来源：http://hz.yuanzhike.top/gtvajxpxpa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.chenjidiqi.icu/gtdkwbgddi.html

[C13] 类型声明 / 类型注解
来源：http://hz.havefunace.top/gtecgzognm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.haohaochexian.top/gtfklvaddx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.iojbl.cn/gtgawxinkg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gotoacloud.top/gtgfvnnlvj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shuidangran.top/gtyaamrhng.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtzlkwdtuz.html

Go:   func add(a, b int) int
来源：http://hz.hysaishi.cn/gtyqnitmci.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.0kj1m.cn/gtceslbhvx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yuanzhike.top/gtinfgmnxo.html

[C14] 泛型函数
来源：http://hz.yangfankeji.com/gtscccwnad.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cheryme.top/gtacyfzytm.html

PHP:  // 无泛型
来源：http://hz.tanke756.top/gtmdparwgl.html

JS:   // 无泛型
来源：http://hz.fzhhl.top/gtqfkhovlu.html


<!-- 参考信息 -->