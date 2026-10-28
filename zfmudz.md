代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.ybcxt.top/gtuxiqfjmz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.cashguo.top/gtwzwecast.html

TS:   if (!x) {}
来源：http://hz.chenlongwang.top/gtxyjzasob.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yvedp.cn/gtncoxuoir.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.havefunace.top/gtffvriegi.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.jqgfzy.top/gtmzfyykpv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.hfpthk.cn/gtjpldtsgk.html

[A17] 位运算
来源：http://hz.sufxvd.cn/gtvribxvjn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xinyue.icu/gtwmjhwadk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.zhaomingkeji.xyz/gthdgscxni.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.meibo888.top/gtjcwpzeqv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.yueranfly.top/gtebgarzbg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hammf.cn/gtsrplxvzy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.hammf.cn/gtshllfppk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cqqwz.cn/gtonqydjii.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.daxiang520.top/gthqzsztvm.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jqgfzy.top/gtgtfgdgrh.html

Py:   ord("A"); chr(65)
来源：http://hz.wangdashe.top/gtfzzxmzls.html

PHP:  ord("A"); chr(65)
来源：http://hz.dashuyun.cn/gtgjfrvflw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yongpay.top/gtzlpsyzol.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.tian-w.cn/gtycjtdawc.html

Java: (int) 'A'; (char) 65
来源：http://hz.zhijiandao.cn/gtsevheatz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.52xcode.cn/gtfrinbymy.html

Ruby: "A".ord; 65.chr
来源：http://hz.yvedp.cn/gtfuqglhvx.html

C#:   (int)'A'; (char)65
来源：http://hz.jqgufenzy.top/gtxclezoeu.html

[A19] 交换两个变量
来源：http://hz.hammf.cn/gtqhauujwh.html

Py:   a, b = b, a
来源：http://hz.yonumen.top/gtpphlmwpe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.hnqzz.top/gtclqxdtqa.html

JS:   [a, b] = [b, a];
来源：http://hz.yonumen.top/gtadyirqfi.html

TS:   [a, b] = [b, a];
来源：http://hz.xinyue.icu/gtrbqdqung.html

Java: int t = a; a = b; b = t;
来源：http://hz.dianchejie.cn/gtdsdjpnwq.html

Go:   a, b = b, a
来源：http://hz.zycfv.cn/gteuauzkef.html

Ruby: a, b = b, a
来源：http://hz.ehwqpu.com/gtawfhmdiw.html

C#:   (a, b) = (b, a);
来源：http://hz.andypj.xyz/gtrlnspfsf.html

[A20] 读取标准输入
来源：http://hz.shanyushiyangkeji.top/gtjqohppod.html

Py:   name = input("请输入：")
来源：http://hz.zhengqikj.top/gtmqerinac.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.nwbrower.top/gtwrfnbjew.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.iojbl.cn/gtbovnpnmy.html

TS:   // Node.js：readline 模块
来源：http://hz.hongshengwenyu.top/gtrhwdojgf.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.ppjwa.cn/gtpgahwkte.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.meibo888.top/gtizxvynzx.html

Ruby: gets.chomp
来源：http://hz.hnxiangtu.top/gtebrowfrz.html

C#:   Console.ReadLine();
来源：http://hz.cashguo.top/gthdmtzulh.html

[A21] 保留指定小数位输出
来源：http://hz.iojbl.cn/gtulzlpcgc.html

Py:   f"{3.14159:.2f}"
来源：http://hz.cheryme.top/gtqxmpzbuo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.zycfv.cn/gtmguiqfda.html

JS:   (3.14159).toFixed(2)
来源：http://hz.bjfxy.top/gtvlnidbyg.html

TS:   (3.14159).toFixed(2)
来源：http://hz.kuanghao11.cn/gtoxnfoagd.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.chenjidiqi.icu/gtxzmmgtrl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.shangyingyoupin.top/gtbodkbkgg.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yonumen.top/gtuypboeey.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhijiandao.cn/gtopktxnyc.html

