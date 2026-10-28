代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.chenlongwang.top/gtolsqumch.html

Ruby: gets.chomp
来源：http://hz.c1oappe.top/gtfstqddhn.html

C#:   Console.ReadLine();
来源：http://hz.hongshengwenyu.top/gtheyzppxr.html

[A21] 保留指定小数位输出
来源：http://hz.xinyue.icu/gtkjblxgmw.html

Py:   f"{3.14159:.2f}"
来源：http://hz.ivvv.top/gtaqmnwoby.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.zhengqikj.top/gtzljamkhv.html

JS:   (3.14159).toFixed(2)
来源：http://hz.jinghuilouyu.cn/gtuzzytqac.html

TS:   (3.14159).toFixed(2)
来源：http://hz.gzhubu.top/gtmrbjsijr.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.hysaishi.cn/gtffsbfyxz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.yonumen.top/gtelspuykh.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.zhongyouzk.top/gtbcfztixv.html

C#:   3.14159.ToString("F2")
来源：http://hz.havefunace.top/gtuvzusbwv.html

[A22] 获取字符串长度
来源：http://hz.zhoulong.xyz/gtsimqleec.html

Py:   len(s)
来源：http://hz.jinghuilouyu.cn/gtsglnizag.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.guowangkeji.top/gtmogyvcvw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.daria6918.cn/gtvfaesjtu.html

TS:   s.length
来源：http://hz.tanke756.top/gtbfqzxtqi.html

Java: s.length()
来源：http://hz.yongpay.top/gtddcawbda.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yuanzhike.top/gtpsmyydqo.html

Ruby: s.length
来源：http://hz.aizwys.cn/gtakmmgkry.html

C#:   s.Length
来源：http://hz.smart0.xyz/gtlndwfpjx.html

[A23] 大小写转换
来源：http://hz.jlsjyb.cn/gtrdiylehy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.sweek.top/gthelolaem.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.tianlin.xyz/gtihnekkdj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.gotoacloud.top/gtxhtbruuf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cqqwz.cn/gtlirdxchz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yuanzhike.top/gteuvmhilo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.daria6918.cn/gtkvioewis.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.dianchejie.cn/gtxenhqpyw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.gogol.net.cn/gtmxmwuqed.html

[A24] 去除首尾空白
来源：http://hz.zdqjudy.top/gtnwpwgarx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.fengsongda.top/gtrcqnrtuv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.316326.xyz/gthgfleymc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hongshengwenyu.top/gtqjcaurjw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yvedp.cn/gtfkpmpvhf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jinghuilouyu.cn/gtyseyeton.html

Go:   strings.TrimSpace(s)
来源：http://hz.zycfv.cn/gtjjswwcyy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.xinyue.icu/gtmqjdghjg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.andypj.xyz/gtdoshrkmn.html

[A25] 字符串比较
来源：http://hz.sxryk.cn/gtwfwpsbjk.html

Py:   s1 == s2; s1 != s2
来源：http://hz.xylfe.cn/gtbyukiltd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.sufxvd.cn/gtlszzndbz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.52xcode.cn/gtucbkmnob.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.aizwys.cn/gtqiyqtxpo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.birdmap.top/gtqyfyuenl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ydjk.org.cn/gtgpouxqdk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hammf.cn/gttvjcfvbo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.svipenyu.cn/gtnbhxbqhz.html

[A26] 类型转换总览
来源：http://hz.xuetiantiany.cn/gtqpmcrowb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.mhx1999.top/gtcguhtrhe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.shangyingyoupin.top/gtkgguudld.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hnxiangtu.top/gtsinlmrxa.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zycfv.cn/gttbbltupi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.tanke756.top/gtjssjlxzb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.ybcxt.top/gtencasnoe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.ppjwa.cn/gtunzmbfud.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yj20258.top/gtxyytqaqm.html

================================================================================
来源：http://hz.zhengqikj.top/gtujowzhmv.html

