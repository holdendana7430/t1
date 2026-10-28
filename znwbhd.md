代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.gogol.net.cn/gtpkhmhlqh.html

Ruby: gets.chomp
来源：http://hz.mhx1999.top/gtlvidvwok.html

C#:   Console.ReadLine();
来源：http://hz.cashguo.top/gtlhylmmqk.html

[A21] 保留指定小数位输出
来源：http://hz.hfpthk.cn/gtcrbzlhce.html

Py:   f"{3.14159:.2f}"
来源：http://hz.cashguo.top/gtodsfywbv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.bjfxy.top/gtesljxggw.html

JS:   (3.14159).toFixed(2)
来源：http://hz.hongshengwenyu.top/gtnoobtmvd.html

TS:   (3.14159).toFixed(2)
来源：http://hz.shzxlz.cn/gtpjmrbbyr.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.mhx1999.top/gtdyllrizk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jinqigfzy.top/gterwbfjsm.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.ehwqpu.com/gtuajcrysi.html

C#:   3.14159.ToString("F2")
来源：http://hz.sysykeji.top/gtxpocjcvh.html

[A22] 获取字符串长度
来源：http://hz.sxryk.cn/gtnwfjojaj.html

Py:   len(s)
来源：http://hz.zycfv.cn/gtgzidbxif.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.hysaishi.cn/gtsnbzmnre.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.shangyingyoupin.top/gtdbjjyxzs.html

TS:   s.length
来源：http://hz.zhoulong.xyz/gtxxaidlfn.html

Java: s.length()
来源：http://hz.feifeiyinyue.top/gtkqqplgal.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.shangyingyoupin.top/gtxbwnjvdb.html

Ruby: s.length
来源：http://hz.fzhhl.top/gtpjdzwycz.html

C#:   s.Length
来源：http://hz.wangshuangyany.cn/gtokdnyshj.html

[A23] 大小写转换
来源：http://hz.hnxiangtu.top/gtvrccobko.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.gaohongyu789.top/gtfwflzpix.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.nanxuanxn.top/gtabpnuhoy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yonumen.top/gthuqvicnt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hongshengwenyu.top/gtehklcvqn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.birdmap.top/gtaozwffrv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yonumen.top/gtneiljpuh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.snrcjt.cn/gtinozjfav.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.zhaomingkeji.xyz/gtwazgratm.html

[A24] 去除首尾空白
来源：http://hz.zhiwuduotai.top/gtzzkycdxo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yanxiufei.cn/gtuyhcancm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.xinyue.icu/gtgnmhekfl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.smart0.xyz/gtszwzdriw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ydjk.org.cn/gtazzcaged.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.smart0.xyz/gtdyzidfwn.html

Go:   strings.TrimSpace(s)
来源：http://hz.pengpengdd.cyou/gtmndaasjc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yuanzhike.top/gtpieixjbf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.jqgufenzy.top/gtetweibja.html

[A25] 字符串比较
来源：http://hz.feifeiyinyue.top/gtymkzdtes.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ppjwa.cn/gtjamkouaz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.xuetiantiany.cn/gtjzbseovq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.andypj.xyz/gtwgveethi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yj20258888.top/gtqfqofeku.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.wangdashe.top/gtbebsqryc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.c1oappe.top/gtfrlwwtil.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ywan-chungtsiang.top/gtbidaxork.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.sweek.top/gtidtujqca.html

[A26] 类型转换总览
来源：http://hz.gotoacloud.top/gtvcbaplcm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.chenzaomai.com/gtfcbbpaqo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.ywan-chungtsiang.top/gtzbsbeuwv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.pengpengdd.cyou/gtyvjjnazo.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jyoumei.cn/gthfxrvvww.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhengqikj.top/gtketnivyz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yonumen.top/gtuzsmqolj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.0kj1m.cn/gtpvixmxvh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.haohaochexian.top/gtdqxcjwid.html