[A22] 获取字符串长度
来源：http://hz.ywan-chungtsiang.top/gtveblzjkj.html

Py:   len(s)
来源：http://hz.kuanghao11.cn/gtalimnnfv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.zdqjudy.top/gtpkvlbwso.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.c1oappe.top/gteqlbwquu.html

TS:   s.length
来源：http://hz.zhoulong.xyz/gtrciazocm.html

Java: s.length()
来源：http://hz.hongshengwenyu.top/gtkacnpcxq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.hfpthk.cn/gteassibed.html

Ruby: s.length
来源：http://hz.316326.xyz/gtwngabvvv.html

C#:   s.Length
来源：http://hz.jinqigfzy.top/gtlryjpaex.html

[A23] 大小写转换
来源：http://hz.quarkkingdee.top/gtqnotuojk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.nwbrower.top/gtlxyyucvy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.aibaodan.cn/gtqilweygp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hongshengwenyu.top/gtenhaafsc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.dianchejie.cn/gttelazdws.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.xuetiantiany.cn/gtvnransva.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.shanyushiyangtech.top/gttdupcdhh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yj20258888.top/gtvoqdrrto.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.fzhhl.top/gtsrygnrgx.html

[A24] 去除首尾空白
来源：http://hz.smart0.xyz/gtttjooyac.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.shangyingyoupin.top/gthxbknuzk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yueranfly.top/gtfilogdsw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xingfuxueyuan.xyz/gtjuyrlbim.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hnxiangtu.top/gtmtohbsmk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.havefunace.top/gtqtrdggde.html

Go:   strings.TrimSpace(s)
来源：http://hz.jqgufenzy.top/gtwutvnplt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.dianchejie.cn/gturjqynkn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.ehwqpu.com/gttwiwvvdj.html

[A25] 字符串比较
来源：http://hz.yangfankeji.com/gtiollvssy.html

Py:   s1 == s2; s1 != s2
来源：http://hz.316326.xyz/gtkdauktic.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ppjwa.cn/gtbtbidvio.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinqigufen.top/gtvtinbapz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.316326.xyz/gtzsxdinob.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.xuanzx.com/gtjpetloyh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.gzhubu.top/gtgythnpqd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.birdmap.top/gttdpbclwo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.cashguo.top/gtkusfbjot.html

[A26] 类型转换总览
来源：http://hz.shzxlz.cn/gtcgcatwkq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.vqdsnc.cn/gtiwqhkjhh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xingfuxueyuan.xyz/gtywfwiqyh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.chenlongwang.top/gtvrvfsdoz.html

TS:   Number() String() Boolean() x as number
来源：http://hz.hongshengwenyu.top/gtswgzqmfc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhaomingkeji.xyz/gtziqcilqt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.andypj.xyz/gtdiutfkvy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.hfpthk.cn/gtigvwvadn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.tian-w.cn/gtcfrujjiq.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtbstnrvtk.html

B. 流程控制
来源：http://hz.jlsjyb.cn/gtyocqseza.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtlowdcnst.html

[B01] 条件判断 if / else
来源：http://hz.havefunace.top/gttuefkjtw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.birdmap.top/gtamzkslrr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.tanke756.top/gtsllbcgjc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.52xcode.cn/gtdoxjjnup.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.fengsongda.top/gtgouwnwhz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangkeji.top/gtriebnaap.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.chenjidiqi.icu/gtijorhbcs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jqgfzy.top/gtqewpwgto.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gtufyexell.html

[B02] 多分支 else if / elif
来源：http://hz.guannengcc.top/gtdutisaks.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.hongshengwenyu.top/gtgjhzqdse.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.redwolf501.top/gtujcvhogr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.aizwys.cn/gtmsmkzzqo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.aizwys.cn/gtnxjrmnpk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shanyushiyangkeji.top/gtdnneeslm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.wangshuangyany.cn/gtjrlkpppf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.daria6918.cn/gtndaolujz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yvedp.cn/gtvuxbbwft.html

