代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://hz.jyoumei.cn/gtpllsixfl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zdqjudy.top/gtpwwdboep.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.kuanghao11.cn/gtgdyvirzp.html

[A25] 字符串比较
来源：http://hz.yongpay.top/gtymwcsjip.html

Py:   s1 == s2; s1 != s2
来源：http://hz.svipenyu.cn/gtinlpsfua.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ydjk.org.cn/gtaqyjykrg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yonumen.top/gteeisedlz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yueranfly.top/gtrfmzwxuz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yj20258888.top/gtcrjhjnwm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yuanzhike.top/gtlpzxmybg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.xuetiantiany.cn/gtvagjkqdb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.zhixingplan.top/gtojeunklj.html

[A26] 类型转换总览
来源：http://hz.nanxuanxn.top/gtnskcrosl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.ywan-chungtsiang.top/gtiltpytsb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.hysaishi.cn/gtkqkzhsxc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.sufxvd.cn/gtniqxwrjl.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zdqjudy.top/gtzbryzkyo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jyoumei.cn/gtsawliafc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.hfpthk.cn/gtuuyvkiiq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.aizwys.cn/gtnuboxfbr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.redwolf501.top/gtxeonnbpo.html

================================================================================
来源：http://hz.xylfe.cn/gtvfdorknn.html

B. 流程控制
来源：http://hz.havefunace.top/gtxqnxnlvg.html

================================================================================
来源：http://hz.haohaochexian.top/gtzvdkpobq.html

[B01] 条件判断 if / else
来源：http://hz.yj202588.top/gtrnhhcilb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cheryme.top/gtbblclcis.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.havefunace.top/gtigqiawyk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.chenjidiqi.icu/gtyeyqrllq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yangfankeji.com/gtsxldzxiz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yvedp.cn/gtzicaojlz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.cheryme.top/gtoaybagrx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.xingfuxueyuan.xyz/gtshtttjdl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.wangshuangyany.cn/gtbqaztbkj.html

[B02] 多分支 else if / elif
来源：http://hz.dianchejie.cn/gtxmegttoq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.nanxuanxn.top/gtjkohpgne.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.kuanghao11.cn/gtxeftcizx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xingfuxueyuan.xyz/gtlmqsdrmt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxinkj.top/gthfogqmsg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gogol.net.cn/gtxvxtsvio.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.kuanghao11.cn/gtsgvipcsa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhiwuduotai.top/gtnhgtqglq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.9152youxi.cn/gtxymgoopt.html

[B03] switch / match / case
来源：http://hz.ydjk.org.cn/gtgxhsexcp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yuxming.cn/gtjgeatfam.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.shanyushiyangtech.top/gtezaynxyx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhixingplan.top/gthbpqaolb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.smart0.xyz/gtqanuctrt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.redwolf501.top/gtcoobwawc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zycfv.cn/gtbdjiwobc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ybcxt.top/gthuakjttz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jqgfzy.top/gtkwiuxmyp.html

[B04] for 计数循环
来源：http://hz.shuidangran.top/gtuvldykiw.html

Py:   for i in range(10): print(i)
来源：http://hz.pengpengdd.cyou/gtcvrsrpsc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yj20258.top/gtsmohewgf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinqigufen.top/gtcbzjgifo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.guannengcc.top/gtvnzuemme.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.chenzaomai.com/gtfaprdeci.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.andypj.xyz/gtzjjdzmfg.html

Ruby: 10.times { |i| puts i }
来源：http://hz.redwolf501.top/gtlaamihbo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.snrcjt.cn/gtvcwiloux.html

[B05] 遍历数组 / 列表
来源：http://hz.hywenlv.cn/gtgtsokvlh.html

Py:   for item in arr: print(item)
来源：http://hz.shanyushiyangtech.top/gtmxrvfgdn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ivvv.top/gtkzzsltme.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.dashuyun.cn/gtujpgwazw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.ybcxt.top/gtqtvbuzaw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.pycfn.com/gtcpxghewt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.sxryk.cn/gtfyeiwekx.html