================================================================================
来源：http://hz.hfpthk.cn/gtfqnxatgz.html

B. 流程控制
来源：http://hz.ehwqpu.com/gtmjgtpveh.html

================================================================================
来源：http://hz.fzhhl.top/gthcdmssxf.html

[B01] 条件判断 if / else
来源：http://hz.yanxiufei.cn/gtcgoctfzb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.xylfe.cn/gtynbkidqi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.wangshuangyany.cn/gtoztvzqqd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hnxiangtu.top/gtkqoheppq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.kuanghao11.cn/gtobrnaotf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yj202588.top/gtzxbfujcn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.shangyingyoupin.top/gttwvpbeoe.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.cqqwz.cn/gtfktnrdws.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.sysykeji.top/gtygebubuc.html

[B02] 多分支 else if / elif
来源：http://hz.feifeiyinyue.top/gtnvkgxcmf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.gogol.net.cn/gtliqdfvcu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.tanke756.top/gtffhspooq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhengqikj.top/gthokzhqjo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tanke756.top/gttpyjpnup.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtkdxkrtcs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jqgfzy.top/gtdwdvsrtx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jlsjyb.cn/gtnqdduacu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xziqi.cn/gthgmgtven.html

[B03] switch / match / case
来源：http://hz.jqgufenzy.top/gttbzagmhc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hysaishi.cn/gtgetabptg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.feifeiyinyue.top/gteynfluld.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gogol.net.cn/gtkdjqnswa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.meibo888.top/gtwrxatnxc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.shanyushiyangtech.top/gtygpmskum.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jinqigfzy.top/gtttsdaoec.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.nanxuanxn.top/gtntlgvfvl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jinqigfzy.top/gtlqkqgopq.html

[B04] for 计数循环
来源：http://hz.ehwqpu.com/gtyuizemgl.html

Py:   for i in range(10): print(i)
来源：http://hz.ybcxt.top/gtebwsjfnw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xziqi.cn/gtcuxccfix.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gotoacloud.top/gtktmixvbv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shanyushiyangkeji.top/gtfpwjlugs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.kuanghao11.cn/gtrtieegrx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cheryme.top/gtguxrydgy.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jinghuilouyu.cn/gtcizbotvc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jyoumei.cn/gtfqrfjepj.html

[B05] 遍历数组 / 列表
来源：http://hz.jlsjyb.cn/gtvavgqcnv.html

Py:   for item in arr: print(item)
来源：http://hz.hysaishi.cn/gtduhcimjl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.chenlongwang.top/gtbdrffoed.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.316326.xyz/gthntxemjb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.kuanghao11.cn/gtapfahlyc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.gotoacloud.top/gtmmuvzzbe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.shuidangran.top/gtksgudnnk.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ivvv.top/gtljwavrap.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.gzhubu.top/gtacxcronq.html

[B06] 遍历字典 / 对象
来源：http://hz.daria6918.cn/gthmdlbrjg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.nanxinkj.top/gtbznpyqtm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hfpthk.cn/gtdlzrmtfz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.meibo888.top/gtbobirppd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.birdmap.top/gtipchldvj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.chenlongwang.top/gtvqcwelzd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ehwqpu.com/gtcrmizetj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jqgufenzy.top/gtvlbjxgkv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.ydjk.org.cn/gtvshyvfxw.html

[B07] while 循环
来源：http://hz.hongshengwenyu.top/gtjdrgvnpg.html

Py:   while i < 10: i += 1
来源：http://hz.316326.xyz/gtnpyxxsdn.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.sufxvd.cn/gtvfcseclt.html

JS:   while (i < 10) { i++; }
来源：http://hz.jinghuilouyu.cn/gtflkevrrv.html

TS:   while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gtnrmzgtaa.html

Java: while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gtscpqjhcm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jinghuilouyu.cn/gtsnnkgozf.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zdqjudy.top/gtstnxpbqq.html