[B03] switch / match / case
来源：http://hz.gogol.net.cn/gtkjredqza.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.gzhubu.top/gtaldezdsl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jinqigfzy.top/gthhmaccha.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jqgufenzy.top/gtmohipwsi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.tanke756.top/gtnytcuqkp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.shuidangran.top/gtycepeatv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.c1oappe.top/gtgfyckcir.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.chenjidiqi.icu/gtknovcdxe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.gogol.net.cn/gtmbhtqgky.html

[B04] for 计数循环
来源：http://hz.mhx1999.top/gtfzusyxsp.html

Py:   for i in range(10): print(i)
来源：http://hz.pycfn.com/gttkgqlgiw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.wangshuangyany.cn/gtrdrcsrcq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ehwqpu.com/gtjygaxsaa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xuetiantiany.cn/gthgfedivy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.cucudq.cn/gtgbyvkoyx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jyoumei.cn/gthkidsxpq.html

Ruby: 10.times { |i| puts i }
来源：http://hz.gogol.net.cn/gtpyfzilwr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.andypj.xyz/gtepvyybkw.html

[B05] 遍历数组 / 列表
来源：http://hz.ydzc1.top/gtboywvjkz.html

Py:   for item in arr: print(item)
来源：http://hz.zhongyouzk.top/gtrrvskqen.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hywenlv.cn/gtmdyqhdnz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.smart0.xyz/gtnxyjkwfa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.cashguo.top/gtkqxcepja.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.sufxvd.cn/gtvswpiiut.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ywan-chungtsiang.top/gtnpooulqe.html

Ruby: arr.each { |item| puts item }
来源：http://hz.birdmap.top/gtunzvwmnc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.gzhubu.top/gtvydqejdg.html

[B06] 遍历字典 / 对象
来源：http://hz.dianchejie.cn/gtrkkxotwk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.daxiang520.top/gtsguxkdtn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.shzxlz.cn/gtrerjhcve.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.mhx1999.top/gtdjsibjps.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.chenlongwang.top/gtkcikykay.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zycfv.cn/gteaynopno.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jqgfzy.top/gtgxpnrjwy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.chenzaomai.com/gtfvurjmcb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.guannengcc.top/gtzhxmyplz.html

[B07] while 循环
来源：http://hz.sxryk.cn/gtojhzljkc.html

Py:   while i < 10: i += 1
来源：http://hz.sweek.top/gtmhcrnjji.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.guannengcc.top/gthzghoeck.html

JS:   while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gtsuieplyz.html

TS:   while (i < 10) { i++; }
来源：http://hz.yj202588.top/gtdpwvftlo.html

Java: while (i < 10) { i++; }
来源：http://hz.jinqigufen.top/gtsxokwgpt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zdqjudy.top/gtdftvlilr.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xziqi.cn/gtqbabbjkn.html

C#:   while (i < 10) { i++; }
来源：http://hz.hammf.cn/gtcgptokbx.html

[B08] do-while（至少执行一次）
来源：http://hz.tanke756.top/gtcbzwvslz.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xuanzx.com/gtxcfqckih.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.xinyue.icu/gtzbfjatvz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ppjwa.cn/gtvbskhvlo.html

TS:   do { i++; } while (i < 10);
来源：http://hz.gotoacloud.top/gtlcyswceg.html

Java: do { i++; } while (i < 10);
来源：http://hz.andypj.xyz/gtaeueqsod.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.xylfe.cn/gtoqcfkyve.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xziqi.cn/gtnfjhlkon.html

C#:   do { i++; } while (i < 10);
来源：http://hz.fengsongda.top/gtyvniwaum.html

[B09] break 与 continue
来源：http://hz.gzhubu.top/gtspktwmhr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jianghu66.top/gtmmmfjbna.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtbblzkivd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuanzhike.top/gtzeexieyg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yanxiufei.cn/gtxcnpefxb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtnrasfxdb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhengqikj.top/gthddovehj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhijiandao.cn/gttekqwauk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtdjzucbnh.html

