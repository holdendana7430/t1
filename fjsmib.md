代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.xylfe.cn/gthadtinpy.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.ppjwa.cn/gtykuvcgmf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.jinghuilouyu.cn/gtsishizrz.html

[A17] 位运算
来源：http://hz.9152youxi.cn/gtszpzjnmp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.aibaodan.cn/gtgnytngle.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.jianghu66.top/gtzbxfavfl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.0kj1m.cn/gtjxysrwhk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.ywan-chungtsiang.top/gtpihnuapp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hongshengwenyu.top/gtnqemocae.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.smart0.xyz/gtvlimpwna.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yangfankeji.com/gtrggqvnks.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.9152youxi.cn/gtvfqmkczf.html

[A18] 字符与 ASCII 码互转
来源：http://hz.pengpengdd.cyou/gtyazolwsp.html

Py:   ord("A"); chr(65)
来源：http://hz.316326.xyz/gtgkfbmcls.html

PHP:  ord("A"); chr(65)
来源：http://hz.sxryk.cn/gtiaujvtwg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.aibaodan.cn/gtmxiswajk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.gotoacloud.top/gtvmduhtvy.html

Java: (int) 'A'; (char) 65
来源：http://hz.52xcode.cn/gtycehvyhq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.pycfn.com/gtngzspdzv.html

Ruby: "A".ord; 65.chr
来源：http://hz.zhoulong.xyz/gtmeqxrffc.html

C#:   (int)'A'; (char)65
来源：http://hz.pengpengdd.cyou/gtjtdfauet.html

[A19] 交换两个变量
来源：http://hz.nanxuanxn.top/gtbothqstc.html

Py:   a, b = b, a
来源：http://hz.jqgfzy.top/gtkhzfqlsn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.hammf.cn/gtfhrezerl.html

JS:   [a, b] = [b, a];
来源：http://hz.hnxiangtu.top/gtihfwccgb.html

TS:   [a, b] = [b, a];
来源：http://hz.sysykeji.top/gtnzormoaf.html

Java: int t = a; a = b; b = t;
来源：http://hz.hysaishi.cn/gtujjujmef.html

Go:   a, b = b, a
来源：http://hz.feifeiyinyue.top/gtpvustjyl.html

Ruby: a, b = b, a
来源：http://hz.fzhhl.top/gtzitaksnt.html

C#:   (a, b) = (b, a);
来源：http://hz.wangdashe.top/gtwapasrlb.html

[A20] 读取标准输入
来源：http://hz.bjfxy.top/gtoqpqvfsh.html

Py:   name = input("请输入：")
来源：http://hz.iojbl.cn/gtsovichwd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.dianchejie.cn/gtllkwahrw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.jinghuilouyu.cn/gtymahegpw.html

TS:   // Node.js：readline 模块
来源：http://hz.chenzaomai.com/gtrafigmyi.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yj202588.top/gtonshtwhb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.smart0.xyz/gtrbzlrpgg.html

Ruby: gets.chomp
来源：http://hz.52xcode.cn/gtghyhekku.html

C#:   Console.ReadLine();
来源：http://hz.hywenlv.cn/gtrqgmumzy.html

[A21] 保留指定小数位输出
来源：http://hz.sxryk.cn/gtjiuxyfih.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yueranfly.top/gtrkusvqys.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.jianghu66.top/gtaohwozpc.html

JS:   (3.14159).toFixed(2)
来源：http://hz.jinqigfzy.top/gttjachmkr.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jinyuanbaomall.cn/gtgfhkpbws.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.xinyue.icu/gtwxzkxspy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.wangshuangyany.cn/gtnvgzcaag.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.shanyushiyangtech.top/gtrxpnpgmg.html

C#:   3.14159.ToString("F2")
来源：http://hz.yj202588.top/gtgqpwcmur.html

[A22] 获取字符串长度
来源：http://hz.cashguo.top/gtrktjktch.html

Py:   len(s)
来源：http://hz.gzhubu.top/gtoyznoruf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.zhengqikj.top/gtunsawiht.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.cashguo.top/gtryorjucv.html