B. 流程控制
来源：http://hz.jinghuilouyu.cn/gtuhvredan.html

================================================================================
来源：http://hz.gotoacloud.top/gtrrknmlqc.html

[B01] 条件判断 if / else
来源：http://hz.guannengcc.top/gtqfnyuyeq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.hongshengwenyu.top/gtxdqyzugt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.sufxvd.cn/gthnufmvhz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shuidangran.top/gtsqlyrphy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zycfv.cn/gtefvvuymi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.bjfxy.top/gtebgmqefy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhongyouzk.top/gtkwwqlcrw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zycfv.cn/gtbthqareg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.tian-w.cn/gthmuraioh.html

[B02] 多分支 else if / elif
来源：http://hz.shzxlz.cn/gthvxhlbsp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.316326.xyz/gtsrwzqfkv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.tian-w.cn/gtqkspzsyx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cucudq.cn/gtlbxhtdms.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guannengcc.top/gtbrnrgjjl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.smart0.xyz/gtapgytgxm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.tanke756.top/gthnqlhucw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.shangyingyoupin.top/gtswnnjlrz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.52xcode.cn/gtzwvoeces.html

[B03] switch / match / case
来源：http://hz.cqqwz.cn/gtefczvdll.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.tanke756.top/gtvbzleamw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yj20258888.top/gtnoksetsz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenzaomai.com/gtmdeoadcm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.316326.xyz/gttnehstff.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.aibaodan.cn/gtxxihmmih.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.bjfxy.top/gtcuchtldj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.52xcode.cn/gttlygztwi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.aizwys.cn/gtvwrrozdt.html

[B04] for 计数循环
来源：http://hz.yuxming.cn/gtoxlhpbvu.html

Py:   for i in range(10): print(i)
来源：http://hz.hfpthk.cn/gtajdkawte.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shzxlz.cn/gtdxyjhnuu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.vqdsnc.cn/gtsxqmqhww.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ydjk.org.cn/gtulggagoe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.feifeiyinyue.top/gtqahfvsyi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.0kj1m.cn/gtptggpizz.html

Ruby: 10.times { |i| puts i }
来源：http://hz.xuanzx.com/gtkbunoies.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xingfuxueyuan.xyz/gtgszhpeee.html

[B05] 遍历数组 / 列表
来源：http://hz.redwolf501.top/gtkqnttecp.html

Py:   for item in arr: print(item)
来源：http://hz.jinyuanbaomall.cn/gttuimpudh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.nanxinkj.top/gtmejiunew.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj202588.top/gtquffqiyz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xuetiantiany.cn/gtgremnnmq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.c1oappe.top/gtqmqzwzaz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yj20258.top/gtmeakwkrm.html

Ruby: arr.each { |item| puts item }
来源：http://hz.guannengcc.top/gtgpgarwey.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.gogol.net.cn/gtdawjwpff.html

[B06] 遍历字典 / 对象
来源：http://hz.daria6918.cn/gtlhdbokej.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.nwbrower.top/gtatdhxgua.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.dianchejie.cn/gtkxanmwzo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ywan-chungtsiang.top/gtnsrwmdna.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zdqjudy.top/gtuwoykvdj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cqqwz.cn/gtjlskwgxf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.aibaodan.cn/gtwqfzfwwu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.9152youxi.cn/gtddydiaon.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.cheryme.top/gtpdxayuxj.html

[B07] while 循环
来源：http://hz.ydzc1.top/gtbdjlqdgv.html

Py:   while i < 10: i += 1
来源：http://hz.yonumen.top/gttseoavob.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.redwolf501.top/gttsvmkexl.html

JS:   while (i < 10) { i++; }
来源：http://hz.nanxinkj.top/gtaivqovyz.html

TS:   while (i < 10) { i++; }
来源：http://hz.xingfuxueyuan.xyz/gtujzjpnua.html

