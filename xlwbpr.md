代发 wailian999

C#:   (int)'A'; (char)65
来源：http://hz.gaohongyu789.top/gtjpssujog.html

[A19] 交换两个变量
来源：http://hz.jlsjyb.cn/gtmmchkosn.html

Py:   a, b = b, a
来源：http://hz.zhixingplan.top/gtwzhioswt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.gzhubu.top/gtfdloxhjb.html

JS:   [a, b] = [b, a];
来源：http://hz.xuetiantiany.cn/gthkadfuht.html

TS:   [a, b] = [b, a];
来源：http://hz.yangfankeji.com/gtvlfiqewg.html

Java: int t = a; a = b; b = t;
来源：http://hz.zhijiandao.cn/gtskmcvbct.html

Go:   a, b = b, a
来源：http://hz.kuanghao11.cn/gtzrasbrgh.html

Ruby: a, b = b, a
来源：http://hz.birdmap.top/gtdsbuusdj.html

C#:   (a, b) = (b, a);
来源：http://hz.316326.xyz/gtkcyvnzna.html

[A20] 读取标准输入
来源：http://hz.meibo888.top/gttmrjfbsd.html

Py:   name = input("请输入：")
来源：http://hz.hnqzz.top/gtmebptiay.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.daria6918.cn/gtfkeragaz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.ppjwa.cn/gteevwiinf.html

TS:   // Node.js：readline 模块
来源：http://hz.shanyushiyangtech.top/gtuouldpjh.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.redwolf501.top/gtksxmmuar.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zhiwuduotai.top/gtfvfpjtqk.html

Ruby: gets.chomp
来源：http://hz.pycfn.com/gtmhlirlas.html

C#:   Console.ReadLine();
来源：http://hz.meibo888.top/gtebgxbzve.html

[A21] 保留指定小数位输出
来源：http://hz.jqgfzy.top/gtklsqiohg.html

Py:   f"{3.14159:.2f}"
来源：http://hz.hfpthk.cn/gtfoyrwstk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.kuanghao11.cn/gtkbozmlky.html

JS:   (3.14159).toFixed(2)
来源：http://hz.jinqigfzy.top/gtgrfxdvza.html

TS:   (3.14159).toFixed(2)
来源：http://hz.xuanzx.com/gttidrxlhz.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.nanxinkj.top/gttntlmfpj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.xingfuxueyuan.xyz/gtslfrefds.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.andypj.xyz/gtkpxyjhqh.html

C#:   3.14159.ToString("F2")
来源：http://hz.ybcxt.top/gtphobuhpr.html

[A22] 获取字符串长度
来源：http://hz.hnxiangtu.top/gtqhkcexdq.html

Py:   len(s)
来源：http://hz.jinyuanbaomall.cn/gtdrgfqibf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.pycfn.com/gtxeakgsdo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yuanzhike.top/gttpcryxfs.html

TS:   s.length
来源：http://hz.ppjwa.cn/gtaislfqmx.html

Java: s.length()
来源：http://hz.dashuyun.cn/gtbhfptkvo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.tian-w.cn/gtvjcymuya.html

Ruby: s.length
来源：http://hz.zhixingplan.top/gtspnukeba.html

C#:   s.Length
来源：http://hz.gotoacloud.top/gtzrqpicga.html

[A23] 大小写转换
来源：http://hz.andypj.xyz/gtlrmfetxi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.gzhubu.top/gtqcgoxykg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.meibo888.top/gtpmykkvhk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.gogol.net.cn/gtadrplzch.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.feifeiyinyue.top/gtlrvqiivv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.snrcjt.cn/gtltmjnlms.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.fengsongda.top/gtbnoxrwov.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.haohaochexian.top/gtmykvodti.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.guannengcc.top/gthstvlzku.html

[A24] 去除首尾空白
来源：http://hz.0kj1m.cn/gtgmgmvjhv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.zhoulong.xyz/gtopzhciop.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.guannengcc.top/gtuzntpehz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ybcxt.top/gtoncwqsmd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.chenzaomai.com/gtkmgicqaa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ywan-chungtsiang.top/gtlmwxklum.html

