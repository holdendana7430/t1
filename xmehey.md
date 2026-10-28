代发 wailian999

Ruby: a, b = b, a
来源：http://hz.ydjk.org.cn/gtuebbsfam.html

C#:   (a, b) = (b, a);
来源：http://hz.jinghuilouyu.cn/gtmvgntxez.html

[A20] 读取标准输入
来源：http://hz.gzhubu.top/gtktjidkqe.html

Py:   name = input("请输入：")
来源：http://hz.bjfxy.top/gthfhifysa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xinyue.icu/gtxgiesdiq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.dianchejie.cn/gtwhbykpgs.html

TS:   // Node.js：readline 模块
来源：http://hz.yj20258.top/gtlgtxmttc.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.mhx1999.top/gtvzuqzhre.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zhongyouzk.top/gttlzkldsz.html

Ruby: gets.chomp
来源：http://hz.yj202588.top/gtnlchbzjk.html

C#:   Console.ReadLine();
来源：http://hz.hfpthk.cn/gtjtyxkajb.html

[A21] 保留指定小数位输出
来源：http://hz.pycfn.com/gtrgdcmuvz.html

Py:   f"{3.14159:.2f}"
来源：http://hz.gogol.net.cn/gthenhuovk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.jqgfzy.top/gtrtnsqoao.html

JS:   (3.14159).toFixed(2)
来源：http://hz.iojbl.cn/gtrndxclbx.html

TS:   (3.14159).toFixed(2)
来源：http://hz.ydjk.org.cn/gtgwqtjsfa.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.birdmap.top/gtudegyhvj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jinqigufen.top/gthsoudgnx.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yvedp.cn/gtlrkzoqcw.html

C#:   3.14159.ToString("F2")
来源：http://hz.c1oappe.top/gtwhuamgkt.html

[A22] 获取字符串长度
来源：http://hz.hysaishi.cn/gtsbdypcfi.html

Py:   len(s)
来源：http://hz.xziqi.cn/gtxmwupath.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.svipenyu.cn/gtpilpouho.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.nwbrower.top/gtgzlinzsi.html

TS:   s.length
来源：http://hz.xuetiantiany.cn/gtqdkkeouq.html

Java: s.length()
来源：http://hz.guowangkeji.top/gtabsypwhl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.zhaomingkeji.xyz/gtmeuwardd.html

Ruby: s.length
来源：http://hz.redwolf501.top/gtcqcfqpkq.html

C#:   s.Length
来源：http://hz.jinyuanbaomall.cn/gtrxwbmoma.html

[A23] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtircwklfl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.aizwys.cn/gtdgzwduiu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.vqdsnc.cn/gtlmxxwvub.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.c1oappe.top/gtlpnzjcor.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhengqikj.top/gtenjxwvig.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenlongwang.top/gtrqldzllj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.smart0.xyz/gtptzamcgs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.hfpthk.cn/gthgtygyks.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.pengpengdd.cyou/gtrnbvmtts.html

[A24] 去除首尾空白
来源：http://hz.ehwqpu.com/gtfgntysed.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.ywan-chungtsiang.top/gtdrhaerbq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.sufxvd.cn/gtlcbmbbfc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xziqi.cn/gtxkigoiqx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xinyue.icu/gtzubhsqrt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.dianchejie.cn/gtgnpplcaa.html

Go:   strings.TrimSpace(s)
来源：http://hz.gogol.net.cn/gtwhpnkjfx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.guannengcc.top/gtmwlobngq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.jqgfzy.top/gtzuxwuaao.html

[A25] 字符串比较
来源：http://hz.iojbl.cn/gttmgqteyl.html

Py:   s1 == s2; s1 != s2
来源：http://hz.xinyue.icu/gtayxmuarw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.zhiwuduotai.top/gtnyginfcu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.bjfxy.top/gtcnmyzkzc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hongshengwenyu.top/gtymybbejt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.zhaomingkeji.xyz/gtjpmdmpsu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ywan-chungtsiang.top/gtlyexeibz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.cashguo.top/gtlfipeqwu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.chenlongwang.top/gtxiknxkca.html