Ruby: arr.each { |item| puts item }
来源：http://hz.nanxinkj.top/gtqejraevh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.sxryk.cn/gtgommsavl.html

[B06] 遍历字典 / 对象
来源：http://hz.yonumen.top/gtonftwahy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.hywenlv.cn/gtlphroyjt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.zhixingplan.top/gtgdexgjvw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gotoacloud.top/gtluakxyoy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.quarkkingdee.top/gtfjuhamky.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.quarkkingdee.top/gtxcoingzo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jyoumei.cn/gtnkubsaxb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.sxryk.cn/gtonmminma.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.fengsongda.top/gturwvixso.html

[B07] while 循环
来源：http://hz.yanxiufei.cn/gtozesgizx.html

Py:   while i < 10: i += 1
来源：http://hz.jqgufenzy.top/gttouobmrg.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.redwolf501.top/gttldhxeiz.html

JS:   while (i < 10) { i++; }
来源：http://hz.hongshengwenyu.top/gtwdubbloz.html

TS:   while (i < 10) { i++; }
来源：http://hz.hammf.cn/gtgocqknbk.html

Java: while (i < 10) { i++; }
来源：http://hz.yangfankeji.com/gtsxbsjlyd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhoulong.xyz/gtgmollqrg.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jinyuanbaomall.cn/gtgsqfdsco.html

C#:   while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gtqxuzsbkp.html

[B08] do-while（至少执行一次）
来源：http://hz.yangfankeji.com/gtlvcrlblh.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.pycfn.com/gtoombjmwu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.wangshuangyany.cn/gtwdqyhreh.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xinyue.icu/gtxfrsxjyz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.fzhhl.top/gtrssmgbhs.html

Java: do { i++; } while (i < 10);
来源：http://hz.shanyushiyangkeji.top/gtzhodnqck.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhongyouzk.top/gtemtkdsjl.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cdnleiting.top/gtoxulodih.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gtpgnifwrz.html

[B09] break 与 continue
来源：http://hz.feifeiyinyue.top/gtuemktqkj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.daria6918.cn/gtnpnucnfw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtawpajyfi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtdmshkhrw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gtstbwjawe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtbznoacoa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.fzhhl.top/gtmzzlzfkq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jqgfzy.top/gtpdsyuque.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zdqjudy.top/gtdlwbkcbb.html

[B10] 遍历同时拿索引
来源：http://hz.ppjwa.cn/gtalhdnhvf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yongpay.top/gtmwbmzajy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.dashuyun.cn/gtekmdebpb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.cdnleiting.top/gtuqvitgwo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jinghuilouyu.cn/gtjjfqtslb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.andypj.xyz/gthaaarfvv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yueranfly.top/gtukzhfugg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hysaishi.cn/gtvvvkxxif.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ivvv.top/gttctrmedx.html

[B11] 生成数字序列 / 区间
来源：http://hz.tianlin.xyz/gtzqqravla.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhixingplan.top/gtjefmynet.html

PHP:  range(0, 10, 2);
来源：http://hz.9152youxi.cn/gtkinvwrxb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dashuyun.cn/gtfoxdcrvk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gtnnpanphh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yangfankeji.com/gtkmzwmxxw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.chenzaomai.com/gtzlxxfolu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.smart0.xyz/gtffmrujsh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.daxiang520.top/gtrtqpujoc.html

[B12] 跳出多层循环
来源：http://hz.jianghu66.top/gtdncywmwz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sxryk.cn/gtcxfjfqhc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.daria6918.cn/gtantaonxa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhongyouzk.top/gtjipbfput.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gaohongyu789.top/gthdthblqd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gthlefktsz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.havefunace.top/gtafbapezc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.quarkkingdee.top/gtcyicfkst.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.iojbl.cn/gtlpzcggyt.html