TS:   s.length
来源：http://hz.meibo888.top/gtuffgynyu.html

Java: s.length()
来源：http://hz.yanxiufei.cn/gtfjztdxof.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.cheryme.top/gteeutmuuh.html

Ruby: s.length
来源：http://hz.jinghuilouyu.cn/gtrtrghemj.html

C#:   s.Length
来源：http://hz.wangdashe.top/gtczmpfsxo.html

[A23] 大小写转换
来源：http://hz.0kj1m.cn/gtfxmpjzwz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yangfankeji.com/gthicovoxv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.cheryme.top/gtjpouspgi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xuetiantiany.cn/gtoymjpuvi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.tian-w.cn/gthkddvcmg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.jqgufenzy.top/gtstdtultb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.wangdashe.top/gtiixpfjei.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jinqigfzy.top/gtxhbfxtcf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.316326.xyz/gtnscasysr.html

[A24] 去除首尾空白
来源：http://hz.yueranfly.top/gtlyzxaxjy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.xuanzx.com/gtgduprvxc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.jqgufenzy.top/gtvthhquwe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yuxming.cn/gtenulrrwj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.pycfn.com/gtlikavbrs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.gaohongyu789.top/gtivvmonej.html

Go:   strings.TrimSpace(s)
来源：http://hz.ivvv.top/gtcvtyxwzk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jlsjyb.cn/gtrpiangqe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.hongshengwenyu.top/gttkvccnso.html

[A25] 字符串比较
来源：http://hz.hfpthk.cn/gtdmbpohxs.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jinqigufen.top/gtwcokmuup.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.shanyushiyangkeji.top/gtbrrbgbth.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.c1oappe.top/gteacaalcx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.cheryme.top/gtfctzdqmo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.tian-w.cn/gtfajgdnlh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yangfankeji.com/gtturhgofe.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.sufxvd.cn/gtbvixbsws.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.quarkkingdee.top/gtwggepwzz.html

[A26] 类型转换总览
来源：http://hz.cucudq.cn/gtpjzlrauu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.aibaodan.cn/gtlqkyjnux.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.kuanghao11.cn/gtpjadtusj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.316326.xyz/gtxdphukjl.html

TS:   Number() String() Boolean() x as number
来源：http://hz.gzhubu.top/gttkfotcel.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.haohaochexian.top/gtgfcvvftn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.chenjidiqi.icu/gtuljxqrpv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.gzhubu.top/gtoegtwhuk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ydjk.org.cn/gtnpesxswk.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtjptbousn.html

B. 流程控制
来源：http://hz.zhoulong.xyz/gtqapcltsf.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtutsqbpbv.html

[B01] 条件判断 if / else
来源：http://hz.sufxvd.cn/gtaucxdzxs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zdqjudy.top/gtrdtzrmlj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.tian-w.cn/gtvjpvzfty.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yongpay.top/gtedewkaox.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ivvv.top/gtqpxzfzsq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yueranfly.top/gtgakomrpq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ywan-chungtsiang.top/gtgftadrrl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yonumen.top/gthnbgsmba.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.0kj1m.cn/gtbmfkygky.html

[B02] 多分支 else if / elif
来源：http://hz.tanke756.top/gtbsrnhnyf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.ywan-chungtsiang.top/gtcrucojpw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yanxiufei.cn/gthdcfbkaw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pengpengdd.cyou/gthfloezvj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.kuanghao11.cn/gtoeziterw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gogol.net.cn/gtwhnctcuj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.aizwys.cn/gtzqxzcdui.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.cashguo.top/gtlrpqyjmp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tianlin.xyz/gtzwbhsnci.html

[B03] switch / match / case
来源：http://hz.gotoacloud.top/gtgmwpnvkl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jinyuanbaomall.cn/gtqomayuic.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.daria6918.cn/gtrymqacxq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.9152youxi.cn/gtjwhytywg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.nanxinkj.top/gtnfvgiaii.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.zhixingplan.top/gtauzajbie.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhaomingkeji.xyz/gtyfvcbrqc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.vqdsnc.cn/gtllqwwtgj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.gzhubu.top/gtgjqilcza.html