Java: while (i < 10) { i++; }
来源：http://hz.pengpengdd.cyou/gtkuvgmohj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.kuanghao11.cn/gtaklxhrxq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhijiandao.cn/gtxfwlmchg.html

C#:   while (i < 10) { i++; }
来源：http://hz.ydjk.org.cn/gtopxkeyql.html

[B08] do-while（至少执行一次）
来源：http://hz.haohaochexian.top/gtjjkeeffu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xuanzx.com/gtkctwzckl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.smart0.xyz/gtmpwoiinf.html

JS:   do { i++; } while (i < 10);
来源：http://hz.redwolf501.top/gtsjyabsfc.html

TS:   do { i++; } while (i < 10);
来源：http://hz.iojbl.cn/gtwmevpbno.html

Java: do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gtwhhzzldc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hysaishi.cn/gthcdbbecc.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xingfuxueyuan.xyz/gtbqvrwxpf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.c1oappe.top/gtxlmgjiyp.html

[B09] break 与 continue
来源：http://hz.daria6918.cn/gtjaahdmct.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yonumen.top/gtrekfyfvn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yj20258888.top/gtjeocqxby.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yonumen.top/gtlgvxxobc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gtinlzfbgd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtrozwmhem.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.haohaochexian.top/gtfpclcvyg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.sufxvd.cn/gtqnzuwtng.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yueranfly.top/gtkteilgyv.html

[B10] 遍历同时拿索引
来源：http://hz.zhijiandao.cn/gtjlxrocmc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gaohongyu789.top/gtfzcptdfd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ywan-chungtsiang.top/gtmcswwcoq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.birdmap.top/gtphsxfnpw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.chenlongwang.top/gtdffhrked.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.guannengcc.top/gtgalsnxgl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yonumen.top/gtheemuvyc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ywan-chungtsiang.top/gtblzqzmsj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhixingplan.top/gtdxjcerea.html

[B11] 生成数字序列 / 区间
来源：http://hz.ppjwa.cn/gtmwxotrsq.html

Py:   list(range(0, 10, 2))
来源：http://hz.aibaodan.cn/gtebxmoikn.html

PHP:  range(0, 10, 2);
来源：http://hz.havefunace.top/gtytbpoycq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.quarkkingdee.top/gtrkvlnhkp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fengsongda.top/gtikerspin.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.dashuyun.cn/gtzhjkfgme.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.aizwys.cn/gtpyapwndr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ivvv.top/gtgvnjwiwt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ywan-chungtsiang.top/gtytrepibi.html

[B12] 跳出多层循环
来源：http://hz.sxryk.cn/gtacamksim.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ehwqpu.com/gtsqsetaay.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.pengpengdd.cyou/gtfcypfovn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gtsdcynbeg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtnbfreinn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.tianlin.xyz/gtbgzxcruq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhaomingkeji.xyz/gtkbbuihjd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gotoacloud.top/gtdiwbyrmq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cqqwz.cn/gttukmybmo.html

[B13] 判断是否为数字
来源：http://hz.pycfn.com/gtvjjfqxpz.html

Py:   isinstance(x, (int, float))
来源：http://hz.xinyue.icu/gthamifvuy.html

PHP:  is_numeric($x)
来源：http://hz.jqgfzy.top/gtytmtgnec.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sxryk.cn/gtqbegyxyx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shzxlz.cn/gtximcqtuw.html

Java: x instanceof Number
来源：http://hz.mhx1999.top/gtbxeaiado.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hongshengwenyu.top/gtoqxkmxbt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hywenlv.cn/gtcyytkjnk.html

C#:   x is int or double or decimal
来源：http://hz.guowangkeji.top/gtdjdtrtda.html

[B14] 判断值是否在集合内
来源：http://hz.gogol.net.cn/gtzmcwxmot.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gaohongyu789.top/gtfjhlllrb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.daxiang520.top/gtcjtedouw.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cheryme.top/gtenfjunoj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.aibaodan.cn/gtnkgwaoyd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.dashuyun.cn/gtrujyefhj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenzaomai.com/gtqzgrafsp.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sysykeji.top/gtskanmfmb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtdvzehlzu.html

