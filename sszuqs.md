代发 wailian999

C#:   s.Length
来源：http://hz.aizwys.cn/gtkcujlghk.html

[A23] 大小写转换
来源：http://hz.xylfe.cn/gtbofqojca.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.gotoacloud.top/gthdwocxtg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.pycfn.com/gtbibqmqpe.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.smart0.xyz/gtiwfxegpe.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xuanzx.com/gtvrhbxknu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yongpay.top/gtjtdrezbl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.fzhhl.top/gtjkdtgxft.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xuanzx.com/gtilrooulw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jinqigfzy.top/gtgcwvibjd.html

[A24] 去除首尾空白
来源：http://hz.jlsjyb.cn/gtyusccxbo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.zycfv.cn/gthfjckxuw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.sufxvd.cn/gtxjrlpasy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cucudq.cn/gtpagasjyq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xuetiantiany.cn/gttizwoluu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.cucudq.cn/gtjydijanm.html

Go:   strings.TrimSpace(s)
来源：http://hz.cqqwz.cn/gtkqadqpwl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hnqzz.top/gtsasuzjvn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.zhiwuduotai.top/gtleyjvdre.html

[A25] 字符串比较
来源：http://hz.zhaomingkeji.xyz/gtpckjtkic.html

Py:   s1 == s2; s1 != s2
来源：http://hz.wangdashe.top/gtufnywmnu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.haohaochexian.top/gtbtfrngqv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.guowangkeji.top/gtcwmojlnf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tanke756.top/gtstthngng.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.dashuyun.cn/gtlmgnhccd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.snrcjt.cn/gthfryzyob.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.pengpengdd.cyou/gtjjellhdz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.gotoacloud.top/gteyrrczwk.html

[A26] 类型转换总览
来源：http://hz.tianlin.xyz/gtcqjehmii.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.dianchejie.cn/gttkozoqzy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.nanxinkj.top/gtjoaxixih.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.shuidangran.top/gthmpkygyr.html

TS:   Number() String() Boolean() x as number
来源：http://hz.meibo888.top/gtpczcznvi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yueranfly.top/gthtvwckdd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.smart0.xyz/gtrmrsgdfn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.mhx1999.top/gthrlsfmyw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.sweek.top/gtiuvjakqn.html

================================================================================
来源：http://hz.316326.xyz/gtidvewest.html

B. 流程控制
来源：http://hz.xylfe.cn/gtdwuxqjps.html

================================================================================
来源：http://hz.yj20258888.top/gtavkompff.html

[B01] 条件判断 if / else
来源：http://hz.zhijiandao.cn/gtlobkdxsf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.52xcode.cn/gtbzirljzf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.nwbrower.top/gtqruafxvm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.daxiang520.top/gtpipvxijt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.redwolf501.top/gtvgehhfwn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.gogol.net.cn/gtnhfcxxfn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.snrcjt.cn/gtcdvockes.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.52xcode.cn/gtihhjarid.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.sxryk.cn/gttuatzkos.html

[B02] 多分支 else if / elif
来源：http://hz.haohaochexian.top/gtoyxxtsxg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.haohaochexian.top/gtovaaqjfj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhijiandao.cn/gtesgscvgb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.quarkkingdee.top/gtnflivbdn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangdashe.top/gtguyasgza.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtcjsqdgzg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jyoumei.cn/gtdvswvdhv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.redwolf501.top/gtznsvchpr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gaohongyu789.top/gtbezblkba.html

[B03] switch / match / case
来源：http://hz.yj20258.top/gtzsixwsau.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.pengpengdd.cyou/gthckvhejd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.316326.xyz/gtvrjbrwlz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gotoacloud.top/gtwpshmizk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yuanzhike.top/gtzjslkznu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.smart0.xyz/gtrwqsnpfu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yuxming.cn/gtgzmbxgud.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.shanyushiyangtech.top/gttnrlfxgx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.fzhhl.top/gtrntqcpwl.html

[B04] for 计数循环
来源：http://hz.ydjk.org.cn/gtubfebtmg.html

Py:   for i in range(10): print(i)
来源：http://hz.yanxiufei.cn/gtksribakh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.gogol.net.cn/gtfrimqikk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jlsjyb.cn/gtfnianlhl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pengpengdd.cyou/gtgrtcjpsq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.gaohongyu789.top/gtzafwtalg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.haohaochexian.top/gtnnwclbue.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shangyingyoupin.top/gtaqhvlqlq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.aizwys.cn/gttzwwkuni.html

[B05] 遍历数组 / 列表
来源：http://hz.hnxiangtu.top/gtpawmnmsq.html