[A26] 类型转换总览
来源：http://hz.yj20258.top/gtqsecrgac.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.tanke756.top/gtdrdxcegw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.gzhubu.top/gtjkbylnnb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.gaohongyu789.top/gtphcaejvo.html

TS:   Number() String() Boolean() x as number
来源：http://hz.sufxvd.cn/gtmjpmhwah.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.chenlongwang.top/gtstafxnxi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.ydzc1.top/gtumztzjdi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jianghu66.top/gtmntihlmk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yanxiufei.cn/gtdcvmwscb.html

================================================================================
来源：http://hz.guannengcc.top/gtiplqvqab.html

B. 流程控制
来源：http://hz.gogol.net.cn/gtxqcytxbb.html

================================================================================
来源：http://hz.zhengqikj.top/gtkygbcvyu.html

[B01] 条件判断 if / else
来源：http://hz.tianlin.xyz/gthrwizdru.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.sysykeji.top/gtgroeerte.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.tian-w.cn/gtxhlqdndg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sufxvd.cn/gtmogbpoll.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cashguo.top/gtcezabxii.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.wangshuangyany.cn/gtokfjfjnz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhaomingkeji.xyz/gtgivldxil.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jqgfzy.top/gtzwqgaknk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.birdmap.top/gtzwckxomw.html

[B02] 多分支 else if / elif
来源：http://hz.xziqi.cn/gteiyqxsyz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zdqjudy.top/gtjggbbyeo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.wangdashe.top/gtvhwudgoz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.52xcode.cn/gtrvppcvec.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xylfe.cn/gticsyobfl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.iojbl.cn/gtsiykobuk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.chenlongwang.top/gtlldywmwv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.shuidangran.top/gtgsrfboij.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxinkj.top/gtirllcear.html

[B03] switch / match / case
来源：http://hz.chenlongwang.top/gtrhtxawcb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.ppjwa.cn/gtdevntaqh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yonumen.top/gtsgsqzhfy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenlongwang.top/gtbkdktcdm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.nanxinkj.top/gtnhviaall.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.zhoulong.xyz/gtdkbcoltz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.shangyingyoupin.top/gtnpjzfxch.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.pycfn.com/gtovriamyy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.snrcjt.cn/gtkfotvqba.html

[B04] for 计数循环
来源：http://hz.chenzaomai.com/gtzeknfcjo.html

Py:   for i in range(10): print(i)
来源：http://hz.svipenyu.cn/gtglpeghmt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.ybcxt.top/gtnktlckuz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.tian-w.cn/gtiumcmgmf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jlsjyb.cn/gtozqxjbln.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhaomingkeji.xyz/gtidkzqgej.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.sweek.top/gtsgqqhnwm.html

Ruby: 10.times { |i| puts i }
来源：http://hz.dianchejie.cn/gtftzuamao.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xylfe.cn/gtroegfjtf.html

[B05] 遍历数组 / 列表
来源：http://hz.xylfe.cn/gtzukxoogh.html

Py:   for item in arr: print(item)
来源：http://hz.shangyingyoupin.top/gtofbrqrbd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.shangyingyoupin.top/gtfikghxps.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xziqi.cn/gtfvqtsbnz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.ydjk.org.cn/gtsymilrre.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.daxiang520.top/gtekhmdusu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.gogol.net.cn/gtekaqedrt.html

Ruby: arr.each { |item| puts item }
来源：http://hz.mhx1999.top/gtsosswtft.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jyoumei.cn/gtgcakbbqr.html

[B06] 遍历字典 / 对象
来源：http://hz.andypj.xyz/gttusqodvb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cashguo.top/gtcbdrunvc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hfpthk.cn/gtbmnvqxfc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.9152youxi.cn/gtnbmfafbp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinqigufen.top/gtbhfcamef.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.vqdsnc.cn/gtgnfqjixh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jiagoushi.top/gteownhnhc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.pycfn.com/gtijusyraa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hammf.cn/gtbfsdmhnm.html