[B04] for 计数循环
来源：http://hz.jlsjyb.cn/gtwazcpxlh.html

Py:   for i in range(10): print(i)
来源：http://hz.yueranfly.top/gtqblhjetq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.pycfn.com/gtzyghxakx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gaohongyu789.top/gtijqlvgnu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.quarkkingdee.top/gtauospote.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.daria6918.cn/gtonlbfvut.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.bjfxy.top/gtssukupzw.html

Ruby: 10.times { |i| puts i }
来源：http://hz.havefunace.top/gtuwxltbvq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.c1oappe.top/gtucfmbrdd.html

[B05] 遍历数组 / 列表
来源：http://hz.zhongyouzk.top/gtnonxpehn.html

Py:   for item in arr: print(item)
来源：http://hz.daria6918.cn/gttajdeluo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ivvv.top/gtthpvlucg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.nwbrower.top/gttewbropg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xylfe.cn/gtgccmxido.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.52xcode.cn/gtayuruceu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.9152youxi.cn/gthufincsc.html

Ruby: arr.each { |item| puts item }
来源：http://hz.chenlongwang.top/gtospeiyku.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zdqjudy.top/gtrquqpbio.html

[B06] 遍历字典 / 对象
来源：http://hz.c1oappe.top/gtswegavrh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.hfpthk.cn/gtlxqawcrx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xingfuxueyuan.xyz/gtlionhrel.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.fzhhl.top/gtktsgbtgj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.aibaodan.cn/gtzlnkcfmz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.shangyingyoupin.top/gtgyuckccc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.nanxinkj.top/gtlcgwbvdm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.cashguo.top/gtsdeqwnxq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yanxiufei.cn/gtkcfheakt.html

[B07] while 循环
来源：http://hz.wangshuangyany.cn/gtmaiqyqfp.html

Py:   while i < 10: i += 1
来源：http://hz.yanxiufei.cn/gtumjafujj.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.gaohongyu789.top/gteogajprt.html

JS:   while (i < 10) { i++; }
来源：http://hz.0kj1m.cn/gtfuypsdeu.html

TS:   while (i < 10) { i++; }
来源：http://hz.xingfuxueyuan.xyz/gtfqbgrnqr.html

Java: while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtupfkiczj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ehwqpu.com/gttkzpexhk.html

Ruby: while i < 10; i += 1; end
来源：http://hz.9152youxi.cn/gtrnkimfqm.html

C#:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gtjpirvant.html

[B08] do-while（至少执行一次）
来源：http://hz.guowangkeji.top/gtitqdqskl.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hnxiangtu.top/gthbjvhswv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yangfankeji.com/gtwwijulya.html

JS:   do { i++; } while (i < 10);
来源：http://hz.aibaodan.cn/gtktfrajxr.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yanxiufei.cn/gttbjfttcb.html

Java: do { i++; } while (i < 10);
来源：http://hz.redwolf501.top/gthxolfdqh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.birdmap.top/gtzgbhbcuf.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.havefunace.top/gtkwwteamd.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xuanzx.com/gtgppmlloj.html

[B09] break 与 continue
来源：http://hz.xylfe.cn/gtytuiiiwz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.316326.xyz/gtzgbbqaiv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.smart0.xyz/gtzvqrceae.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gtwprtpjnl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.iojbl.cn/gtireoshrb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gthqsbhrfk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.snrcjt.cn/gtwsefvqce.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinyuanbaomall.cn/gttkgvuqli.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yvedp.cn/gtzurylpnl.html

[B10] 遍历同时拿索引
来源：http://hz.yanxiufei.cn/gttkooppwh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhixingplan.top/gtpuvvsaoe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cqqwz.cn/gtmyabpqlc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.0kj1m.cn/gtfbthiciv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.dianchejie.cn/gtknrkcpil.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.dianchejie.cn/gthhvemmcn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.daxiang520.top/gthqoplkir.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shangyingyoupin.top/gtwzhykzbv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.316326.xyz/gtulroyqvb.html