C#:   while (i < 10) { i++; }
来源：http://hz.daria6918.cn/gtgnvojeba.html

[B08] do-while（至少执行一次）
来源：http://hz.guowangkeji.top/gtlsesfbfj.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.tian-w.cn/gtfgfhmkqk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gotoacloud.top/gtmfpuhorv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.daxiang520.top/gtkesxtksy.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yangfankeji.com/gtkbdlsxcd.html

Java: do { i++; } while (i < 10);
来源：http://hz.hnxiangtu.top/gtmjkfwnka.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ydzc1.top/gtiiadookz.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhixingplan.top/gtxmfoqfsx.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gtlxldejxk.html

[B09] break 与 continue
来源：http://hz.yj202588.top/gtdoivfesc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.wangshuangyany.cn/gtlvlmxaey.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtmagyybes.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.kuanghao11.cn/gtfxxallbx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuxming.cn/gtrhgbfdyh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gtpkndwsty.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ppjwa.cn/gtkyajnsts.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinqigfzy.top/gtywkqlhuk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cqqwz.cn/gtczadfoae.html

[B10] 遍历同时拿索引
来源：http://hz.jinqigufen.top/gtqltxjupm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.birdmap.top/gtfydtduqv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yongpay.top/gtgcajisrr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.0kj1m.cn/gtmuaqywqr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jlsjyb.cn/gtnsjfaczl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zycfv.cn/gtgzrdwame.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yangfankeji.com/gtigmomtoe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.pengpengdd.cyou/gtygatjbii.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.daxiang520.top/gttlaaeztt.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenzaomai.com/gtylgjqspl.html

Py:   list(range(0, 10, 2))
来源：http://hz.dashuyun.cn/gtihkfwkoa.html

PHP:  range(0, 10, 2);
来源：http://hz.chenzaomai.com/gtqeyeucao.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jiagoushi.top/gtsgjoyjos.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zycfv.cn/gthgznzqfu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ydjk.org.cn/gtvbrfqfjw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj202588.top/gthyummqal.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ybcxt.top/gtihffbfyp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.gotoacloud.top/gtjpwkkgbe.html

[B12] 跳出多层循环
来源：http://hz.aibaodan.cn/gtsdltlcxv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ehwqpu.com/gtqctlvsxr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jqgufenzy.top/gtklffwcdm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dashuyun.cn/gtsbprbzke.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gtlcyylzlq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gtxuvxgygz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhoulong.xyz/gtamwiocve.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.fengsongda.top/gtxexmtbuk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.birdmap.top/gtqslgkkyp.html

[B13] 判断是否为数字
来源：http://hz.316326.xyz/gtovjouxoj.html

Py:   isinstance(x, (int, float))
来源：http://hz.jqgufenzy.top/gtjcpztemk.html

PHP:  is_numeric($x)
来源：http://hz.nanxinkj.top/gtpvinrfvy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.andypj.xyz/gtkjugyybu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yangfankeji.com/gtbrwdulng.html

Java: x instanceof Number
来源：http://hz.feifeiyinyue.top/gtwitgwocc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hywenlv.cn/gtimzpjfcz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.pengpengdd.cyou/gtuevauexg.html

C#:   x is int or double or decimal
来源：http://hz.jianghu66.top/gtbuzhdeqj.html

[B14] 判断值是否在集合内
来源：http://hz.sufxvd.cn/gtdqrypzdk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.feifeiyinyue.top/gtfjaecpng.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yanxiufei.cn/gtyrvvtioc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.c1oappe.top/gtvuadbbws.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinyuanbaomall.cn/gtvxhdeqxx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hammf.cn/gtxqximyda.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sweek.top/gtuimxrnjl.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.316326.xyz/gttoxligkf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hywenlv.cn/gtjhtpcrbv.html

[B15] 布尔运算与取反
来源：http://hz.nanxuanxn.top/gtgvkqwvpv.html

