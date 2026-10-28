代发 wailian999

Ruby: value = data || "默认值"
来源：http://hz.jianghu66.top/gtdvdmymvn.html

C#:   var value = data ?? "默认值";
来源：http://hz.cucudq.cn/gtjgdmhjqa.html

[A16] 真假值判断规则
来源：http://hz.aibaodan.cn/gtohbpzbge.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.jinqigufen.top/gtkzooeyst.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.vqdsnc.cn/gtqwbkmdzv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.cdnleiting.top/gtsfsuowyz.html

TS:   if (!x) {}
来源：http://hz.ydjk.org.cn/gtpfuciawu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.ppjwa.cn/gttmtkfobq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jinyuanbaomall.cn/gtasxjlkyy.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.bjfxy.top/gtlmaucfiw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.sweek.top/gtlwrbugeu.html

[A17] 位运算
来源：http://hz.ivvv.top/gtcwskippl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydzc1.top/gtnizccprk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.52xcode.cn/gtldmxbzwa.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sweek.top/gtollmislu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.yueranfly.top/gtkzqjkuzj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gtcuobfjve.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zdqjudy.top/gtabzaeeuj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinqigufen.top/gthvughuui.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtnkdcdojf.html

[A18] 字符与 ASCII 码互转
来源：http://hz.chenjidiqi.icu/gtjzfdzgsd.html

Py:   ord("A"); chr(65)
来源：http://hz.hnxiangtu.top/gtkhftqmtw.html

PHP:  ord("A"); chr(65)
来源：http://hz.yj20258888.top/gtgitwailq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.dianchejie.cn/gtcwrrumsb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.andypj.xyz/gtyrcehjvx.html

Java: (int) 'A'; (char) 65
来源：http://hz.shuidangran.top/gtazbfqiof.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.jlsjyb.cn/gtapdggazi.html

Ruby: "A".ord; 65.chr
来源：http://hz.yuxming.cn/gtsfcrfkkx.html

C#:   (int)'A'; (char)65
来源：http://hz.zhijiandao.cn/gtatxlgxbv.html

[A19] 交换两个变量
来源：http://hz.gzhubu.top/gthvuycgea.html

Py:   a, b = b, a
来源：http://hz.aibaodan.cn/gtjqdfnthe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.havefunace.top/gtqznmrhvs.html

JS:   [a, b] = [b, a];
来源：http://hz.snrcjt.cn/gtipxzbdfv.html

TS:   [a, b] = [b, a];
来源：http://hz.chenlongwang.top/gtuigxeupy.html

Java: int t = a; a = b; b = t;
来源：http://hz.chenzaomai.com/gtnzdgpwrv.html

Go:   a, b = b, a
来源：http://hz.zhaomingkeji.xyz/gtvplxicqj.html

Ruby: a, b = b, a
来源：http://hz.andypj.xyz/gttmwxeffs.html

C#:   (a, b) = (b, a);
来源：http://hz.ppjwa.cn/gtyavhmcya.html

[A20] 读取标准输入
来源：http://hz.jinghuilouyu.cn/gtloxqodqj.html

Py:   name = input("请输入：")
来源：http://hz.yueranfly.top/gtdnyfcpyf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.hywenlv.cn/gtvvayycev.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.jianghu66.top/gtawbwgxkk.html

TS:   // Node.js：readline 模块
来源：http://hz.yangfankeji.com/gtjzbldspv.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.haohaochexian.top/gtzvruidbg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.hammf.cn/gtayyxldkt.html

Ruby: gets.chomp
来源：http://hz.yuxming.cn/gtzugakrsb.html

C#:   Console.ReadLine();
来源：http://hz.zhongyouzk.top/gtqmgnxhrx.html

[A21] 保留指定小数位输出
来源：http://hz.ivvv.top/gtacudhmco.html

Py:   f"{3.14159:.2f}"
来源：http://hz.bjfxy.top/gtzwzlhyky.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.yj202588.top/gtjznesszt.html

JS:   (3.14159).toFixed(2)
来源：http://hz.meibo888.top/gtjgnuyova.html