[B07] while 循环
来源：http://hz.yj20258888.top/gtekmpgalo.html

Py:   while i < 10: i += 1
来源：http://hz.zycfv.cn/gtzvqasynm.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yvedp.cn/gtwihiqdjc.html

JS:   while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtokphosmz.html

TS:   while (i < 10) { i++; }
来源：http://hz.wangdashe.top/gttseiscwp.html

Java: while (i < 10) { i++; }
来源：http://hz.zycfv.cn/gtjyqtdztg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jinqigfzy.top/gtmzpciawx.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jlsjyb.cn/gtfwhtqhty.html

C#:   while (i < 10) { i++; }
来源：http://hz.jyoumei.cn/gtyxadppxb.html

[B08] do-while（至少执行一次）
来源：http://hz.tianlin.xyz/gtbkgvtuom.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.pengpengdd.cyou/gtpeojkznu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yj20258888.top/gtenylojtz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhixingplan.top/gtscuanetf.html

TS:   do { i++; } while (i < 10);
来源：http://hz.fzhhl.top/gtejrxpdmy.html

Java: do { i++; } while (i < 10);
来源：http://hz.hnqzz.top/gtthlytuuu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.0kj1m.cn/gtepghkanl.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jlsjyb.cn/gtgvtkahzp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gtwcyknndk.html

[B09] break 与 continue
来源：http://hz.gzhubu.top/gtoasmlpun.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jianghu66.top/gtsjikcnca.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zycfv.cn/gtqgyzzxka.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtfzjugcop.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yanxiufei.cn/gthuhflsur.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gtggdijxqr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.fzhhl.top/gtqfibajzk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hfpthk.cn/gtqzzflqlg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cdnleiting.top/gtdlszmqeq.html

[B10] 遍历同时拿索引
来源：http://hz.yj20258.top/gteiklkddc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.mhx1999.top/gtzegrbhhp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.quarkkingdee.top/gtdquhxeib.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ywan-chungtsiang.top/gtwhmvwpbm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhiwuduotai.top/gtdmuxmrsl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shanyushiyangkeji.top/gtnvdgvxxu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.svipenyu.cn/gtbptzuwvm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hnxiangtu.top/gtuslnmlrc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jiagoushi.top/gtszdsslwk.html

[B11] 生成数字序列 / 区间
来源：http://hz.pycfn.com/gtxcaetvfj.html

Py:   list(range(0, 10, 2))
来源：http://hz.cucudq.cn/gtmpzbpebe.html

PHP:  range(0, 10, 2);
来源：http://hz.zdqjudy.top/gtnfytlxyv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.meibo888.top/gterymzfkg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xuetiantiany.cn/gttnuxcdaa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zycfv.cn/gtdqsfnafo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.tianlin.xyz/gtcblyaqrz.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhoulong.xyz/gtpalbbcrc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.svipenyu.cn/gtouzzbdai.html

[B12] 跳出多层循环
来源：http://hz.tianlin.xyz/gtezisspmc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shanyushiyangtech.top/gtghtjwjcg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.dianchejie.cn/gtignhpbob.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnqzz.top/gtbvrmuzsv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gtxmrbhijg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.pengpengdd.cyou/gtodwapvzw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xuetiantiany.cn/gtjamenddu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hnqzz.top/gtfmvbelfb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yongpay.top/gtuahpguhy.html

[B13] 判断是否为数字
来源：http://hz.pycfn.com/gtnvweudqf.html

Py:   isinstance(x, (int, float))
来源：http://hz.yueranfly.top/gtyqzlclwk.html

PHP:  is_numeric($x)
来源：http://hz.zhoulong.xyz/gtufpovfob.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hongshengwenyu.top/gtpcgwehtg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cucudq.cn/gttymmxyup.html

Java: x instanceof Number
来源：http://hz.vqdsnc.cn/gtpgchpbtq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhongyouzk.top/gtuoqdjeew.html