[B13] 判断是否为数字
来源：http://hz.c1oappe.top/gtezufqefk.html

Py:   isinstance(x, (int, float))
来源：http://hz.havefunace.top/gttohicxqu.html

PHP:  is_numeric($x)
来源：http://hz.shuidangran.top/gtbjksoznh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinqigfzy.top/gtsbocjvzl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jyoumei.cn/gtdajbadcb.html

Java: x instanceof Number
来源：http://hz.yanxiufei.cn/gtpjckdrma.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hywenlv.cn/gtlidxhzub.html

Ruby: x.is_a?(Numeric)
来源：http://hz.snrcjt.cn/gttmkkielu.html

C#:   x is int or double or decimal
来源：http://hz.zhongyouzk.top/gtihsibzyc.html

[B14] 判断值是否在集合内
来源：http://hz.yuxming.cn/gtlrqeghof.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zycfv.cn/gtertknfxh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhongyouzk.top/gtbduvfmmt.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ivvv.top/gtmjddytgi.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hammf.cn/gtiwrkfrhr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.svipenyu.cn/gtugytbmaf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nanxuanxn.top/gteeggdubn.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.316326.xyz/gttvzgzyyq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtpanwndci.html

[B15] 布尔运算与取反
来源：http://hz.zhengqikj.top/gtozvfpxjn.html

Py:   a and b or not c
来源：http://hz.mhx1999.top/gtugnvxldr.html

PHP:  $a && $b || !$c
来源：http://hz.wangshuangyany.cn/gtaffxrrbl.html

JS:   a && b || !c
来源：http://hz.cqqwz.cn/gtdaqlkowj.html

TS:   a && b || !c
来源：http://hz.yanxiufei.cn/gtuusopgbz.html

Java: a && b || !c
来源：http://hz.jinqigufen.top/gtagankpyl.html

Go:   a && b || !c
来源：http://hz.cqqwz.cn/gtwfztqikb.html

Ruby: a && b || !c
来源：http://hz.jqgfzy.top/gtlcqrtgyo.html

C#:   a && b || !c
来源：http://hz.yueranfly.top/gtikmwfdwl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shuidangran.top/gtpnfirdss.html

Py:   if not data: return
来源：http://hz.shanyushiyangtech.top/gtzjiqcfku.html

PHP:  if (!$data) { return; }
来源：http://hz.hfpthk.cn/gtohzzzyko.html

JS:   if (!data) return;
来源：http://hz.wangdashe.top/gtciukbfpz.html

TS:   if (!data) return;
来源：http://hz.wangdashe.top/gtutnglkez.html

Java: if (data == null) return;
来源：http://hz.hywenlv.cn/gtrcwhgqpl.html

Go:   if data == nil { return }
来源：http://hz.jiagoushi.top/gtoswxtvqv.html

Ruby: return if data.nil?
来源：http://hz.yuxming.cn/gtbjndcdtz.html

C#:   if (data == null) return;
来源：http://hz.xuetiantiany.cn/gtnuhsvpsr.html

================================================================================
来源：http://hz.cheryme.top/gtiyalhazc.html

C. 函数与作用域
来源：http://hz.wangshuangyany.cn/gtdjirrlnk.html

================================================================================
来源：http://hz.zycfv.cn/gtcqmjakzj.html

[C01] 定义函数
来源：http://hz.316326.xyz/gtvkktvgke.html

Py:   def add(a, b): return a + b
来源：http://hz.jinyuanbaomall.cn/gtizftbibe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yanxiufei.cn/gtgzrbapnx.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtygqfbryx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sxryk.cn/gtmphgxvqd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtfjdsvwgz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhongyouzk.top/gtmwwggzfd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gogol.net.cn/gtysvxyoko.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.9152youxi.cn/gtgblvokhy.html

[C02] 默认参数
来源：http://hz.jinghuilouyu.cn/gtmjbvegwu.html

