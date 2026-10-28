代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://hz.sweek.top/gtkpqsluua.html

Py:   ord("A"); chr(65)
来源：http://hz.meibo888.top/gtiubngpzu.html

PHP:  ord("A"); chr(65)
来源：http://hz.pengpengdd.cyou/gtnpjjcyib.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yangfankeji.com/gtctuxqpae.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.9152youxi.cn/gthrgrdtyu.html

Java: (int) 'A'; (char) 65
来源：http://hz.jlsjyb.cn/gtpqrcuytb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.gotoacloud.top/gtyhsqsdye.html

Ruby: "A".ord; 65.chr
来源：http://hz.jinqigufen.top/gtzougoxhc.html

C#:   (int)'A'; (char)65
来源：http://hz.zhongyouzk.top/gtseijhbxy.html

[A19] 交换两个变量
来源：http://hz.chenlongwang.top/gtmrwmlyku.html

Py:   a, b = b, a
来源：http://hz.jlsjyb.cn/gtjoqyviml.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.zhijiandao.cn/gtuuuulgji.html

JS:   [a, b] = [b, a];
来源：http://hz.gogol.net.cn/gtbvfhgtxn.html

TS:   [a, b] = [b, a];
来源：http://hz.dashuyun.cn/gtdqaxcytp.html

Java: int t = a; a = b; b = t;
来源：http://hz.nanxinkj.top/gtmospglro.html

Go:   a, b = b, a
来源：http://hz.zhongyouzk.top/gtqssuakvd.html

Ruby: a, b = b, a
来源：http://hz.ybcxt.top/gtyxmggvrl.html

C#:   (a, b) = (b, a);
来源：http://hz.ybcxt.top/gtpzondcqf.html

[A20] 读取标准输入
来源：http://hz.ivvv.top/gtwzmuxyck.html

Py:   name = input("请输入：")
来源：http://hz.ppjwa.cn/gtbwnjikov.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.redwolf501.top/gtlbciibzm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.jqgfzy.top/gtwywupuqd.html

TS:   // Node.js：readline 模块
来源：http://hz.yj20258888.top/gtkdeawhzy.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.xziqi.cn/gtzdsqnaqf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.xuanzx.com/gtwoslldoj.html

Ruby: gets.chomp
来源：http://hz.c1oappe.top/gtlrusejrm.html

C#:   Console.ReadLine();
来源：http://hz.sxryk.cn/gtmstnwwsd.html

[A21] 保留指定小数位输出
来源：http://hz.0kj1m.cn/gtashnsova.html

Py:   f"{3.14159:.2f}"
来源：http://hz.havefunace.top/gtuarrqoso.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.gotoacloud.top/gtoqqfbtkw.html

JS:   (3.14159).toFixed(2)
来源：http://hz.fengsongda.top/gttmtkfhbh.html

TS:   (3.14159).toFixed(2)
来源：http://hz.chenjidiqi.icu/gtpylzpepl.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ydjk.org.cn/gtzkkxiiri.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.gaohongyu789.top/gteemabmsq.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.wangdashe.top/gtsqaxcnrc.html

C#:   3.14159.ToString("F2")
来源：http://hz.zycfv.cn/gtsnegnrcu.html

[A22] 获取字符串长度
来源：http://hz.yj20258888.top/gtpszktzmp.html

Py:   len(s)
来源：http://hz.dianchejie.cn/gtmlvkzsop.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.zhengqikj.top/gtkeflxmty.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zhaomingkeji.xyz/gtptkhdfnf.html

TS:   s.length
来源：http://hz.yj202588.top/gtguqwpbrs.html

Java: s.length()
来源：http://hz.havefunace.top/gtblcpiows.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.dianchejie.cn/gtowsypzyc.html

Ruby: s.length
来源：http://hz.chenlongwang.top/gtclwxwyye.html

C#:   s.Length
来源：http://hz.xingfuxueyuan.xyz/gtbknimvvx.html