Ruby: x.is_a?(Numeric)
来源：http://hz.316326.xyz/gtwcylpxuq.html

C#:   x is int or double or decimal
来源：http://hz.guannengcc.top/gtnfmpaxkb.html

[B14] 判断值是否在集合内
来源：http://hz.daria6918.cn/gtgyqkljon.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.aizwys.cn/gtuxknetza.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yongpay.top/gteowaswzd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhoulong.xyz/gtsgltoqne.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangtech.top/gtsdkiciwp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jiagoushi.top/gtzuzyuevj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.c1oappe.top/gtiqecztnz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ybcxt.top/gtsyyvxdmi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.dashuyun.cn/gtjgpjsgmv.html

[B15] 布尔运算与取反
来源：http://hz.wangshuangyany.cn/gtfqkjtyhh.html

Py:   a and b or not c
来源：http://hz.aizwys.cn/gtazmeguoc.html

PHP:  $a && $b || !$c
来源：http://hz.zhongyouzk.top/gtuqjgcqhz.html

JS:   a && b || !c
来源：http://hz.yonumen.top/gtfvsgynqm.html

TS:   a && b || !c
来源：http://hz.ybcxt.top/gtzgzkcikb.html

Java: a && b || !c
来源：http://hz.jinghuilouyu.cn/gtgxactmyo.html

Go:   a && b || !c
来源：http://hz.wangshuangyany.cn/gtipdetbop.html

Ruby: a && b || !c
来源：http://hz.hywenlv.cn/gtnhyhlhpl.html

C#:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtwbncxtji.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hfpthk.cn/gtabnvbhnx.html

Py:   if not data: return
来源：http://hz.9152youxi.cn/gtnfzpbmql.html

PHP:  if (!$data) { return; }
来源：http://hz.yangfankeji.com/gtwateqtuc.html

JS:   if (!data) return;
来源：http://hz.hysaishi.cn/gtlmphoqnq.html

TS:   if (!data) return;
来源：http://hz.jinqigufen.top/gttbgnphjj.html

Java: if (data == null) return;
来源：http://hz.yvedp.cn/gtovmizydd.html

Go:   if data == nil { return }
来源：http://hz.sufxvd.cn/gtdxmofulq.html

Ruby: return if data.nil?
来源：http://hz.havefunace.top/gtimkzwkbd.html

C#:   if (data == null) return;
来源：http://hz.ydzc1.top/gtiutmhfsh.html

================================================================================
来源：http://hz.cqqwz.cn/gtdyybgnmf.html

C. 函数与作用域
来源：http://hz.chenjidiqi.icu/gtxttpnvbk.html

================================================================================
来源：http://hz.vqdsnc.cn/gtleqlxgso.html

[C01] 定义函数
来源：http://hz.guowangkeji.top/gtrprwbcfg.html

Py:   def add(a, b): return a + b
来源：http://hz.cqqwz.cn/gtwzkoueee.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtgpjuqvro.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jianghu66.top/gtnhipokmm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hongshengwenyu.top/gtjdwbycdw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtiosuvaml.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinyuanbaomall.cn/gtmyexjyxw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.snrcjt.cn/gtnxpyecmb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtzzyrvgcg.html

[C02] 默认参数
来源：http://hz.dashuyun.cn/gtvtchvbhy.html

Py:   def greet(name="World"): return name
来源：http://hz.ydjk.org.cn/gtatdknsec.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hongshengwenyu.top/gtyurnakgm.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhixingplan.top/gtdnvzpqjg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.birdmap.top/gtoyzrthxg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xuanzx.com/gtmgqwxekd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.chenzaomai.com/gtscsakbct.html

Ruby: def greet(name = "World") = name
来源：http://hz.snrcjt.cn/gtxfwbzpgv.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yueranfly.top/gtyixmylah.html

[C03] 可变参数
来源：http://hz.yueranfly.top/gtzilctkvr.html