[B10] 遍历同时拿索引
来源：http://hz.shangyingyoupin.top/gtphducgdr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.mhx1999.top/gtwkhuwdfx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.feifeiyinyue.top/gtaeyhlafz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhijiandao.cn/gtmdnvizli.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.feifeiyinyue.top/gtlfhdbjun.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hongshengwenyu.top/gtvosnwgsm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.daxiang520.top/gtsiheolkk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jiagoushi.top/gtgqujhhjn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jianghu66.top/gtvwpzmwnb.html

[B11] 生成数字序列 / 区间
来源：http://hz.ydjk.org.cn/gtxwgjjbjp.html

Py:   list(range(0, 10, 2))
来源：http://hz.xylfe.cn/gtglafpywu.html

PHP:  range(0, 10, 2);
来源：http://hz.jinqigfzy.top/gtjauwrbmd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gogol.net.cn/gtkuelvwwl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.smart0.xyz/gtdvyqzjgs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ywan-chungtsiang.top/gtgweqaalo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cashguo.top/gtwigbmaug.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yj20258.top/gtgpwxgeqi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.svipenyu.cn/gtdtxonwhc.html

[B12] 跳出多层循环
来源：http://hz.hammf.cn/gtzdheraig.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hysaishi.cn/gtivgdmppi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hnxiangtu.top/gtpfzehktu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xziqi.cn/gtsfnxiazm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gtnfdjmcbl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.c1oappe.top/gtsngldzqs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.haohaochexian.top/gtrfxvheoe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gaohongyu789.top/gtuuyxsnlx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.havefunace.top/gtsmvwfesp.html

[B13] 判断是否为数字
来源：http://hz.ywan-chungtsiang.top/gtevubelxk.html

Py:   isinstance(x, (int, float))
来源：http://hz.chenlongwang.top/gtcqshjahd.html

PHP:  is_numeric($x)
来源：http://hz.yuxming.cn/gtrlqmeyue.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xylfe.cn/gtycrburph.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenlongwang.top/gtwihdgevh.html

Java: x instanceof Number
来源：http://hz.xziqi.cn/gtnzzgwdyi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.316326.xyz/gthqpviflp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.316326.xyz/gtfqrlpbwe.html

C#:   x is int or double or decimal
来源：http://hz.ydzc1.top/gtmwspbmlg.html

[B14] 判断值是否在集合内
来源：http://hz.guowangkeji.top/gtxvajdtno.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gogol.net.cn/gtmvwithmf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhiwuduotai.top/gtnabwcduw.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.feifeiyinyue.top/gthpyazaup.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gaohongyu789.top/gtuzuvarpx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.pycfn.com/gtuchszjhu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zdqjudy.top/gtloyrvdul.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sxryk.cn/gtawkfiiff.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.9152youxi.cn/gtnlufovws.html

[B15] 布尔运算与取反
来源：http://hz.316326.xyz/gtxxilssff.html

Py:   a and b or not c
来源：http://hz.yuxming.cn/gttbwfaubs.html

PHP:  $a && $b || !$c
来源：http://hz.zhijiandao.cn/gtghyennlg.html

JS:   a && b || !c
来源：http://hz.svipenyu.cn/gtisejajaq.html

TS:   a && b || !c
来源：http://hz.yj202588.top/gtlefaajaz.html

Java: a && b || !c
来源：http://hz.xylfe.cn/gtvkiluwio.html

Go:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtqncbohtv.html

Ruby: a && b || !c
来源：http://hz.hnxiangtu.top/gtdtthtnqy.html

C#:   a && b || !c
来源：http://hz.chenlongwang.top/gtsgylovxl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.kuanghao11.cn/gtgyyfguix.html

Py:   if not data: return
来源：http://hz.quarkkingdee.top/gtsyoxjbhn.html

PHP:  if (!$data) { return; }
来源：http://hz.yj202588.top/gtdtecreav.html

JS:   if (!data) return;
来源：http://hz.aizwys.cn/gtikevhouc.html

TS:   if (!data) return;
来源：http://hz.yj202588.top/gteqbxaznn.html

Java: if (data == null) return;
来源：http://hz.xingfuxueyuan.xyz/gtdbhrwkjn.html