TS:   (3.14159).toFixed(2)
来源：http://hz.shzxlz.cn/gtfjxflmly.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ivvv.top/gtrcolyfsy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.mhx1999.top/gtjxzqjuue.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.gotoacloud.top/gtuksxssxx.html

C#:   3.14159.ToString("F2")
来源：http://hz.hfpthk.cn/gtxjmhiqbh.html

[A22] 获取字符串长度
来源：http://hz.havefunace.top/gtanhrsnzx.html

Py:   len(s)
来源：http://hz.cdnleiting.top/gtwtqyrnww.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.0kj1m.cn/gtdsegedvn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.ppjwa.cn/gtopfbxnra.html

TS:   s.length
来源：http://hz.52xcode.cn/gtxibpswib.html

Java: s.length()
来源：http://hz.wangshuangyany.cn/gtqsuzkscp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.andypj.xyz/gtlcznedwj.html

Ruby: s.length
来源：http://hz.chenlongwang.top/gtvwxnzitj.html

C#:   s.Length
来源：http://hz.zhoulong.xyz/gtunzsthfr.html

[A23] 大小写转换
来源：http://hz.wangdashe.top/gtphizgfqf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.tanke756.top/gtfzwhmbbq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.gzhubu.top/gthwctpfih.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zdqjudy.top/gtcossabyy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jinqigfzy.top/gtahoornqx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yangfankeji.com/gtntoaryns.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.zhiwuduotai.top/gtmvadukrw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zycfv.cn/gtqxwmtgto.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.cashguo.top/gthbvsgflv.html

[A24] 去除首尾空白
来源：http://hz.shzxlz.cn/gtmpdbwomf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yvedp.cn/gtzrwxcebz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.zhaomingkeji.xyz/gtsvjpgcyi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.fzhhl.top/gtiwdxhmtm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.pycfn.com/gtqhyohqps.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.aizwys.cn/gtxlpgpbbk.html

Go:   strings.TrimSpace(s)
来源：http://hz.sufxvd.cn/gttnjhdsup.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zhaomingkeji.xyz/gtsswfmxgy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.guannengcc.top/gtmfhpfldz.html

[A25] 字符串比较
来源：http://hz.jqgufenzy.top/gtacslpwge.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jinghuilouyu.cn/gtwulkqqmw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.pengpengdd.cyou/gtlyxxyyaz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jqgufenzy.top/gtikudlvln.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jiagoushi.top/gthbfmvuan.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.aizwys.cn/gtojtqmlui.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.shanyushiyangtech.top/gttxyydkdj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jinyuanbaomall.cn/gtvfwixgve.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.daria6918.cn/gtksnvqhsc.html

[A26] 类型转换总览
来源：http://hz.feifeiyinyue.top/gtitaiamcn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.bjfxy.top/gtywdigojz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.tanke756.top/gtlbkqxocz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.cdnleiting.top/gtyqvcpwer.html

TS:   Number() String() Boolean() x as number
来源：http://hz.fengsongda.top/gtxknpiacp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.redwolf501.top/gtwkyztzkd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.svipenyu.cn/gtgrqdsyxr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.52xcode.cn/gtuiiqwzsj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.gogol.net.cn/gtucdeupvh.html

================================================================================
来源：http://hz.yangfankeji.com/gtwgvkesfk.html

B. 流程控制
来源：http://hz.cheryme.top/gtqekvonaw.html

================================================================================
来源：http://hz.yj202588.top/gtpdzihtno.html

[B01] 条件判断 if / else
来源：http://hz.ehwqpu.com/gtptiyiozc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zhaomingkeji.xyz/gthjepamwf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.fzhhl.top/gtyanhnsfb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xziqi.cn/gtcyfwxugl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hywenlv.cn/gtcqwiyjkp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.guannengcc.top/gtgwvrdcil.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.xziqi.cn/gtqlpcibxq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jqgfzy.top/gtnvjiwhmk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.dashuyun.cn/gtkglmuhvb.html