Py:   def greet(name="World"): return name
来源：http://hz.dashuyun.cn/gtcjrsvqzz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.andypj.xyz/gtppqgpyvt.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenlongwang.top/gtnqqyxznd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gotoacloud.top/gtibmknyqb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.aizwys.cn/gtcalggsdw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.316326.xyz/gtljzjnqbg.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhaomingkeji.xyz/gtgyvdjxlh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xinyue.icu/gtrsgnuxco.html

[C03] 可变参数
来源：http://hz.zhixingplan.top/gtlvixlkrv.html

Py:   def total(*args): return sum(args)
来源：http://hz.havefunace.top/gtbtxtfpch.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.tanke756.top/gttixqoyeg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhiwuduotai.top/gtdjevoyfe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.havefunace.top/gtiymkxzwu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.kuanghao11.cn/gtcwogufqu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.c1oappe.top/gtqpyvszsr.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hnqzz.top/gtxxslpwnx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yongpay.top/gticlpycfe.html

[C04] 命名参数 / 关键字参数
来源：http://hz.mhx1999.top/gtswpswbnz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.birdmap.top/gtfytbsipa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gogol.net.cn/gttragdjrm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shzxlz.cn/gtekcomnuf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ppjwa.cn/gtdvkfakzg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shangyingyoupin.top/gtqwpghoee.html

Go:   // 无：用配置结构体参数
来源：http://hz.jianghu66.top/gtxvznyncw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtjjpbhlqp.html

C#:   f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gtkzqspugb.html

[C05] 返回多个值
来源：http://hz.jqgufenzy.top/gtwxjiolvc.html

Py:   return a, b
来源：http://hz.tanke756.top/gtgazolfex.html

PHP:  return [$a, $b];
来源：http://hz.sxryk.cn/gtwfrzccuw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hammf.cn/gttwtryrsj.html

TS:   return { a, b };
来源：http://hz.mhx1999.top/gtwxdlywpi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.dashuyun.cn/gtyszvwuoy.html

Go:   return a, b
来源：http://hz.yonumen.top/gtasxvltsn.html

Ruby: return a, b
来源：http://hz.gotoacloud.top/gtgibgomoj.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.chenlongwang.top/gtwwhvpozq.html

[C06] 匿名函数 / lambda
来源：http://hz.yonumen.top/gtyfnqvemu.html

Py:   square = lambda x: x * x
来源：http://hz.iojbl.cn/gtdvjajrpr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.dashuyun.cn/gtrcomtwjy.html

JS:   const square = x => x * x;
来源：http://hz.chenzaomai.com/gtieiisfgw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shzxlz.cn/gtwwyhkvvz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinghuilouyu.cn/gtergayaix.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinqigufen.top/gtvapywoea.html

Ruby: square = ->(x) { x * x }
来源：http://hz.andypj.xyz/gtmyutrnkd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhongyouzk.top/gtezfrnkgc.html

[C07] 把函数作为参数传入
来源：http://hz.jlsjyb.cn/gtlvqltnfc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.meibo888.top/gtdmuferip.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jlsjyb.cn/gtpmdcohdi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sweek.top/gtmezvcyss.html

TS:   arr.map(String)
来源：http://hz.hnxiangtu.top/gtxqsrkrjm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gaohongyu789.top/gtuzorzptc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenzaomai.com/gtikkvrxzk.html

Ruby: arr.map(&:upcase)
来源：http://hz.sweek.top/gtjedfgscj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yueranfly.top/gtkdjpxzsi.html

[C08] 闭包
来源：http://hz.0kj1m.cn/gtuhjciega.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.fzhhl.top/gtfhpowwif.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jqgfzy.top/gtyheovrht.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.daxiang520.top/gtfhidmkdp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtvvfwelzt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.52xcode.cn/gtuytwbxml.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.9152youxi.cn/gtlcongxid.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cucudq.cn/gtmdrpzzfn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhaomingkeji.xyz/gtatympyiz.html