Go:   strings.TrimSpace(s)
来源：http://hz.jqgufenzy.top/gtkzvktxlq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.gotoacloud.top/gtlozipawi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.ehwqpu.com/gtttkzhjkj.html

[A25] 字符串比较
来源：http://hz.tianlin.xyz/gtspvydlde.html

Py:   s1 == s2; s1 != s2
来源：http://hz.quarkkingdee.top/gttokieewn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.nwbrower.top/gtaxlgkqsj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.cheryme.top/gtvzruoqyp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.fzhhl.top/gtnosxxtcb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.cashguo.top/gtxogoqxwc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.chenlongwang.top/gtcihhkxzd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.zhaomingkeji.xyz/gtqvaabwkk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ydzc1.top/gtseygljrq.html

[A26] 类型转换总览
来源：http://hz.dianchejie.cn/gtfsazhjnb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zycfv.cn/gtxknfchzb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.316326.xyz/gttwtuhgez.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.cheryme.top/gtochxbrkc.html

TS:   Number() String() Boolean() x as number
来源：http://hz.wangshuangyany.cn/gthghxqqsp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yvedp.cn/gthpqrfnbv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.chenjidiqi.icu/gtuiymwcip.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.c1oappe.top/gtjnkkayvv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.hywenlv.cn/gtbvcsssix.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwbysmifn.html

B. 流程控制
来源：http://hz.snrcjt.cn/gtvollphgq.html

================================================================================
来源：http://hz.pycfn.com/gtkgarngaw.html

[B01] 条件判断 if / else
来源：http://hz.zhaomingkeji.xyz/gtyaqimbyp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.xuetiantiany.cn/gtsjlhkbwy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.redwolf501.top/gtdpexmrku.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gtobdaytun.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhongyouzk.top/gtzarbayad.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.havefunace.top/gttyyrlzew.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.0kj1m.cn/gtsgtmovcr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.chenzaomai.com/gtqnatjfwm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhoulong.xyz/gtgszmgfjd.html

[B02] 多分支 else if / elif
来源：http://hz.xziqi.cn/gtfzjlijaa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.cqqwz.cn/gtjzcowoak.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.ywan-chungtsiang.top/gtcyhrvjst.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jyoumei.cn/gthxjuaeyt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xingfuxueyuan.xyz/gtiycnyzin.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.mhx1999.top/gtnxrqkbfc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.smart0.xyz/gttqrknjrl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.0kj1m.cn/gtukpanlwd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ybcxt.top/gtyqtchrgo.html

[B03] switch / match / case
来源：http://hz.wangdashe.top/gtfjuslius.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.vqdsnc.cn/gtiiqyhuqb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ivvv.top/gtgjuoefbc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yuanzhike.top/gteidbmfez.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhengqikj.top/gtadmjhwfg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.c1oappe.top/gtfhmocupr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.meibo888.top/gtvnvsfirv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.chenzaomai.com/gtmcaopqfi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.hnxiangtu.top/gtpzsrludh.html

[B04] for 计数循环
来源：http://hz.zhijiandao.cn/gtxavnlxmm.html

Py:   for i in range(10): print(i)
来源：http://hz.gogol.net.cn/gtivrkwyce.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.ivvv.top/gtdjhswuol.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yueranfly.top/gtsejgogft.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jqgufenzy.top/gtbbyhdtwc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.cdnleiting.top/gtolkkvgew.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ydjk.org.cn/gtgqvvwrim.html

Ruby: 10.times { |i| puts i }
来源：http://hz.vqdsnc.cn/gtsnrnldvb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.aibaodan.cn/gtyqsfnrwu.html

[B05] 遍历数组 / 列表
来源：http://hz.ehwqpu.com/gtsvieghbe.html

Py:   for item in arr: print(item)
来源：http://hz.havefunace.top/gthnkctreg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ydzc1.top/gtycgtiwgm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ybcxt.top/gtkkwiefvn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yanxiufei.cn/gthjiglepi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.gzhubu.top/gtxifupiva.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hnqzz.top/gtgybfihye.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yj20258.top/gtbdntdysy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jiagoushi.top/gtvcxakrpb.html