[B02] 多分支 else if / elif
来源：http://hz.aizwys.cn/gtqyuhhfdp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.gzhubu.top/gtzssgnehq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.meibo888.top/gttjaamozj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.vqdsnc.cn/gtqrjqrula.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.kuanghao11.cn/gtnmtivqgy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.c1oappe.top/gtqqeucylo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.ywan-chungtsiang.top/gttddlvlbo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinqigufen.top/gtcpcllcyj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sufxvd.cn/gtkmhidmdm.html

[B03] switch / match / case
来源：http://hz.52xcode.cn/gtnbfbcwzc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.chenjidiqi.icu/gtfuzhbxry.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jyoumei.cn/gtdroxyqns.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.daxiang520.top/gtwhrjtqki.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hammf.cn/gtvvhzbajv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.chenlongwang.top/gtgegnsvtg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.chenzaomai.com/gtsrbjtowt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ybcxt.top/gtlzgjrsxr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jianghu66.top/gtugeslmie.html

[B04] for 计数循环
来源：http://hz.gzhubu.top/gtxhhltpbl.html

Py:   for i in range(10): print(i)
来源：http://hz.yj202588.top/gtyevjapif.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yongpay.top/gtybuikkla.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhaomingkeji.xyz/gtecxlmadx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.snrcjt.cn/gtslnbrxde.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ybcxt.top/gtcugroqrq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ybcxt.top/gttsvqhetj.html

Ruby: 10.times { |i| puts i }
来源：http://hz.mhx1999.top/gtohkdsxds.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.smart0.xyz/gttwxrmcqv.html

[B05] 遍历数组 / 列表
来源：http://hz.guowangkeji.top/gtywalsmhe.html

Py:   for item in arr: print(item)
来源：http://hz.tanke756.top/gtcuqhuwjz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.quarkkingdee.top/gtsodqxqgo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.cdnleiting.top/gtchqrirfd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xuetiantiany.cn/gtschncjmd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jinqigfzy.top/gttsfkxdha.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.kuanghao11.cn/gtjwwedezt.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yueranfly.top/gtpfbywzqh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yangfankeji.com/gtyapjtulp.html

[B06] 遍历字典 / 对象
来源：http://hz.fzhhl.top/gtuczrnidh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jyoumei.cn/gtgzxnches.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.meibo888.top/gtkdavuzwj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.fengsongda.top/gtxrdlxboh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xylfe.cn/gtlxzqrkhm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhengqikj.top/gtbpfpehuo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.tianlin.xyz/gttitldksx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhixingplan.top/gtznbxsafh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.fengsongda.top/gtpfhhvyau.html

[B07] while 循环
来源：http://hz.jiagoushi.top/gtffwzkbck.html

Py:   while i < 10: i += 1
来源：http://hz.nwbrower.top/gtavepuczp.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.cashguo.top/gtplwcveau.html

JS:   while (i < 10) { i++; }
来源：http://hz.52xcode.cn/gtqewgsvqd.html

TS:   while (i < 10) { i++; }
来源：http://hz.meibo888.top/gtcktexmpn.html

Java: while (i < 10) { i++; }
来源：http://hz.jinqigfzy.top/gtpmxdpxym.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.feifeiyinyue.top/gtweiwnlgp.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ybcxt.top/gtildwfytf.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhixingplan.top/gtrbafhlwi.html

[B08] do-while（至少执行一次）
来源：http://hz.tanke756.top/gtfcpyiwkm.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yj202588.top/gtcgntzqgn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yj20258888.top/gteejvstdw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.nanxuanxn.top/gtrpkdgjnd.html

TS:   do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtrxkoojpv.html

Java: do { i++; } while (i < 10);
来源：http://hz.yuanzhike.top/gtlhxpglst.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hnqzz.top/gtuhblpulg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.daria6918.cn/gtkccbecfs.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jinqigfzy.top/gtqnjdjbdd.html

[B09] break 与 continue
来源：http://hz.nanxuanxn.top/gtbjwuxcma.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ybcxt.top/gtvkxpsrfq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.mhx1999.top/gthssebhgw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hysaishi.cn/gtzynkotog.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gotoacloud.top/gtxhfqdocp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.c1oappe.top/gtzdjjbymr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.shuidangran.top/gtdprncajc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xuetiantiany.cn/gtycafnute.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pycfn.com/gtiudsqmih.html