[C09] 递归
来源：http://hz.fengsongda.top/gtzwpsrvwh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.tanke756.top/gtlebhsknv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.316326.xyz/gtcsihtzgi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yangfankeji.com/gtpcovdoaz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hfpthk.cn/gtjawqdtni.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jlsjyb.cn/gtuibkkseb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ydjk.org.cn/gtmlhmpdif.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhixingplan.top/gtbzkgcgsp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenjidiqi.icu/gtpjryekgh.html

[C10] 变量作用域
来源：http://hz.sysykeji.top/gtxjbrpfqj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shuidangran.top/gtytwfslap.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.svipenyu.cn/gtfchcanne.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cheryme.top/gtxgmeqnqh.html

TS:   同 JS
来源：http://hz.zhiwuduotai.top/gtmkwjvrbs.html

Java: 方法内为块级作用域
来源：http://hz.jlsjyb.cn/gtobmjeeuf.html

Go:   花括号块级作用域
来源：http://hz.haohaochexian.top/gtpmyvlhng.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.mhx1999.top/gteqjnpfvs.html

C#:   块级作用域
来源：http://hz.dashuyun.cn/gtgtqddjht.html

[C11] 模块导入与导出
来源：http://hz.sysykeji.top/gtyibyimrx.html

Py:   from module import func
来源：http://hz.zhixingplan.top/gtbbtbopcy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.andypj.xyz/gtagwzndcw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tanke756.top/gtqntspzti.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.daria6918.cn/gtolqhicix.html

Java: import java.util.List;
来源：http://hz.aibaodan.cn/gtiapmibto.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.svipenyu.cn/gtxczrbtau.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hnqzz.top/gtseyaqeub.html

C#:   using System.Text;
来源：http://hz.zhiwuduotai.top/gtahiefdun.html

[C12] 立即执行函数 IIFE
来源：http://hz.c1oappe.top/gtzklswzhj.html

Py:   (lambda: print("run"))()
来源：http://hz.quarkkingdee.top/gtxjiftdfy.html

PHP:  (function () { echo "run"; })();
来源：http://hz.svipenyu.cn/gtpvpilqkb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gttoxvkidf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtmbjermof.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.wangdashe.top/gtfmyckfja.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.svipenyu.cn/gtynxafrnn.html

Ruby: -> { puts "run" }.call
来源：http://hz.gzhubu.top/gtfzzyahxu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hfpthk.cn/gthapinvrv.html

[C13] 类型声明 / 类型注解
来源：http://hz.ydzc1.top/gtcrhqhquy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aizwys.cn/gtkrvocyyi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtblzhpdxy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xingfuxueyuan.xyz/gtlqqcuzsn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yvedp.cn/gtpawwamfy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtibetvqbe.html

Go:   func add(a, b int) int
来源：http://hz.9152youxi.cn/gtaqywvpvk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnqzz.top/gtmwxvhqug.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ydjk.org.cn/gtcjufxzll.html

[C14] 泛型函数
来源：http://hz.yuanzhike.top/gtdbuzvpxu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhaomingkeji.xyz/gtuokpqqek.html

PHP:  // 无泛型
来源：http://hz.cashguo.top/gtizllwzds.html

JS:   // 无泛型
来源：http://hz.dashuyun.cn/gtbucafiru.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xingfuxueyuan.xyz/gtwrznskbw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sxryk.cn/gtrfcrpdct.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.316326.xyz/gtbxiafilm.html

Ruby: # 无泛型
来源：http://hz.birdmap.top/gtiubleduh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.nanxuanxn.top/gtukbmwozj.html

[C15] 解构 / 展开参数
来源：http://hz.chenjidiqi.icu/gtjvtqkbsv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.52xcode.cn/gtymyntcwl.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jyoumei.cn/gtdlhssnti.html


<!-- 参考信息 -->