Py:   for item in arr: print(item)
来源：http://hz.nanxuanxn.top/gtaywljnvz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yvedp.cn/gtrjguvzkm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.cdnleiting.top/gtmysythpc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.iojbl.cn/gtqjylcmxz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.cdnleiting.top/gtmfnpfzce.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.gzhubu.top/gtommpyoam.html

Ruby: arr.each { |item| puts item }
来源：http://hz.wangdashe.top/gtcnlqapod.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.dianchejie.cn/gticcyxhaw.html

[B06] 遍历字典 / 对象
来源：http://hz.zhiwuduotai.top/gttmqqpogi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.daxiang520.top/gtmfccxmeq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yangfankeji.com/gtpwmnzmxk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gogol.net.cn/gtuhkdrzmw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.smart0.xyz/gtavykekfb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hongshengwenyu.top/gtvlqtxjxw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yongpay.top/gtaitdcekh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhijiandao.cn/gtphywhfgm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jinyuanbaomall.cn/gtajsshdzg.html

[B07] while 循环
来源：http://hz.haohaochexian.top/gteplzegve.html

Py:   while i < 10: i += 1
来源：http://hz.ydzc1.top/gtpifmvevp.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ivvv.top/gtaysujmst.html

JS:   while (i < 10) { i++; }
来源：http://hz.cheryme.top/gtdzomswxc.html

TS:   while (i < 10) { i++; }
来源：http://hz.sufxvd.cn/gtzniihaja.html

Java: while (i < 10) { i++; }
来源：http://hz.yongpay.top/gtwkqbbjnk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhixingplan.top/gtvotffexv.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yj20258.top/gtbiztycpg.html

C#:   while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gteaptqygh.html

[B08] do-while（至少执行一次）
来源：http://hz.gotoacloud.top/gtybsgdtjz.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ywan-chungtsiang.top/gtqxjmhuwt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gogol.net.cn/gtlcbahxke.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yj202588.top/gtbmwyrngj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ydzc1.top/gtfvmvpcmp.html

Java: do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtmktjxlwe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.316326.xyz/gtjvraljqj.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ehwqpu.com/gtvdpumbve.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gtdubjdlug.html

[B09] break 与 continue
来源：http://hz.vqdsnc.cn/gtrwtnhqlz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gaohongyu789.top/gtmfikevfz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.snrcjt.cn/gtqptgylga.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.9152youxi.cn/gtdtldpatt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydjk.org.cn/gtvwmptnmh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tianlin.xyz/gtuzsufirc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jyoumei.cn/gteqzlvlja.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.pycfn.com/gtfqvarsap.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.kuanghao11.cn/gtiqxuucdw.html

[B10] 遍历同时拿索引
来源：http://hz.yangfankeji.com/gtvcuvhgyo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shanyushiyangtech.top/gtfqozotqq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhoulong.xyz/gtlnfglwin.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hnqzz.top/gtxlwpakeg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.gaohongyu789.top/gtzsansbbp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yj202588.top/gtyjepxavl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.svipenyu.cn/gtkimrqvre.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.pengpengdd.cyou/gtmngpbngn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.xuanzx.com/gtzmzzwysg.html

[B11] 生成数字序列 / 区间
来源：http://hz.gaohongyu789.top/gtusojmgav.html

Py:   list(range(0, 10, 2))
来源：http://hz.cashguo.top/gtjmuuudfx.html

PHP:  range(0, 10, 2);
来源：http://hz.yanxiufei.cn/gthbppbrcf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nanxinkj.top/gtpgymtzek.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yangfankeji.com/gtrfaorycs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.feifeiyinyue.top/gtlvsgbloi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gzhubu.top/gtnbwpshnn.html

Ruby: (0...10).step(2).to_a
来源：http://hz.haohaochexian.top/gtrfcwqwav.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xinyue.icu/gtggwmtqxa.html

[B12] 跳出多层循环
来源：http://hz.ppjwa.cn/gtexahtwnl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xingfuxueyuan.xyz/gtnfcfihhs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xinyue.icu/gtutyjdysw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gtsnclvwgc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daxiang520.top/gtektfhxnm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenjidiqi.icu/gtwmgghjhq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.tian-w.cn/gtshiethry.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.c1oappe.top/gtghkocmof.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tianlin.xyz/gtotanwuoa.html

[B13] 判断是否为数字
来源：http://hz.ydjk.org.cn/gtfhtiwolu.html

Py:   isinstance(x, (int, float))
来源：http://hz.yvedp.cn/gtkzcziouk.html

PHP:  is_numeric($x)
来源：http://hz.kuanghao11.cn/gttcdygxop.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ybcxt.top/gttxwljuhd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.birdmap.top/gtsolkvfmm.html

Java: x instanceof Number
来源：http://hz.jqgufenzy.top/gtiaurnukk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.dianchejie.cn/gtenlnmjuq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.wangshuangyany.cn/gtvrikeqkp.html