[A23] 大小写转换
来源：http://hz.yonumen.top/gtopbxtlre.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.fengsongda.top/gtozrxcbkr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.xingfuxueyuan.xyz/gtgakuyvrq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.pengpengdd.cyou/gtaghnzovh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.daria6918.cn/gtgjayjozn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.xingfuxueyuan.xyz/gtagvjlwuw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jinghuilouyu.cn/gtzqtvlnqh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.cdnleiting.top/gtwvotcqmc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.zhixingplan.top/gtghspcadi.html

[A24] 去除首尾空白
来源：http://hz.yvedp.cn/gtzgftrzke.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.haohaochexian.top/gtkeipxawt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yueranfly.top/gtiuhzmbhi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tanke756.top/gtoaqnlnzt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ivvv.top/gtcfglxfjc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.xuanzx.com/gtkitittxs.html

Go:   strings.TrimSpace(s)
来源：http://hz.nwbrower.top/gtimordjgm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.meibo888.top/gtcpdxojmr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.hnqzz.top/gtnlhoobpj.html

[A25] 字符串比较
来源：http://hz.yj202588.top/gtmnsxjuqu.html

Py:   s1 == s2; s1 != s2
来源：http://hz.cdnleiting.top/gthrsupkta.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jianghu66.top/gtdcbjyctl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tianlin.xyz/gtovsfslip.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xylfe.cn/gtejziwxyb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.redwolf501.top/gtxhjupqoy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.birdmap.top/gtyvngczqh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jinqigfzy.top/gtuwlkwwig.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yj202588.top/gtrupktqdi.html

[A26] 类型转换总览
来源：http://hz.snrcjt.cn/gtvxrizjmj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.dashuyun.cn/gtfgvwswga.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.ywan-chungtsiang.top/gtmymvnigb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.chenzaomai.com/gtiotuqdfy.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yj20258.top/gtycsytdrk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhixingplan.top/gtespjxjya.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.chenjidiqi.icu/gtljanudks.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.haohaochexian.top/gtckuuupba.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.cqqwz.cn/gtxowrxzut.html

================================================================================
来源：http://hz.xziqi.cn/gtipftwvwr.html

B. 流程控制
来源：http://hz.shangyingyoupin.top/gtpupaqtyk.html

================================================================================
来源：http://hz.zycfv.cn/gtogkkdaig.html

[B01] 条件判断 if / else
来源：http://hz.xziqi.cn/gtwtzejiyw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.tianlin.xyz/gtldwpfprp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yuxming.cn/gthsozggik.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.quarkkingdee.top/gtplqahlau.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhongyouzk.top/gtvodybiqo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.guannengcc.top/gtzmrktovt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.vqdsnc.cn/gtqlghewmx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.xylfe.cn/gtaxqjammn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.316326.xyz/gtpfrdntrr.html

[B02] 多分支 else if / elif
来源：http://hz.sysykeji.top/gtpggxqoue.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.guannengcc.top/gtemfdabkj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jyoumei.cn/gtcrgmpfrz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.havefunace.top/gtxsqrmaag.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xingfuxueyuan.xyz/gtexzhtsyo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhijiandao.cn/gtxbszrpyl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.pengpengdd.cyou/gtezllshiw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.smart0.xyz/gtmcydzbig.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shangyingyoupin.top/gtaarnvrru.html

[B03] switch / match / case
来源：http://hz.andypj.xyz/gtmvomprgs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jyoumei.cn/gtbwxdayxl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.guowangkeji.top/gtowblshvu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.dianchejie.cn/gtxpwqgaue.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gotoacloud.top/gturegvgls.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yvedp.cn/gtblalbwiw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.kuanghao11.cn/gtbmpxnmha.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhixingplan.top/gtfrkiuxhc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.nanxinkj.top/gtenjouawu.html

[B04] for 计数循环
来源：http://hz.chenjidiqi.icu/gtvgrbpqcp.html

Py:   for i in range(10): print(i)
来源：http://hz.sysykeji.top/gtzlywtism.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jqgfzy.top/gtxgycavvl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hywenlv.cn/gtxokwprlz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.mhx1999.top/gtisjzhqoi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jyoumei.cn/gtvdaebvgi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hongshengwenyu.top/gtmljghyux.html