[B06] 遍历字典 / 对象
来源：http://hz.jyoumei.cn/gtjodxdlqu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.haohaochexian.top/gtxpvmfmlv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinqigufen.top/gtfnuckkgv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gzhubu.top/gtyfxjasnd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.pycfn.com/gticpvjmxh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hnxiangtu.top/gtadagmyhg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.andypj.xyz/gtlmipwqev.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.daria6918.cn/gtyrynfowv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yuxming.cn/gtatohonic.html

[B07] while 循环
来源：http://hz.chenlongwang.top/gttxddhict.html

Py:   while i < 10: i += 1
来源：http://hz.ybcxt.top/gtfuaiscuh.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.guowangkeji.top/gtgtylvmck.html

JS:   while (i < 10) { i++; }
来源：http://hz.gzhubu.top/gtrkzgtmep.html

TS:   while (i < 10) { i++; }
来源：http://hz.cashguo.top/gtifxxuhrp.html

Java: while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gtdjwxzojs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.daria6918.cn/gtmvggeyuh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.smart0.xyz/gtflfklgsq.html

C#:   while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gthihebsav.html

[B08] do-while（至少执行一次）
来源：http://hz.nwbrower.top/gtfzrxfnmt.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zdqjudy.top/gtxuhqteau.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yonumen.top/gtrtadzdxw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.chenzaomai.com/gtsbxctupn.html

TS:   do { i++; } while (i < 10);
来源：http://hz.wangdashe.top/gtojnneyde.html

Java: do { i++; } while (i < 10);
来源：http://hz.iojbl.cn/gtlfxhrccj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.c1oappe.top/gtvimdayfi.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jinghuilouyu.cn/gtmgojbmon.html

C#:   do { i++; } while (i < 10);
来源：http://hz.chenzaomai.com/gtalkcdlcx.html

[B09] break 与 continue
来源：http://hz.guannengcc.top/gtbnpbggoz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.tanke756.top/gtmaqourht.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yj202588.top/gtgsctkjwe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuanzhike.top/gtycjgxmfv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yangfankeji.com/gteyxkgdka.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtrkpmbjez.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.feifeiyinyue.top/gtzxhikzoy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yonumen.top/gtjtopexzm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xylfe.cn/gtljwmnnui.html

[B10] 遍历同时拿索引
来源：http://hz.ydjk.org.cn/gtvxysllqz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jlsjyb.cn/gtkwkshqrr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gzhubu.top/gtigtgsway.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yongpay.top/gtxdxsicjl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ybcxt.top/gtzoqbnvcg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shangyingyoupin.top/gtqyjlssla.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.pycfn.com/gthubuzrjk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.feifeiyinyue.top/gtcamlsrny.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gzhubu.top/gtbksdowts.html

[B11] 生成数字序列 / 区间
来源：http://hz.yj20258888.top/gtmjfskuyf.html

Py:   list(range(0, 10, 2))
来源：http://hz.gotoacloud.top/gtlxtgvzyt.html

PHP:  range(0, 10, 2);
来源：http://hz.meibo888.top/gtwtwdhlvd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ivvv.top/gtggvkdkhk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.smart0.xyz/gtzxkgmkuc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jqgfzy.top/gtzkymfzvh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xinyue.icu/gteuxeqnzp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sufxvd.cn/gtlbwfipxh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.dashuyun.cn/gtquwkmiox.html

[B12] 跳出多层循环
来源：http://hz.cqqwz.cn/gtffhqezkw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.quarkkingdee.top/gtitbklboq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jinghuilouyu.cn/gthdodpmiv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinyuanbaomall.cn/gtfgcccilu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtkypdpsyw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cheryme.top/gtkpkvxznu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ivvv.top/gtmlyqnbfg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ybcxt.top/gtlknwvdff.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shanyushiyangkeji.top/gtqjugwjdu.html