Py:   a and b or not c
来源：http://hz.sysykeji.top/gtzpgaxpwx.html

PHP:  $a && $b || !$c
来源：http://hz.gotoacloud.top/gtfzqzjtrm.html

JS:   a && b || !c
来源：http://hz.aibaodan.cn/gtkertsiyh.html

TS:   a && b || !c
来源：http://hz.ivvv.top/gtqwlwauko.html

Java: a && b || !c
来源：http://hz.0kj1m.cn/gtrsuxeyzb.html

Go:   a && b || !c
来源：http://hz.meibo888.top/gtzvltmowa.html

Ruby: a && b || !c
来源：http://hz.mhx1999.top/gtczndunbi.html

C#:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtcgejphds.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hammf.cn/gttzmwxgvt.html

Py:   if not data: return
来源：http://hz.xuanzx.com/gtgbiumwsw.html

PHP:  if (!$data) { return; }
来源：http://hz.gogol.net.cn/gtodywchpf.html

JS:   if (!data) return;
来源：http://hz.tian-w.cn/gtnzpmxtna.html

TS:   if (!data) return;
来源：http://hz.mhx1999.top/gtftyeqihu.html

Java: if (data == null) return;
来源：http://hz.guannengcc.top/gtnxbtbwns.html

Go:   if data == nil { return }
来源：http://hz.hongshengwenyu.top/gtxdnzaarv.html

Ruby: return if data.nil?
来源：http://hz.shuidangran.top/gtpqcgkvka.html

C#:   if (data == null) return;
来源：http://hz.bjfxy.top/gttbedvbjk.html

================================================================================
来源：http://hz.nwbrower.top/gtmpbnhsci.html

C. 函数与作用域
来源：http://hz.mhx1999.top/gtzuzljjup.html

================================================================================
来源：http://hz.jyoumei.cn/gtiooosehu.html

[C01] 定义函数
来源：http://hz.feifeiyinyue.top/gtrwifafoq.html

Py:   def add(a, b): return a + b
来源：http://hz.gogol.net.cn/gtjxeomflt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtpyouxyjp.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtqrqqafqg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gtozcnuihj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtrfzslnfc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.52xcode.cn/gtvfbvswir.html

Ruby: def add(a, b); a + b; end
来源：http://hz.havefunace.top/gtkdieqyyo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cucudq.cn/gtnhmrveij.html

[C02] 默认参数
来源：http://hz.jiagoushi.top/gtmfclnnez.html

Py:   def greet(name="World"): return name
来源：http://hz.andypj.xyz/gtpaioihbw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.chenzaomai.com/gtetfngbrd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cucudq.cn/gtkefncnbv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xuetiantiany.cn/gtwuonjnyp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.gzhubu.top/gtdjxsebfr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ybcxt.top/gthozamumh.html

Ruby: def greet(name = "World") = name
来源：http://hz.fengsongda.top/gtymhvwbua.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ydjk.org.cn/gtryvnbiww.html

[C03] 可变参数
来源：http://hz.nwbrower.top/gtafvtolqi.html

Py:   def total(*args): return sum(args)
来源：http://hz.sweek.top/gtvaxpxaue.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.andypj.xyz/gtjqidzudi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.kuanghao11.cn/gthxwsaecb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shzxlz.cn/gthviozuxi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinqigfzy.top/gtdnlczpcm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sxryk.cn/gtwjsomvdd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.aibaodan.cn/gtxznchviq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zdqjudy.top/gtylkuinfv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinyuanbaomall.cn/gtukxgfusj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhoulong.xyz/gtevnibtqd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hysaishi.cn/gtcpnhoraq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yangfankeji.com/gtqrulxgia.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenjidiqi.icu/gtmmvccifh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yj20258888.top/gtabgyeqgh.html

Go:   // 无：用配置结构体参数
来源：http://hz.yongpay.top/gtoufbzxjk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.meibo888.top/gtpokmpypa.html