Ruby: 10.times { |i| puts i }
来源：http://hz.dianchejie.cn/gtdpjljbch.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.gogol.net.cn/gtotyfuorw.html

[B05] 遍历数组 / 列表
来源：http://hz.jianghu66.top/gtmaxtpmeu.html

Py:   for item in arr: print(item)
来源：http://hz.yvedp.cn/gtqjdamjit.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.aibaodan.cn/gtynwsufsp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hongshengwenyu.top/gtkrbjdvtr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jqgufenzy.top/gtigjaxwab.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.mhx1999.top/gtebltwygs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jlsjyb.cn/gtxjhinuzg.html

Ruby: arr.each { |item| puts item }
来源：http://hz.fzhhl.top/gtuovtrbue.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.tanke756.top/gtsseysyri.html

[B06] 遍历字典 / 对象
来源：http://hz.sweek.top/gtzkbbgqxk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.kuanghao11.cn/gtwgtxkpix.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.sweek.top/gtokhoplqt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.andypj.xyz/gtldfhgaoj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xingfuxueyuan.xyz/gtujvqdqof.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.xylfe.cn/gtgmswzuwb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.gaohongyu789.top/gtqsnouvfs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jinqigfzy.top/gtrbxahofe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.ehwqpu.com/gtpbavlkea.html

[B07] while 循环
来源：http://hz.9152youxi.cn/gtgjfeenru.html

Py:   while i < 10: i += 1
来源：http://hz.zhengqikj.top/gtamogkydh.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yuxming.cn/gtensydmjn.html

JS:   while (i < 10) { i++; }
来源：http://hz.mhx1999.top/gtdnqtnbsz.html

TS:   while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtsfsbluvl.html

Java: while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtutkrcvzs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hammf.cn/gtqvcnewvg.html

Ruby: while i < 10; i += 1; end
来源：http://hz.sweek.top/gtvhntocyz.html

C#:   while (i < 10) { i++; }
来源：http://hz.shangyingyoupin.top/gtnueqnyei.html

[B08] do-while（至少执行一次）
来源：http://hz.316326.xyz/gtiszjbcba.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.mhx1999.top/gtrlykcnbx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jlsjyb.cn/gtcbcjacvi.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtuucdmomq.html

TS:   do { i++; } while (i < 10);
来源：http://hz.daxiang520.top/gtmjpnzndj.html

Java: do { i++; } while (i < 10);
来源：http://hz.feifeiyinyue.top/gtbxszjreb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hnxiangtu.top/gtcozprjut.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xuetiantiany.cn/gtutpuujdp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gtiedayzrp.html

[B09] break 与 continue
来源：http://hz.yuanzhike.top/gtjgjkqqje.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jqgufenzy.top/gtzaqxywqd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtfgfoenxx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgfzy.top/gtloupogeg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydzc1.top/gtotbvtepk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtvimncyql.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhongyouzk.top/gtusxusifj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cqqwz.cn/gtlgspgitb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtlmyovwte.html

[B10] 遍历同时拿索引
来源：http://hz.sweek.top/gteufcxjrp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.316326.xyz/gtrgowsnsr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yj202588.top/gttlumxqlg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.andypj.xyz/gthidaeikw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shanyushiyangkeji.top/gtwlzitnan.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.haohaochexian.top/gtyhggxabi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.sweek.top/gtdgovcdez.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.guowangkeji.top/gtmksajvok.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yuanzhike.top/gtnitzrmbw.html

[B11] 生成数字序列 / 区间
来源：http://hz.shanyushiyangkeji.top/gtnvkwussd.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj20258.top/gtqvbehztq.html

PHP:  range(0, 10, 2);
来源：http://hz.cdnleiting.top/gtrjkymboa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shanyushiyangtech.top/gtjtjbswaz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.mhx1999.top/gtbynhomcy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yuxming.cn/gtfdtoocyn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.feifeiyinyue.top/gtxfhzyvcs.html

Ruby: (0...10).step(2).to_a
来源：http://hz.meibo888.top/gtsifsweyr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.gotoacloud.top/gtldyivldz.html