[B13] 判断是否为数字
来源：http://hz.cheryme.top/gtdojqoujz.html

Py:   isinstance(x, (int, float))
来源：http://hz.yvedp.cn/gtjcuysqaj.html

PHP:  is_numeric($x)
来源：http://hz.shzxlz.cn/gtebsiosrp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shuidangran.top/gtbkipbhie.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fengsongda.top/gthpllnoxr.html

Java: x instanceof Number
来源：http://hz.dashuyun.cn/gtqelyoowi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xziqi.cn/gtlagfpqfn.html

Ruby: x.is_a?(Numeric)
来源：http://hz.bjfxy.top/gthtojqmpd.html

C#:   x is int or double or decimal
来源：http://hz.yangfankeji.com/gtfzsgybaq.html

[B14] 判断值是否在集合内
来源：http://hz.haohaochexian.top/gtskgzktdb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.andypj.xyz/gtuwwpmxdg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zycfv.cn/gtonrmtzvt.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangkeji.top/gtqkrasump.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.chenzaomai.com/gtncnjkxvn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hongshengwenyu.top/gtqsowpfft.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.svipenyu.cn/gtfycxkdnw.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ppjwa.cn/gtukqdqklk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhongyouzk.top/gthglwyitg.html

[B15] 布尔运算与取反
来源：http://hz.birdmap.top/gtitaoqwlv.html

Py:   a and b or not c
来源：http://hz.guowangkeji.top/gtbgizuirf.html

PHP:  $a && $b || !$c
来源：http://hz.feifeiyinyue.top/gtrzsbwjjq.html

JS:   a && b || !c
来源：http://hz.yongpay.top/gtubkoakgi.html

TS:   a && b || !c
来源：http://hz.zdqjudy.top/gtpjwxjbuo.html

Java: a && b || !c
来源：http://hz.aibaodan.cn/gtoxzwnnfn.html

Go:   a && b || !c
来源：http://hz.dianchejie.cn/gtvsowwrrc.html

Ruby: a && b || !c
来源：http://hz.jqgfzy.top/gtxzflsgok.html

C#:   a && b || !c
来源：http://hz.fengsongda.top/gtpkycqqji.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.svipenyu.cn/gtwefgrzek.html

Py:   if not data: return
来源：http://hz.jqgufenzy.top/gtqmelywra.html

PHP:  if (!$data) { return; }
来源：http://hz.ehwqpu.com/gtaqpoxqqw.html

JS:   if (!data) return;
来源：http://hz.hnxiangtu.top/gtcjufjefr.html

TS:   if (!data) return;
来源：http://hz.sweek.top/gtzruikcue.html

Java: if (data == null) return;
来源：http://hz.zhixingplan.top/gtsmqxlufq.html

Go:   if data == nil { return }
来源：http://hz.shzxlz.cn/gthchercee.html

Ruby: return if data.nil?
来源：http://hz.shanyushiyangkeji.top/gtrfuilwix.html

C#:   if (data == null) return;
来源：http://hz.jinyuanbaomall.cn/gtexhjofme.html

================================================================================
来源：http://hz.yj20258.top/gtfilyyhee.html

C. 函数与作用域
来源：http://hz.hnqzz.top/gtjrgnzsvi.html

================================================================================
来源：http://hz.jinqigufen.top/gtmadrqqyn.html

[C01] 定义函数
来源：http://hz.zhoulong.xyz/gthqgjxxgm.html

Py:   def add(a, b): return a + b
来源：http://hz.gotoacloud.top/gtmycncpwj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhoulong.xyz/gtpsryyaml.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.bjfxy.top/gtqsuwfefn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258888.top/gtjimxtjuc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtfeoghsjv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guannengcc.top/gtvvslbcon.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sysykeji.top/gtpumburua.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtkxvcqeap.html

[C02] 默认参数
来源：http://hz.nanxinkj.top/gtplbwolon.html

Py:   def greet(name="World"): return name
来源：http://hz.yuanzhike.top/gtjfldgvnk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cucudq.cn/gtmkrijldx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.snrcjt.cn/gtsvddzzkm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xuanzx.com/gtyplkjefa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hysaishi.cn/gtqfqoidkm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yangfankeji.com/gtxocewadd.html