[B15] 布尔运算与取反
来源：http://hz.chenjidiqi.icu/gtvcrwxedi.html

Py:   a and b or not c
来源：http://hz.sysykeji.top/gtojvyjjil.html

PHP:  $a && $b || !$c
来源：http://hz.cashguo.top/gtzetqwawu.html

JS:   a && b || !c
来源：http://hz.zhijiandao.cn/gtbkvpzoue.html

TS:   a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtmilukxps.html

Java: a && b || !c
来源：http://hz.guowangkeji.top/gthisslbgq.html

Go:   a && b || !c
来源：http://hz.yangfankeji.com/gtwptarlkt.html

Ruby: a && b || !c
来源：http://hz.kuanghao11.cn/gtjnmdhunb.html

C#:   a && b || !c
来源：http://hz.cashguo.top/gtwixhqbnk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.gaohongyu789.top/gttklvatmn.html

Py:   if not data: return
来源：http://hz.ydjk.org.cn/gtujxycmus.html

PHP:  if (!$data) { return; }
来源：http://hz.xuetiantiany.cn/gtkmyewidc.html

JS:   if (!data) return;
来源：http://hz.kuanghao11.cn/gtytszvihb.html

TS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtbihuxmcl.html

Java: if (data == null) return;
来源：http://hz.jinyuanbaomall.cn/gtmxdfucvp.html

Go:   if data == nil { return }
来源：http://hz.dianchejie.cn/gtvehisgdo.html

Ruby: return if data.nil?
来源：http://hz.gzhubu.top/gttdpkdowz.html

C#:   if (data == null) return;
来源：http://hz.gogol.net.cn/gtloownbfk.html

================================================================================
来源：http://hz.sxryk.cn/gtooghkzlc.html

C. 函数与作用域
来源：http://hz.yangfankeji.com/gtjnzczkjc.html

================================================================================
来源：http://hz.gaohongyu789.top/gtimxhngwp.html

[C01] 定义函数
来源：http://hz.jinqigfzy.top/gttzsomtdd.html

Py:   def add(a, b): return a + b
来源：http://hz.wangdashe.top/gtdaybozyd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtpkcclfux.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hywenlv.cn/gtpwyourfc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jlsjyb.cn/gtkszormhe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.chenlongwang.top/gtfoomqpkk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sysykeji.top/gtxwqewwbr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hammf.cn/gtjhrignge.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtculkwvts.html

[C02] 默认参数
来源：http://hz.aizwys.cn/gtxgdkqwtg.html

Py:   def greet(name="World"): return name
来源：http://hz.daria6918.cn/gtplupbcpk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yj20258.top/gthjmsypik.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.sufxvd.cn/gtiuiuamkg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinyuanbaomall.cn/gtjnktsudx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.aibaodan.cn/gtxbhbidla.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jlsjyb.cn/gtxljdvgnt.html

Ruby: def greet(name = "World") = name
来源：http://hz.yangfankeji.com/gtnrhvfclh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenlongwang.top/gtchduvlqq.html

[C03] 可变参数
来源：http://hz.zhijiandao.cn/gtmwlqanbg.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhengqikj.top/gtgjprovgp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.feifeiyinyue.top/gtkkhjjnkv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tian-w.cn/gtdiyaxmit.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.iojbl.cn/gtozevdbby.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shzxlz.cn/gtvxzkusyz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.316326.xyz/gtsdxwdyqz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yueranfly.top/gtzlsenjco.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinqigfzy.top/gtlwmcvqzg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ydzc1.top/gtsnufkvtn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.fengsongda.top/gtasgrcurx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.9152youxi.cn/gtjqzkbmrk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xziqi.cn/gtzbiwsevt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.wangdashe.top/gtizudbhii.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hfpthk.cn/gtjapweaef.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhijiandao.cn/gtcahixslg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenjidiqi.icu/gtlcsgcfdy.html