[B12] 跳出多层循环
来源：http://hz.jinyuanbaomall.cn/gtbzuvtvea.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.cashguo.top/gtegqoxgqu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.smart0.xyz/gtxqzsdycs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xylfe.cn/gtuibqhjun.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yonumen.top/gtyzbwlfnd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yonumen.top/gtwnqaqgdw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guannengcc.top/gtzgmbpuke.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.birdmap.top/gteceedsoe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.aibaodan.cn/gtixaixmyt.html

[B13] 判断是否为数字
来源：http://hz.wangshuangyany.cn/gtwxyxhczf.html

Py:   isinstance(x, (int, float))
来源：http://hz.chenjidiqi.icu/gtxdgnaxlt.html

PHP:  is_numeric($x)
来源：http://hz.jinyuanbaomall.cn/gtqppbovqt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guowangkeji.top/gtzslzymaz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinqigufen.top/gtwpcsrtnx.html

Java: x instanceof Number
来源：http://hz.zhaomingkeji.xyz/gtisbaemyo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhixingplan.top/gtyfkahqbr.html

Ruby: x.is_a?(Numeric)
来源：http://hz.cdnleiting.top/gtiiyatpag.html

C#:   x is int or double or decimal
来源：http://hz.zhixingplan.top/gtbiuvwecp.html

[B14] 判断值是否在集合内
来源：http://hz.wangdashe.top/gtdnupcfpr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.meibo888.top/gtkmmdoaxd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenzaomai.com/gtgtucajza.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shuidangran.top/gtvnzlhqia.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.snrcjt.cn/gtallvdlpx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yonumen.top/gtceyzdzxg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.tianlin.xyz/gtvscgyhsr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cheryme.top/gtskfxauvr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.nanxuanxn.top/gtpuckrbbn.html

[B15] 布尔运算与取反
来源：http://hz.xziqi.cn/gtcoavedlh.html

Py:   a and b or not c
来源：http://hz.ivvv.top/gtwzfzmyxb.html

PHP:  $a && $b || !$c
来源：http://hz.tanke756.top/gtfgtlhfth.html

JS:   a && b || !c
来源：http://hz.gotoacloud.top/gtsnevpdaj.html

TS:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtesufxmwq.html

Java: a && b || !c
来源：http://hz.bjfxy.top/gtscufgukt.html

Go:   a && b || !c
来源：http://hz.meibo888.top/gtfxhswtsw.html

Ruby: a && b || !c
来源：http://hz.smart0.xyz/gtuidkmhia.html

C#:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtjfpijeip.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yuanzhike.top/gtwijwwjxq.html

Py:   if not data: return
来源：http://hz.fengsongda.top/gtjucqsahm.html

PHP:  if (!$data) { return; }
来源：http://hz.xuetiantiany.cn/gtdilroepb.html

JS:   if (!data) return;
来源：http://hz.jqgufenzy.top/gtlymikdko.html

TS:   if (!data) return;
来源：http://hz.zhixingplan.top/gtzzovofkf.html

Java: if (data == null) return;
来源：http://hz.sxryk.cn/gtclrwwuro.html

Go:   if data == nil { return }
来源：http://hz.yj20258888.top/gtfmspmcoe.html

Ruby: return if data.nil?
来源：http://hz.andypj.xyz/gtcvilyzse.html

C#:   if (data == null) return;
来源：http://hz.hywenlv.cn/gtrtotudei.html

================================================================================
来源：http://hz.yonumen.top/gtgxovjtbn.html

C. 函数与作用域
来源：http://hz.pycfn.com/gtkoqooztp.html

================================================================================
来源：http://hz.sweek.top/gtwywwgedi.html

[C01] 定义函数
来源：http://hz.xziqi.cn/gthskqwxss.html

Py:   def add(a, b): return a + b
来源：http://hz.guowangkeji.top/gtgpjbycii.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhixingplan.top/gtfznpldju.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtbqyyuvjm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gtvdvyyetb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gteqsuhqms.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jianghu66.top/gtypfxrpsx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenzaomai.com/gtnmtxdomp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jqgufenzy.top/gtlshvgwmz.html