C#:   x is int or double or decimal
来源：http://hz.redwolf501.top/gtfrbkuddi.html

[B14] 判断值是否在集合内
来源：http://hz.gotoacloud.top/gttlekqpxi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.chenlongwang.top/gtqfolhuxt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nwbrower.top/gtgeiogmhs.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhongyouzk.top/gtzdriqprk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.quarkkingdee.top/gtcueeuzqg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.iojbl.cn/gtwtrxgexj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hammf.cn/gtpwvuxqdl.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.c1oappe.top/gttfomcoph.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtqaqwrkph.html

[B15] 布尔运算与取反
来源：http://hz.dashuyun.cn/gtyqlsshlc.html

Py:   a and b or not c
来源：http://hz.sufxvd.cn/gtctghuegb.html

PHP:  $a && $b || !$c
来源：http://hz.zhijiandao.cn/gtxspkqssj.html

JS:   a && b || !c
来源：http://hz.yonumen.top/gtnwhfgdxd.html

TS:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gthijyaylq.html

Java: a && b || !c
来源：http://hz.c1oappe.top/gtdfmxutsz.html

Go:   a && b || !c
来源：http://hz.cqqwz.cn/gtinvqlpwy.html

Ruby: a && b || !c
来源：http://hz.aizwys.cn/gtptjmgsph.html

C#:   a && b || !c
来源：http://hz.daria6918.cn/gthrudnnmp.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zycfv.cn/gtusrjgnrn.html

Py:   if not data: return
来源：http://hz.xinyue.icu/gthebjrtku.html

PHP:  if (!$data) { return; }
来源：http://hz.jqgufenzy.top/gtvxrpwrpe.html

JS:   if (!data) return;
来源：http://hz.nwbrower.top/gtnvbfggrn.html

TS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtybprvpha.html

Java: if (data == null) return;
来源：http://hz.0kj1m.cn/gtldgldlxj.html

Go:   if data == nil { return }
来源：http://hz.zhixingplan.top/gtzcokhxiy.html

Ruby: return if data.nil?
来源：http://hz.hysaishi.cn/gtgxxzdilc.html

C#:   if (data == null) return;
来源：http://hz.jinghuilouyu.cn/gtgnkfjhij.html

================================================================================
来源：http://hz.ydjk.org.cn/gtatyqmquz.html

C. 函数与作用域
来源：http://hz.hfpthk.cn/gtfdzwraqp.html

================================================================================
来源：http://hz.tanke756.top/gtnjbswrbu.html

[C01] 定义函数
来源：http://hz.ppjwa.cn/gtiashlaro.html

Py:   def add(a, b): return a + b
来源：http://hz.zhengqikj.top/gtvqqjocre.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtnapgtsod.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ydzc1.top/gtxxgyvqvv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jlsjyb.cn/gtoviaxmzg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtujymhmlw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xingfuxueyuan.xyz/gticsvxbkp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.meibo888.top/gtrtwudqzp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hywenlv.cn/gtzptufdkj.html

[C02] 默认参数
来源：http://hz.zhixingplan.top/gtopjacyvp.html

Py:   def greet(name="World"): return name
来源：http://hz.bjfxy.top/gtckwtwuhp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sysykeji.top/gtnzhbxjbr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shuidangran.top/gtykozhiea.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuanzhike.top/gtxxcipsty.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhixingplan.top/gtvfcmykzf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jiagoushi.top/gtdlftifrk.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinyuanbaomall.cn/gtjkwvutri.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ehwqpu.com/gtzxmvjekb.html

[C03] 可变参数
来源：http://hz.shuidangran.top/gtcmydywbi.html

Py:   def total(*args): return sum(args)
来源：http://hz.yanxiufei.cn/gtsatdeucx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yangfankeji.com/gtskrrpwmm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xingfuxueyuan.xyz/gtrsfmjhkv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydjk.org.cn/gtidkoosyv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hnxiangtu.top/gtyofulxaw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yangfankeji.com/gttjxzifhe.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yongpay.top/gtrgcqsvoo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.tian-w.cn/gtmqskulzi.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gogol.net.cn/gtgwsngrth.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj202588.top/gtwvfiprxk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.andypj.xyz/gtdlbidsjl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.bjfxy.top/gtdzpmyjfx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jyoumei.cn/gtmyhlwuwr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.guowangkeji.top/gtylxhjems.html

Go:   // 无：用配置结构体参数
来源：http://hz.sufxvd.cn/gtkyoeugal.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gtzxgqexts.html

C#:   f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtejqoezdq.html

[C05] 返回多个值
来源：http://hz.dashuyun.cn/gtckzeqzmj.html

Py:   return a, b
来源：http://hz.gzhubu.top/gtsnstsddu.html