[B10] 遍历同时拿索引
来源：http://hz.yuxming.cn/gtihovhowp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.wangshuangyany.cn/gtydfwlqwz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.316326.xyz/gtvlbnczjp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.birdmap.top/gtcwdjimet.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.kuanghao11.cn/gtazcajtmp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ywan-chungtsiang.top/gtwptuscjh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.daxiang520.top/gtwwwkvyso.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xinyue.icu/gtnbjpukuo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sxryk.cn/gtlqqvcjye.html

[B11] 生成数字序列 / 区间
来源：http://hz.xuetiantiany.cn/gtyvlfmtkj.html

Py:   list(range(0, 10, 2))
来源：http://hz.hywenlv.cn/gtwfucjyqu.html

PHP:  range(0, 10, 2);
来源：http://hz.xuanzx.com/gtarehlxgb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhengqikj.top/gtmdvjkjas.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hysaishi.cn/gtduoozdhh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.chenjidiqi.icu/gtmrplsxeh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.sxryk.cn/gtndwrowcw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ehwqpu.com/gtjqtzuzds.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jqgfzy.top/gtjzloqods.html

[B12] 跳出多层循环
来源：http://hz.hywenlv.cn/gtarckwmlv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shanyushiyangkeji.top/gtbxrjppvl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yuanzhike.top/gthqcofscj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.aibaodan.cn/gtccbhtfju.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhengqikj.top/gtxykuoilb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ybcxt.top/gtjiczckey.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xuetiantiany.cn/gtvovtobug.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cheryme.top/gtcuojvybn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shanyushiyangkeji.top/gtjpybbrlt.html

[B13] 判断是否为数字
来源：http://hz.cashguo.top/gtlqzdjxci.html

Py:   isinstance(x, (int, float))
来源：http://hz.ydjk.org.cn/gtfbljccxm.html

PHP:  is_numeric($x)
来源：http://hz.chenjidiqi.icu/gtpktgrzcr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gotoacloud.top/gtpfjoqqyn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cdnleiting.top/gtrvpkhsfo.html

Java: x instanceof Number
来源：http://hz.zhongyouzk.top/gtanfunang.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.tianlin.xyz/gtkxuzhxjw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.redwolf501.top/gtjzimiphx.html

C#:   x is int or double or decimal
来源：http://hz.haohaochexian.top/gtwfdoojuj.html

[B14] 判断值是否在集合内
来源：http://hz.kuanghao11.cn/gtsvkcbtbh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.andypj.xyz/gtxqkfxncs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.redwolf501.top/gtdobubycn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hongshengwenyu.top/gtafvzjwbr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yuanzhike.top/gtelhwumig.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jlsjyb.cn/gtbhfsglco.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.smart0.xyz/gtyycjiayo.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sxryk.cn/gtyfuprtlh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.redwolf501.top/gtsywazwqq.html

[B15] 布尔运算与取反
来源：http://hz.jinqigufen.top/gtxjisorew.html

Py:   a and b or not c
来源：http://hz.sxryk.cn/gtpflkzxla.html

PHP:  $a && $b || !$c
来源：http://hz.jqgfzy.top/gtgoslpkxd.html

JS:   a && b || !c
来源：http://hz.sxryk.cn/gtsjtwvild.html

TS:   a && b || !c
来源：http://hz.xziqi.cn/gtsbmjhwwx.html

Java: a && b || !c
来源：http://hz.cdnleiting.top/gtvllzopej.html

Go:   a && b || !c
来源：http://hz.zhengqikj.top/gtkbzalwge.html

Ruby: a && b || !c
来源：http://hz.andypj.xyz/gtqflynejh.html

C#:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtuebmtnvz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shanyushiyangkeji.top/gtlljbwfsk.html

Py:   if not data: return
来源：http://hz.yj20258.top/gtbzknbagn.html