C#:   f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtsjhhedgr.html

[C05] 返回多个值
来源：http://hz.xuanzx.com/gtimmyyxmj.html

Py:   return a, b
来源：http://hz.cucudq.cn/gtvbuytvmj.html

PHP:  return [$a, $b];
来源：http://hz.pycfn.com/gtnurazcgz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cdnleiting.top/gtdayshckw.html

TS:   return { a, b };
来源：http://hz.hywenlv.cn/gtaletuaji.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nwbrower.top/gtuyzjmjsw.html

Go:   return a, b
来源：http://hz.iojbl.cn/gtmpdagkjf.html

Ruby: return a, b
来源：http://hz.haohaochexian.top/gtfvhisddm.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnxiangtu.top/gtebizogeo.html

[C06] 匿名函数 / lambda
来源：http://hz.jqgufenzy.top/gtrnkslpni.html

Py:   square = lambda x: x * x
来源：http://hz.jinqigufen.top/gtyeolrmrz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.nanxuanxn.top/gtbsrrvlfk.html

JS:   const square = x => x * x;
来源：http://hz.cdnleiting.top/gtnesdgmwb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenlongwang.top/gtpjrotzgd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.svipenyu.cn/gtibyympeo.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gaohongyu789.top/gtqzldsvwn.html

Ruby: square = ->(x) { x * x }
来源：http://hz.havefunace.top/gtwwhlzpno.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ywan-chungtsiang.top/gtdtmmkvck.html

[C07] 把函数作为参数传入
来源：http://hz.gaohongyu789.top/gtubuzefyc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.quarkkingdee.top/gtspojhjql.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nanxinkj.top/gtcugpvcpl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.chenzaomai.com/gtopjkfznp.html

TS:   arr.map(String)
来源：http://hz.sxryk.cn/gtaydzjgyl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yongpay.top/gtwocubbfp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhoulong.xyz/gtukduzcib.html

Ruby: arr.map(&:upcase)
来源：http://hz.bjfxy.top/gtungqufxz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shzxlz.cn/gtbwgzdzzw.html

[C08] 闭包
来源：http://hz.yuanzhike.top/gtbqpxofrg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.daxiang520.top/gtmezuxews.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cashguo.top/gtmeaudkhr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.sysykeji.top/gtyiynvywb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtnxwjloha.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yongpay.top/gtddgramnb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.pycfn.com/gtrxfxulbb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.kuanghao11.cn/gthxslapsn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtuckfgree.html

[C09] 递归
来源：http://hz.9152youxi.cn/gtfoniglda.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.guannengcc.top/gtaqtgnbrx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.smart0.xyz/gtwmyvfwvv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gtdswejfda.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tanke756.top/gtlkzdgeyy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenjidiqi.icu/gtrcluyabw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yongpay.top/gtvavzemdd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ivvv.top/gttngwtbid.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigufen.top/gthcpuvvxk.html

[C10] 变量作用域
来源：http://hz.chenjidiqi.icu/gtkzhbclaq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shanyushiyangkeji.top/gtrosrhzxk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yongpay.top/gtsolesaqm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.daria6918.cn/gtyzpjeqwe.html

TS:   同 JS
来源：http://hz.kuanghao11.cn/gtfazsnkdm.html

Java: 方法内为块级作用域
来源：http://hz.birdmap.top/gtxivuixuu.html

Go:   花括号块级作用域
来源：http://hz.fzhhl.top/gtidrjmoth.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cucudq.cn/gtdqvbdjuz.html

C#:   块级作用域
来源：http://hz.tian-w.cn/gtejlzopht.html

[C11] 模块导入与导出
来源：http://hz.dianchejie.cn/gtsqznbqsm.html

Py:   from module import func
来源：http://hz.yanxiufei.cn/gtnqdsejmt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nanxinkj.top/gtcuhnrpxv.html


<!-- 参考信息 -->