Py:   def total(*args): return sum(args)
来源：http://hz.yonumen.top/gtkcttvhtt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hywenlv.cn/gtjvchfwxd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.52xcode.cn/gtqvqqarzt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenlongwang.top/gtnkoabebr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.snrcjt.cn/gtvzcwdxgl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hongshengwenyu.top/gtxchklaxf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.pengpengdd.cyou/gtpshzwial.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yonumen.top/gtrfawyhml.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shanyushiyangkeji.top/gthgopwnfp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tanke756.top/gtzykabuss.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.birdmap.top/gtxdmvsiyr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.feifeiyinyue.top/gtmjnbukar.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.guowangkeji.top/gtfhzqhcne.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.wangdashe.top/gtgvvlyxst.html

Go:   // 无：用配置结构体参数
来源：http://hz.havefunace.top/gttgigauaq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cucudq.cn/gtgvkpuccc.html

C#:   f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtcmxnphzb.html

[C05] 返回多个值
来源：http://hz.tianlin.xyz/gtpsbwdfws.html

Py:   return a, b
来源：http://hz.wangdashe.top/gtfhwpetrd.html

PHP:  return [$a, $b];
来源：http://hz.redwolf501.top/gtxfnxcqmt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cucudq.cn/gtoywkitvt.html

TS:   return { a, b };
来源：http://hz.yj20258888.top/gtdptunwqx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.fengsongda.top/gtlspqnncq.html

Go:   return a, b
来源：http://hz.chenjidiqi.icu/gtkwllkyll.html

Ruby: return a, b
来源：http://hz.sufxvd.cn/gtvdzbzavp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cucudq.cn/gtglmbpmuk.html

[C06] 匿名函数 / lambda
来源：http://hz.sxryk.cn/gtpddkwfwq.html

Py:   square = lambda x: x * x
来源：http://hz.fzhhl.top/gtowcypafr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shangyingyoupin.top/gtwqxwiose.html

JS:   const square = x => x * x;
来源：http://hz.zhixingplan.top/gtewxfgqjh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yuxming.cn/gtqakeyoot.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gotoacloud.top/gtotepjwfn.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.meibo888.top/gtrhxgavwi.html

Ruby: square = ->(x) { x * x }
来源：http://hz.guannengcc.top/gtrmyagcut.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.wangshuangyany.cn/gtzlnfebpm.html

[C07] 把函数作为参数传入
来源：http://hz.sweek.top/gtqwbcjjem.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ydzc1.top/gtlbmftmxw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hysaishi.cn/gtrgotytlk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.mhx1999.top/gtvmaulxll.html

TS:   arr.map(String)
来源：http://hz.cdnleiting.top/gturketcdp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shangyingyoupin.top/gtnrzltisg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.redwolf501.top/gtmxwapljt.html

Ruby: arr.map(&:upcase)
来源：http://hz.52xcode.cn/gthdtdrgzo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yuanzhike.top/gtzvtpthfh.html

[C08] 闭包
来源：http://hz.mhx1999.top/gtmdigysrt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gogol.net.cn/gtrdkhkeud.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yangfankeji.com/gtsfakrbvq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtldpgslpr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtpkcclgsh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xuetiantiany.cn/gtrrpvbcux.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.daxiang520.top/gtchafhofc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ywan-chungtsiang.top/gtntftmsfr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtzxuzdefj.html

[C09] 递归
来源：http://hz.9152youxi.cn/gtjxiyedez.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinghuilouyu.cn/gtzmymmuyj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinqigufen.top/gtbpyichug.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.haohaochexian.top/gtflqplxff.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.daxiang520.top/gtspjjmmuy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yvedp.cn/gtcpxesspt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhixingplan.top/gtkczvalyx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.andypj.xyz/gtuxstpkhn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xylfe.cn/gtvxobeunx.html

[C10] 变量作用域
来源：http://hz.chenzaomai.com/gtyyomzime.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.haohaochexian.top/gtdkokzodm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangdashe.top/gttwllcwul.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhengqikj.top/gtdphzkxzx.html


<!-- 参考信息 -->