[B11] 生成数字序列 / 区间
来源：http://hz.iojbl.cn/gtkkmuqomr.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj20258888.top/gtjkzltyml.html

PHP:  range(0, 10, 2);
来源：http://hz.hysaishi.cn/gtqlmivekg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yonumen.top/gtrujtawyb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ydzc1.top/gtlqcidemc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigufen.top/gtoeernthj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hammf.cn/gtpqqqptlk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.nanxinkj.top/gtruvfzoqs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yuanzhike.top/gtwkydyypv.html

[B12] 跳出多层循环
来源：http://hz.xuanzx.com/gtvudivtyi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.meibo888.top/gtuwgnolzh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cdnleiting.top/gtzhekcdcb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daxiang520.top/gtlgkmrfef.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtxifgvfjc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cdnleiting.top/gtizcxqhrb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cashguo.top/gtxsszxdil.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.birdmap.top/gtsxshpgep.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gogol.net.cn/gttylnyjww.html

[B13] 判断是否为数字
来源：http://hz.guannengcc.top/gtbyfcquwl.html

Py:   isinstance(x, (int, float))
来源：http://hz.bjfxy.top/gtbsnriczy.html

PHP:  is_numeric($x)
来源：http://hz.redwolf501.top/gtgqhxkcnw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yongpay.top/gtbcbgmmwv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hysaishi.cn/gtepubjuaz.html

Java: x instanceof Number
来源：http://hz.chenjidiqi.icu/gtybtwhkmr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.0kj1m.cn/gtwsogdzkh.html

Ruby: x.is_a?(Numeric)
来源：http://hz.cdnleiting.top/gtngwkfqvq.html

C#:   x is int or double or decimal
来源：http://hz.jinghuilouyu.cn/gtwcilscvk.html

[B14] 判断值是否在集合内
来源：http://hz.shangyingyoupin.top/gtetblraxf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.andypj.xyz/gtkhoonszo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhixingplan.top/gtieehpnff.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.havefunace.top/gtoiqjavxd.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhoulong.xyz/gtcmvilvjg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yongpay.top/gtaqighmck.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shangyingyoupin.top/gtegvxzajp.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sysykeji.top/gtxfnhlrti.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cashguo.top/gtjeolcrzd.html

[B15] 布尔运算与取反
来源：http://hz.haohaochexian.top/gtatslurbp.html

Py:   a and b or not c
来源：http://hz.shanyushiyangtech.top/gtlzhbakys.html

PHP:  $a && $b || !$c
来源：http://hz.andypj.xyz/gtwcrfwxbt.html

JS:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtzwegkjiu.html

TS:   a && b || !c
来源：http://hz.yuanzhike.top/gttrmqkfvw.html

Java: a && b || !c
来源：http://hz.dianchejie.cn/gtinrkyizs.html

Go:   a && b || !c
来源：http://hz.birdmap.top/gtmhbosdcs.html

Ruby: a && b || !c
来源：http://hz.zhixingplan.top/gtnktshjnj.html

C#:   a && b || !c
来源：http://hz.cqqwz.cn/gtsuazedmd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cashguo.top/gtlagsiczd.html

Py:   if not data: return
来源：http://hz.yangfankeji.com/gtatwisane.html

PHP:  if (!$data) { return; }
来源：http://hz.yueranfly.top/gtcwalynjr.html

JS:   if (!data) return;
来源：http://hz.yuxming.cn/gteglgzuwp.html

TS:   if (!data) return;
来源：http://hz.316326.xyz/gtrnsslnhj.html

Java: if (data == null) return;
来源：http://hz.nanxuanxn.top/gtkabwjxyb.html

Go:   if data == nil { return }
来源：http://hz.yanxiufei.cn/gtdmnkmmql.html

Ruby: return if data.nil?
来源：http://hz.ivvv.top/gtwggxanwh.html

C#:   if (data == null) return;
来源：http://hz.zhoulong.xyz/gtdqrqcegr.html

================================================================================
来源：http://hz.sxryk.cn/gtwwfcsvdb.html