Ruby: def greet(name = "World") = name
来源：http://hz.cucudq.cn/gtsfwdywzp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.havefunace.top/gtxclrwdbb.html

[C03] 可变参数
来源：http://hz.yongpay.top/gtirwyervp.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj202588.top/gthyxibbwv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhiwuduotai.top/gttnzsahjj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fengsongda.top/gtgkysuakh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guowangkeji.top/gttdfrozhe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hongshengwenyu.top/gtdgsclxsk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.chenzaomai.com/gtgvvoqmmd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinyuanbaomall.cn/gtmgtweeqh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.mhx1999.top/gtbowaeoky.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hfpthk.cn/gtmxcyfowg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yongpay.top/gtfikjznsl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ivvv.top/gtlvlqrzuc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shuidangran.top/gtptdjhcxq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gaohongyu789.top/gtsfhwhpox.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenzaomai.com/gtadyljgvt.html

Go:   // 无：用配置结构体参数
来源：http://hz.shanyushiyangkeji.top/gtgbrhfsor.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gtzedibqhl.html

C#:   f(a: 1, b: 2)
来源：http://hz.tianlin.xyz/gtdvumpkhl.html

[C05] 返回多个值
来源：http://hz.nwbrower.top/gtqxljkfly.html

Py:   return a, b
来源：http://hz.cashguo.top/gtpyjdpcpt.html

PHP:  return [$a, $b];
来源：http://hz.guowangkeji.top/gtyhadobrb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.fengsongda.top/gtedquvinv.html

TS:   return { a, b };
来源：http://hz.yonumen.top/gtivbakhvg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xuetiantiany.cn/gtwhzpahvf.html

Go:   return a, b
来源：http://hz.xuanzx.com/gtywoveeqf.html

Ruby: return a, b
来源：http://hz.daria6918.cn/gtwkhvpcnz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ywan-chungtsiang.top/gtkfltldih.html

[C06] 匿名函数 / lambda
来源：http://hz.redwolf501.top/gtqtqeenvw.html

Py:   square = lambda x: x * x
来源：http://hz.havefunace.top/gtjiowxzyf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.dianchejie.cn/gtkfdlwdcf.html

JS:   const square = x => x * x;
来源：http://hz.shanyushiyangkeji.top/gtqwsihcqt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.redwolf501.top/gtwghvbyce.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ywan-chungtsiang.top/gtkriqcjma.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shuidangran.top/gthvrqumix.html

Ruby: square = ->(x) { x * x }
来源：http://hz.meibo888.top/gtruxlcwtz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gzhubu.top/gtabukenzy.html

[C07] 把函数作为参数传入
来源：http://hz.wangdashe.top/gtbhubfisb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shanyushiyangkeji.top/gtjwnctmnb.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dashuyun.cn/gtwwqbvnpb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.snrcjt.cn/gtivhoyewd.html

TS:   arr.map(String)
来源：http://hz.quarkkingdee.top/gtvtvcmmgd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cqqwz.cn/gtdgctmfsy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.9152youxi.cn/gtnsmcjsrz.html

Ruby: arr.map(&:upcase)
来源：http://hz.316326.xyz/gtssdxeaxh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xylfe.cn/gtmwsnrgfk.html

[C08] 闭包
来源：http://hz.yuanzhike.top/gtvnpcppox.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ivvv.top/gtfqlbkwgy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ehwqpu.com/gtxrcchgoi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xuanzx.com/gtswzkeplj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtovtglsan.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinyuanbaomall.cn/gthgsazsng.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.guowangkeji.top/gtbsqetzsd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xylfe.cn/gtedxpryeh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xylfe.cn/gtgsojpdfd.html

[C09] 递归
来源：http://hz.haohaochexian.top/gtizugnglj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gtisdtgjwf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.daria6918.cn/gtaiubrurz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.mhx1999.top/gtsalrzdho.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtmjoukfnx.html


<!-- 参考信息 -->