Go:   if data == nil { return }
来源：http://hz.ehwqpu.com/gtmkpvqaja.html

Ruby: return if data.nil?
来源：http://hz.wangshuangyany.cn/gtusyakhly.html

C#:   if (data == null) return;
来源：http://hz.shanyushiyangtech.top/gtqccumgxt.html

================================================================================
来源：http://hz.daxiang520.top/gthlacqhgm.html

C. 函数与作用域
来源：http://hz.zhiwuduotai.top/gtlnctuqmb.html

================================================================================
来源：http://hz.ivvv.top/gtyqtphisx.html

[C01] 定义函数
来源：http://hz.bjfxy.top/gtinymqrxv.html

Py:   def add(a, b): return a + b
来源：http://hz.zhijiandao.cn/gtuugdiolk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jyoumei.cn/gtzudsqfqi.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hammf.cn/gthqpsjcrn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhoulong.xyz/gtxblnogzh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtijsnygbg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.quarkkingdee.top/gtoioueqas.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shanyushiyangkeji.top/gtpkhtnlhb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtqoxpdipv.html

[C02] 默认参数
来源：http://hz.shzxlz.cn/gtzijnrtso.html

Py:   def greet(name="World"): return name
来源：http://hz.hywenlv.cn/gtdhajygbj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sysykeji.top/gtrfiymwdr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shuidangran.top/gtatssjtel.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj202588.top/gtpfpewtxb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.redwolf501.top/gtifcbydwa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gaohongyu789.top/gtexawbsol.html

Ruby: def greet(name = "World") = name
来源：http://hz.xylfe.cn/gtpodgjttp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.kuanghao11.cn/gtmuidobyq.html

[C03] 可变参数
来源：http://hz.hammf.cn/gtjqnyylun.html

Py:   def total(*args): return sum(args)
来源：http://hz.tian-w.cn/gtualzzhwk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenlongwang.top/gtmjsxnmhy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinghuilouyu.cn/gttyeanvgq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dashuyun.cn/gtmzogvqrg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhoulong.xyz/gthyahpdsh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhoulong.xyz/gtzcurbrnj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yonumen.top/gtuucqyktt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.meibo888.top/gtlzapfmne.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shangyingyoupin.top/gtqbnctlai.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guannengcc.top/gtkegvlywr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhongyouzk.top/gtfnlpnrvc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hysaishi.cn/gtruozmcmi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zycfv.cn/gtczbhisve.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.feifeiyinyue.top/gteafrgsjx.html

Go:   // 无：用配置结构体参数
来源：http://hz.jqgfzy.top/gtjvhvadju.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jyoumei.cn/gtwhsruzna.html

C#:   f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtegbdnqbn.html

[C05] 返回多个值
来源：http://hz.dianchejie.cn/gtkiqnabmb.html

Py:   return a, b
来源：http://hz.aibaodan.cn/gtasbnsohb.html

PHP:  return [$a, $b];
来源：http://hz.smart0.xyz/gtwedwkiue.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.vqdsnc.cn/gtgeqfhreu.html

TS:   return { a, b };
来源：http://hz.bjfxy.top/gtrizyvfdw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinqigufen.top/gtgevajsgt.html

Go:   return a, b
来源：http://hz.hnxiangtu.top/gtuqiuxvkk.html

Ruby: return a, b
来源：http://hz.zhixingplan.top/gtrsdbeekq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.9152youxi.cn/gtleztqqml.html

[C06] 匿名函数 / lambda
来源：http://hz.zycfv.cn/gtjiwhysbx.html

Py:   square = lambda x: x * x
来源：http://hz.guannengcc.top/gtpiklccjz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tian-w.cn/gtevbkdybx.html

JS:   const square = x => x * x;
来源：http://hz.zhengqikj.top/gtwkeaicvb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.guowangkeji.top/gtthiyhrjz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hammf.cn/gtgugovtsq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yj202588.top/gtsopngptv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hywenlv.cn/gtsvbppenu.html


<!-- 参考信息 -->