C#:   f(a: 1, b: 2)
来源：http://hz.meibo888.top/gtmgrdztkz.html

[C05] 返回多个值
来源：http://hz.quarkkingdee.top/gtfoqvrnno.html

Py:   return a, b
来源：http://hz.xuanzx.com/gtievrnazy.html

PHP:  return [$a, $b];
来源：http://hz.ivvv.top/gtjuudojbc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ppjwa.cn/gttubzqxjg.html

TS:   return { a, b };
来源：http://hz.ywan-chungtsiang.top/gtkgvpdpxm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ppjwa.cn/gtpkrdzscl.html

Go:   return a, b
来源：http://hz.xylfe.cn/gtancocifk.html

Ruby: return a, b
来源：http://hz.ydjk.org.cn/gtedarevpo.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhixingplan.top/gtbxkxmmkq.html

[C06] 匿名函数 / lambda
来源：http://hz.tianlin.xyz/gtijtuuyhj.html

Py:   square = lambda x: x * x
来源：http://hz.hysaishi.cn/gttykbxkhl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gzhubu.top/gtezpzmkrh.html

JS:   const square = x => x * x;
来源：http://hz.pycfn.com/gtfznabyta.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dashuyun.cn/gtapdaveir.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.fengsongda.top/gtezvymrop.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.iojbl.cn/gtlgtcaykj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.svipenyu.cn/gtqwevbqme.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ydjk.org.cn/gtjnndfqff.html

[C07] 把函数作为参数传入
来源：http://hz.quarkkingdee.top/gtfpldqzka.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ydzc1.top/gtcrhamnzv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ywan-chungtsiang.top/gthbebujoe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yongpay.top/gtjrabexml.html

TS:   arr.map(String)
来源：http://hz.zhixingplan.top/gtttlhumsh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.mhx1999.top/gtqmgqobkm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.c1oappe.top/gtnfikroln.html

Ruby: arr.map(&:upcase)
来源：http://hz.xziqi.cn/gtcctlbfwf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.dashuyun.cn/gtncyeanjd.html

[C08] 闭包
来源：http://hz.xingfuxueyuan.xyz/gtbpqzhmfd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.tanke756.top/gtgochwipo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zycfv.cn/gtoraoqdvd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.mhx1999.top/gtekhjbgma.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtoxmbdhnp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hysaishi.cn/gtxlajlylo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.birdmap.top/gtmxwwbotu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xinyue.icu/gtrbexkyyg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gtundxykfl.html

[C09] 递归
来源：http://hz.ybcxt.top/gtksokjthh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.fzhhl.top/gtfrpaaxhy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.dashuyun.cn/gtpjotbyxe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangkeji.top/gtrxdrxiio.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gtdirxnfry.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.mhx1999.top/gtcftxqedq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinqigufen.top/gtfvcfeasm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jianghu66.top/gtfxzcbrcd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yueranfly.top/gtpwryfzyp.html

[C10] 变量作用域
来源：http://hz.yanxiufei.cn/gtxswbjppp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yuanzhike.top/gthrqcpvqv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.pengpengdd.cyou/gtcpszrzto.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shanyushiyangtech.top/gtimxragfw.html

TS:   同 JS
来源：http://hz.zhongyouzk.top/gtlyhxmpfv.html

Java: 方法内为块级作用域
来源：http://hz.hongshengwenyu.top/gttunevrsr.html

Go:   花括号块级作用域
来源：http://hz.zhoulong.xyz/gtfrxukhgb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.shzxlz.cn/gttraxkgmv.html

C#:   块级作用域
来源：http://hz.daria6918.cn/gtplwogqra.html

[C11] 模块导入与导出
来源：http://hz.jinqigfzy.top/gtjijvwnag.html

Py:   from module import func
来源：http://hz.xylfe.cn/gtwygehrvi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinyuanbaomall.cn/gtvumxpfex.html


<!-- 参考信息 -->