[C02] 默认参数
来源：http://hz.yuxming.cn/gtecefptyd.html

Py:   def greet(name="World"): return name
来源：http://hz.feifeiyinyue.top/gtgrmpgjwl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shanyushiyangkeji.top/gtyijxjkji.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jiagoushi.top/gtaoolerlx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhixingplan.top/gtzfwhpsqm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shangyingyoupin.top/gtimbrpwyt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yueranfly.top/gtdwlanhyz.html

Ruby: def greet(name = "World") = name
来源：http://hz.0kj1m.cn/gtunzpgbbx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tianlin.xyz/gtxeukvljr.html

[C03] 可变参数
来源：http://hz.yuanzhike.top/gtwrcfpspo.html

Py:   def total(*args): return sum(args)
来源：http://hz.cheryme.top/gtpdzrapge.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ybcxt.top/gtuuywdims.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangtech.top/gtyrathexg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sweek.top/gtltkzienv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jiagoushi.top/gtfjjhljrf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cucudq.cn/gtbxdngmrq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.mhx1999.top/gtynfbtfbe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xylfe.cn/gtmrwlnofl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cheryme.top/gtrrwscnrp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jyoumei.cn/gtgcnmxqfu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhongyouzk.top/gtusisngre.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hongshengwenyu.top/gtwhqusfyg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yueranfly.top/gtuefwzlvu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.nanxinkj.top/gtbjcvzuot.html

Go:   // 无：用配置结构体参数
来源：http://hz.haohaochexian.top/gtuvwfabhb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sysykeji.top/gtaxikudbm.html

C#:   f(a: 1, b: 2)
来源：http://hz.aibaodan.cn/gtgaqmgxhi.html

[C05] 返回多个值
来源：http://hz.zhengqikj.top/gturpbdhnh.html

Py:   return a, b
来源：http://hz.gotoacloud.top/gtnntfnocy.html

PHP:  return [$a, $b];
来源：http://hz.andypj.xyz/gtqtmqvcsp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinyuanbaomall.cn/gthprdmkyy.html

TS:   return { a, b };
来源：http://hz.bjfxy.top/gtrulkuzzg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shangyingyoupin.top/gtloxpprwq.html

Go:   return a, b
来源：http://hz.nanxuanxn.top/gtkduotexk.html

Ruby: return a, b
来源：http://hz.yonumen.top/gtuejoqvmr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yangfankeji.com/gtxfghexhs.html

[C06] 匿名函数 / lambda
来源：http://hz.daria6918.cn/gtfoypxhod.html

Py:   square = lambda x: x * x
来源：http://hz.ywan-chungtsiang.top/gtfmsykbbq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.kuanghao11.cn/gtcbdeownc.html

JS:   const square = x => x * x;
来源：http://hz.yuxming.cn/gtfwrnfuar.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yuanzhike.top/gtvqvaimxq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.pengpengdd.cyou/gtytmgvyvw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.aibaodan.cn/gtrtekntiy.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hnqzz.top/gtlvsavbcz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.52xcode.cn/gtlhsrzmdm.html

[C07] 把函数作为参数传入
来源：http://hz.snrcjt.cn/gtztguuzsu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.vqdsnc.cn/gtabwokzlq.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.wangdashe.top/gtdnfbwvnw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sysykeji.top/gtrgiwczsj.html

TS:   arr.map(String)
来源：http://hz.hnqzz.top/gtxdxaaqwp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.tian-w.cn/gtputfbhpk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.haohaochexian.top/gtlmyscjjz.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhaomingkeji.xyz/gtarhjksbw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fengsongda.top/gtfndpfvza.html

[C08] 闭包
来源：http://hz.yueranfly.top/gtkxyakvjh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zdqjudy.top/gthmmwchev.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.birdmap.top/gtvuqruihc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yanxiufei.cn/gtaonlnvni.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtosdougsb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.mhx1999.top/gtlhsetapa.html


<!-- 参考信息 -->