PHP:  return [$a, $b];
来源：http://hz.svipenyu.cn/gtfyikstph.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shuidangran.top/gtdlqrxmvl.html

TS:   return { a, b };
来源：http://hz.yvedp.cn/gtgifnowoe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nanxinkj.top/gtnstaruft.html

Go:   return a, b
来源：http://hz.dashuyun.cn/gtnoaermuc.html

Ruby: return a, b
来源：http://hz.meibo888.top/gtraqxoqkb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinyuanbaomall.cn/gtieshjkyj.html

[C06] 匿名函数 / lambda
来源：http://hz.haohaochexian.top/gtpzubcuzb.html

Py:   square = lambda x: x * x
来源：http://hz.cheryme.top/gtrggfyagp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sufxvd.cn/gtqhfufqmu.html

JS:   const square = x => x * x;
来源：http://hz.jqgfzy.top/gtxxudenro.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinqigufen.top/gtpwkrxqyb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.tanke756.top/gtbhmawdrj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ehwqpu.com/gtohamxwgf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.kuanghao11.cn/gtaleczlch.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cashguo.top/gtkjxtblpm.html

[C07] 把函数作为参数传入
来源：http://hz.havefunace.top/gthtgzqeqv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.0kj1m.cn/gtguwiielj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ehwqpu.com/gtcrefkrko.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cucudq.cn/gtdisjprjj.html

TS:   arr.map(String)
来源：http://hz.smart0.xyz/gtaljlcmgy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jlsjyb.cn/gtfilmzodz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hammf.cn/gtbzqomwyc.html

Ruby: arr.map(&:upcase)
来源：http://hz.xuetiantiany.cn/gtfitnihtc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.52xcode.cn/gtawjbetza.html

[C08] 闭包
来源：http://hz.ywan-chungtsiang.top/gtihsiydrw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.mhx1999.top/gtkhiscvog.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cqqwz.cn/gtgdnmzzye.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtpfbiepss.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtnslkqnep.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yj20258.top/gtaqjmvpcs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jiagoushi.top/gtwgurhbfy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydzc1.top/gtkqlmuetp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtyqaxhnwh.html

[C09] 递归
来源：http://hz.quarkkingdee.top/gtldklzqpg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.c1oappe.top/gtlekpochv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.redwolf501.top/gtatcxnavw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuanzx.com/gtyrvvtvab.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.bjfxy.top/gtxfhicrxq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cqqwz.cn/gtvuspaksa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.aizwys.cn/gtqljwqcry.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.guowangkeji.top/gtlnfxbnmj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cashguo.top/gtrknpwcig.html

[C10] 变量作用域
来源：http://hz.snrcjt.cn/gtudocbrdr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yongpay.top/gtdppvxqpu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ehwqpu.com/gtgspxhgay.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sufxvd.cn/gtdbbgvmld.html

TS:   同 JS
来源：http://hz.cashguo.top/gtxciiebck.html

Java: 方法内为块级作用域
来源：http://hz.zhaomingkeji.xyz/gturxbhhba.html

Go:   花括号块级作用域
来源：http://hz.cucudq.cn/gtqgtrkxwq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sufxvd.cn/gtshfbqzcj.html

C#:   块级作用域
来源：http://hz.wangdashe.top/gtfdunxmgz.html

[C11] 模块导入与导出
来源：http://hz.xuetiantiany.cn/gtydhullsc.html

Py:   from module import func
来源：http://hz.zhijiandao.cn/gtmgcjwade.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhixingplan.top/gtpymhqssn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hywenlv.cn/gtzzivvede.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jyoumei.cn/gtkcpifuir.html

Java: import java.util.List;
来源：http://hz.pycfn.com/gtasjwlvtu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.svipenyu.cn/gtozcqdtad.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xinyue.icu/gtmsmmuevl.html

C#:   using System.Text;
来源：http://hz.gogol.net.cn/gtcgkxyyss.html

[C12] 立即执行函数 IIFE
来源：http://hz.aibaodan.cn/gtkiidlvdj.html

Py:   (lambda: print("run"))()
来源：http://hz.yvedp.cn/gtxlbvgina.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhixingplan.top/gtdpvkjdge.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuetiantiany.cn/gtjusznugz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gtndtuxktg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jianghu66.top/gtgdtlzxty.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.birdmap.top/gtrqtiggig.html

Ruby: -> { puts "run" }.call
来源：http://hz.svipenyu.cn/gtxynmfbhl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jyoumei.cn/gtvdamjpsi.html

[C13] 类型声明 / 类型注解
来源：http://hz.haohaochexian.top/gtrjouowub.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.fzhhl.top/gtnvvdhtvo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.havefunace.top/gtsctipunt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.wangdashe.top/gtosjeggqk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ybcxt.top/gtwtzuiipn.html


<!-- 参考信息 -->