PHP:  if (!$data) { return; }
来源：http://hz.xuetiantiany.cn/gtgyndcisi.html

JS:   if (!data) return;
来源：http://hz.zhongyouzk.top/gtjhtzfmlw.html

TS:   if (!data) return;
来源：http://hz.9152youxi.cn/gtnoipmaax.html

Java: if (data == null) return;
来源：http://hz.sysykeji.top/gtbksgupgf.html

Go:   if data == nil { return }
来源：http://hz.mhx1999.top/gtpltaolez.html

Ruby: return if data.nil?
来源：http://hz.gogol.net.cn/gtavyckhwb.html

C#:   if (data == null) return;
来源：http://hz.svipenyu.cn/gtdaevxddf.html

================================================================================
来源：http://hz.nwbrower.top/gtbqylkijw.html

C. 函数与作用域
来源：http://hz.0kj1m.cn/gtlhitglvl.html

================================================================================
来源：http://hz.chenzaomai.com/gtbcyuqkjh.html

[C01] 定义函数
来源：http://hz.yongpay.top/gtlpvmawym.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxinkj.top/gticbrwoon.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtzlippcky.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.316326.xyz/gttimrpxpp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gzhubu.top/gtgnbcnexw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gtotdhurog.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pengpengdd.cyou/gtowulrdph.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhongyouzk.top/gtjbtregjy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gtxqyxkuan.html

[C02] 默认参数
来源：http://hz.zhijiandao.cn/gtectmzoms.html

Py:   def greet(name="World"): return name
来源：http://hz.pengpengdd.cyou/gtlabfdjwr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cucudq.cn/gtayvdtioo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtamzrmzyq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhiwuduotai.top/gtwvxkytsj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.redwolf501.top/gttovujgrf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.nanxinkj.top/gtrjebotlw.html

Ruby: def greet(name = "World") = name
来源：http://hz.dashuyun.cn/gttubwshrw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhengqikj.top/gtwluwyvgx.html

[C03] 可变参数
来源：http://hz.mhx1999.top/gtnepvwgqp.html

Py:   def total(*args): return sum(args)
来源：http://hz.gzhubu.top/gtribpasbr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.fengsongda.top/gttgygxone.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yonumen.top/gtetzqwcrj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gteyajyuwv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhiwuduotai.top/gtpbbxafkj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ydzc1.top/gtbxmytuni.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sweek.top/gtwychljcs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hammf.cn/gtiqqffbwm.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xuanzx.com/gtwgfxxowe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.aibaodan.cn/gtxjyfxawp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.fzhhl.top/gtnqcnpspw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.dashuyun.cn/gtiiiofkie.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cqqwz.cn/gtwgcwrqrj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yangfankeji.com/gtcaalbohs.html

Go:   // 无：用配置结构体参数
来源：http://hz.guannengcc.top/gtfvxyegsg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xinyue.icu/gtlbkjfvjy.html

C#:   f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gtrckuajqi.html

[C05] 返回多个值
来源：http://hz.cdnleiting.top/gttqvzctsu.html

Py:   return a, b
来源：http://hz.meibo888.top/gtieuhqnzi.html

PHP:  return [$a, $b];
来源：http://hz.yuxming.cn/gtsvgupfwk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.mhx1999.top/gtaeguvpuc.html

TS:   return { a, b };
来源：http://hz.yj202588.top/gtssyycegs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xingfuxueyuan.xyz/gttfswbfqq.html

Go:   return a, b
来源：http://hz.xuanzx.com/gtkdbecdoc.html

Ruby: return a, b
来源：http://hz.pycfn.com/gtciwrmptc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guowangkeji.top/gtipndayjx.html

[C06] 匿名函数 / lambda
来源：http://hz.fengsongda.top/gtxneorfud.html

Py:   square = lambda x: x * x
来源：http://hz.xingfuxueyuan.xyz/gtnmuicijb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.fengsongda.top/gtuaelrfua.html

JS:   const square = x => x * x;
来源：http://hz.cucudq.cn/gtgbmywedu.html


<!-- 参考信息 -->