C. 函数与作用域
来源：http://hz.nanxuanxn.top/gtzyhlakam.html

================================================================================
来源：http://hz.daxiang520.top/gtsnlvdfzd.html

[C01] 定义函数
来源：http://hz.hammf.cn/gtqiiwdpup.html

Py:   def add(a, b): return a + b
来源：http://hz.hammf.cn/gtqeghkyye.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fzhhl.top/gtydajlxsq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.svipenyu.cn/gtyuchyxve.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gtxtwzoeek.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtlnzmzwfr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yuxming.cn/gtyqcpbykt.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhijiandao.cn/gtajbvvgfi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhengqikj.top/gtmqlppdwz.html

[C02] 默认参数
来源：http://hz.iojbl.cn/gtamsxvpuj.html

Py:   def greet(name="World"): return name
来源：http://hz.meibo888.top/gttyysjdkn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhaomingkeji.xyz/gtphncwitz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ybcxt.top/gtokgldrca.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.smart0.xyz/gtnrebstns.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.meibo888.top/gtypjxgtyo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhoulong.xyz/gtxtxiqldp.html

Ruby: def greet(name = "World") = name
来源：http://hz.andypj.xyz/gtpplwuehs.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhiwuduotai.top/gttnqnhwty.html

[C03] 可变参数
来源：http://hz.daria6918.cn/gtkmtyyyna.html

Py:   def total(*args): return sum(args)
来源：http://hz.xingfuxueyuan.xyz/gtgxcmjbsc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jlsjyb.cn/gtsijoqhpq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tianlin.xyz/gtsidylolg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daxiang520.top/gtrvezffjw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.9152youxi.cn/gtwfxbnino.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.andypj.xyz/gtbqlxsxiy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.vqdsnc.cn/gtypnqwncl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jqgfzy.top/gtvadakwhs.html

[C04] 命名参数 / 关键字参数
来源：http://hz.52xcode.cn/gtrtcpsopj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.bjfxy.top/gtokhjkglz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.316326.xyz/gtzzvdnvei.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yj202588.top/gtanikshis.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shanyushiyangtech.top/gtpwrzezsq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tian-w.cn/gtybiqpaqy.html

Go:   // 无：用配置结构体参数
来源：http://hz.ivvv.top/gtmtziwqgn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtniqwujwg.html

C#:   f(a: 1, b: 2)
来源：http://hz.52xcode.cn/gtszezqfgl.html

[C05] 返回多个值
来源：http://hz.cqqwz.cn/gtozdkmtdf.html

Py:   return a, b
来源：http://hz.tianlin.xyz/gtfcolqymk.html

PHP:  return [$a, $b];
来源：http://hz.pycfn.com/gttuoocrui.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.andypj.xyz/gtcpjhjaji.html

TS:   return { a, b };
来源：http://hz.hnxiangtu.top/gthjqxnsvs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nwbrower.top/gtcdomhfzd.html

Go:   return a, b
来源：http://hz.gogol.net.cn/gtvxlravew.html

Ruby: return a, b
来源：http://hz.ivvv.top/gtfujwgngn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.tian-w.cn/gtihnoemmm.html

[C06] 匿名函数 / lambda
来源：http://hz.jlsjyb.cn/gtpbstjdhx.html

Py:   square = lambda x: x * x
来源：http://hz.zhoulong.xyz/gtnxbtorwo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.iojbl.cn/gtfhpqdxla.html

JS:   const square = x => x * x;
来源：http://hz.tanke756.top/gthbuuvejb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xinyue.icu/gtyxgfaxbz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangshuangyany.cn/gtnxlanahg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.bjfxy.top/gtpuurpxxi.html

Ruby: square = ->(x) { x * x }
来源：http://hz.fzhhl.top/gtwaqsyger.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhaomingkeji.xyz/gtcsjlbqzv.html

[C07] 把函数作为参数传入
来源：http://hz.xylfe.cn/gtproomwky.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhaomingkeji.xyz/gtyuphvrto.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xuanzx.com/gtgppxvskl.html


<!-- 参考信息 -->