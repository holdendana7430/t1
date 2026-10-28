代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.cqqwz.cn/gtsbwylcih.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.zhiwuduotai.top/gtadarqgck.html

TS:   if (!x) {}
来源：http://hz.chenjidiqi.icu/gtnfvfvftq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.sxryk.cn/gtvtugqfji.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jlsjyb.cn/gtoncetxua.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.aizwys.cn/gtugelefzb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.nanxuanxn.top/gthghbqfky.html

[A17] 位运算
来源：http://hz.chenzaomai.com/gthypwkxxl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhixingplan.top/gtfatvueud.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.ppjwa.cn/gtlwjuylwq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yuxming.cn/gtuwitiweo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.yvedp.cn/gtaebztybg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tianlin.xyz/gtasjvthgp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zhoulong.xyz/gtbkmesfgt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.aibaodan.cn/gtjlkoiyfz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zdqjudy.top/gtwtqdxyip.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jinqigufen.top/gtceofwjiv.html

Py:   ord("A"); chr(65)
来源：http://hz.zhengqikj.top/gtxvfuofnj.html

PHP:  ord("A"); chr(65)
来源：http://hz.redwolf501.top/gtxlpuojfj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.ybcxt.top/gtrzfypmhf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.sysykeji.top/gttbdqanrq.html

Java: (int) 'A'; (char) 65
来源：http://hz.yangfankeji.com/gtnxxsemxm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.gotoacloud.top/gtucicvywj.html

Ruby: "A".ord; 65.chr
来源：http://hz.cheryme.top/gtnlxwjuia.html

C#:   (int)'A'; (char)65
来源：http://hz.zhaomingkeji.xyz/gtsobxhhyl.html

[A19] 交换两个变量
来源：http://hz.gzhubu.top/gtoksbfxeb.html

Py:   a, b = b, a
来源：http://hz.zdqjudy.top/gtvxxdhqoh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.tanke756.top/gtmedesbik.html

JS:   [a, b] = [b, a];
来源：http://hz.cucudq.cn/gtrmjhbpfb.html

TS:   [a, b] = [b, a];
来源：http://hz.bjfxy.top/gtshhlsrel.html

Java: int t = a; a = b; b = t;
来源：http://hz.yj20258.top/gtliinikpf.html

Go:   a, b = b, a
来源：http://hz.snrcjt.cn/gtfkfprmmb.html

Ruby: a, b = b, a
来源：http://hz.ehwqpu.com/gtqiwypdaj.html

C#:   (a, b) = (b, a);
来源：http://hz.nanxuanxn.top/gtimiqdiah.html

[A20] 读取标准输入
来源：http://hz.yongpay.top/gtolfqgadu.html

Py:   name = input("请输入：")
来源：http://hz.xuanzx.com/gtvegsykrn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.quarkkingdee.top/gtsqxsgqcf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.sufxvd.cn/gtsppkwqct.html

TS:   // Node.js：readline 模块
来源：http://hz.kuanghao11.cn/gteongkcbu.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zdqjudy.top/gtbtqlgksm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jyoumei.cn/gtcdbrryws.html

Ruby: gets.chomp
来源：http://hz.zhixingplan.top/gtclosjfth.html

C#:   Console.ReadLine();
来源：http://hz.cdnleiting.top/gtcnprulrs.html

[A21] 保留指定小数位输出
来源：http://hz.yuxming.cn/gtqdpakvvt.html

Py:   f"{3.14159:.2f}"
来源：http://hz.cqqwz.cn/gtxgmquooi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.wangdashe.top/gtjkjuvblv.html

JS:   (3.14159).toFixed(2)
来源：http://hz.cqqwz.cn/gttntxglnv.html

TS:   (3.14159).toFixed(2)
来源：http://hz.meibo888.top/gtcywkptnl.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.cheryme.top/gtliijtgnw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jyoumei.cn/gthjvmmfcp.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.jlsjyb.cn/gtsrsahtkp.html

C#:   3.14159.ToString("F2")
来源：http://hz.cqqwz.cn/gtvxuofcmh.html

[A22] 获取字符串长度
来源：http://hz.shzxlz.cn/gthsjomrec.html

Py:   len(s)
来源：http://hz.xuanzx.com/gtxzftvflb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.sweek.top/gtbiqdvyxf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.birdmap.top/gtytjeptjs.html

TS:   s.length
来源：http://hz.guannengcc.top/gtlstrduhv.html

Java: s.length()
来源：http://hz.hnxiangtu.top/gtftlcqkie.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.jyoumei.cn/gtujudmnle.html

Ruby: s.length
来源：http://hz.316326.xyz/gtgdtvfcyq.html

C#:   s.Length
来源：http://hz.ydzc1.top/gtwwuyaswi.html

[A23] 大小写转换
来源：http://hz.sufxvd.cn/gtklayyiqj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.ydjk.org.cn/gtgpdwsynu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yanxiufei.cn/gtsfobgjsj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jinqigufen.top/gtflhzawok.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yonumen.top/gtjvbizkqo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.tianlin.xyz/gttguduohg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.xingfuxueyuan.xyz/gtgwlfinlj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yueranfly.top/gthzqeapvv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.quarkkingdee.top/gtkxkxabvx.html

[A24] 去除首尾空白
来源：http://hz.hongshengwenyu.top/gtdqefrlev.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.haohaochexian.top/gtenbbqczv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.guannengcc.top/gtqmdzuwhu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gotoacloud.top/gtpdhggxkr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jiagoushi.top/gtdfultgkv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.svipenyu.cn/gtkoeasprd.html

Go:   strings.TrimSpace(s)
来源：http://hz.jinyuanbaomall.cn/gtgkfcegue.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yangfankeji.com/gtocoqgiuc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.chenlongwang.top/gtpfbgdkca.html

[A25] 字符串比较
来源：http://hz.ppjwa.cn/gtoyzprekc.html

Py:   s1 == s2; s1 != s2
来源：http://hz.quarkkingdee.top/gtdosnrjmv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.feifeiyinyue.top/gtxsnswvrq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.guowangkeji.top/gtefveftmx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.feifeiyinyue.top/gtcdwjwawf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.tian-w.cn/gtfviejhkb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.aibaodan.cn/gttofppczz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.iojbl.cn/gtukjarwxd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.nanxuanxn.top/gtgjrukfkx.html

[A26] 类型转换总览
来源：http://hz.zdqjudy.top/gteuzxomgi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.chenjidiqi.icu/gtyghrrzcq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.pengpengdd.cyou/gtlqozogmw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.tianlin.xyz/gtwiwojdma.html

TS:   Number() String() Boolean() x as number
来源：http://hz.gaohongyu789.top/gtngrsgszj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.ivvv.top/gthqonbxve.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.sweek.top/gtawbpsvnz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.redwolf501.top/gtadiqhoct.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yuanzhike.top/gtknjwxxxr.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxrdfohic.html

B. 流程控制
来源：http://hz.jinyuanbaomall.cn/gtmwzaxnze.html

================================================================================
来源：http://hz.sysykeji.top/gtqcgjtuoh.html

[B01] 条件判断 if / else
来源：http://hz.hfpthk.cn/gtelqubeti.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zycfv.cn/gtyceobzwf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.haohaochexian.top/gtnkpcwupl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.bjfxy.top/gtidqktyca.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.smart0.xyz/gtlckzwxps.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hywenlv.cn/gtsqmimjqn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hfpthk.cn/gtbtqkynab.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.tianlin.xyz/gtmsxyrcel.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.ybcxt.top/gtwvlkvxtk.html

[B02] 多分支 else if / elif
来源：http://hz.shangyingyoupin.top/gtgascupgy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zycfv.cn/gtavpzgrez.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yj202588.top/gtuoxisnra.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ybcxt.top/gtuoxlzmej.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hfpthk.cn/gtwhgyqdzy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guowangkeji.top/gttzjmslao.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.hfpthk.cn/gtcyagxlsd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.daxiang520.top/gtgvcnlpbj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydjk.org.cn/gtangdixah.html

[B03] switch / match / case
来源：http://hz.cqqwz.cn/gtvifpzkot.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hammf.cn/gttnwtdifc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.dashuyun.cn/gtnnhevinj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gogol.net.cn/gtegjodrjz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.tanke756.top/gtvubsqwlu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.hysaishi.cn/gttakskjvm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.quarkkingdee.top/gtphxvyhwt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yuxming.cn/gtbsftgdea.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.sxryk.cn/gtrjpstduz.html

[B04] for 计数循环
来源：http://hz.vqdsnc.cn/gtspxsrzfb.html

Py:   for i in range(10): print(i)
来源：http://hz.fengsongda.top/gtnifzqxve.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.bjfxy.top/gtvpadzazx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.smart0.xyz/gtsuwfwmhx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.nanxuanxn.top/gtfvclcgcy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.feifeiyinyue.top/gtsgscxfpl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yangfankeji.com/gtfcmsgqwq.html

Ruby: 10.times { |i| puts i }
来源：http://hz.sweek.top/gtnjwlfyqy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.fzhhl.top/gtlgoidkoo.html

[B05] 遍历数组 / 列表
来源：http://hz.hongshengwenyu.top/gtxobbwjqa.html

Py:   for item in arr: print(item)
来源：http://hz.andypj.xyz/gtetdsjfoq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ybcxt.top/gtvgocxwlw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenzaomai.com/gtefhqncsg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xinyue.icu/gtmpddckbf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.pengpengdd.cyou/gtopzsloft.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.wangshuangyany.cn/gtrmoflmsd.html

Ruby: arr.each { |item| puts item }
来源：http://hz.dashuyun.cn/gtdyqcneyz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jinqigfzy.top/gtaunyncvg.html

[B06] 遍历字典 / 对象
来源：http://hz.wangdashe.top/gtpygcuhur.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.shangyingyoupin.top/gtrpkdvftv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.mhx1999.top/gtvdobxvbs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.bjfxy.top/gtdbdhnbya.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hnqzz.top/gtsdmqnxop.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yj20258888.top/gtzesbdnbm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.316326.xyz/gtemrqxkgn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.mhx1999.top/gtikyhwetk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.tian-w.cn/gtkzufndgp.html

[B07] while 循环
来源：http://hz.hnqzz.top/gtfxqcburu.html

Py:   while i < 10: i += 1
来源：http://hz.zhaomingkeji.xyz/gtwwsziflf.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zhoulong.xyz/gttczrxiru.html

JS:   while (i < 10) { i++; }
来源：http://hz.cashguo.top/gtbrkrojfb.html

TS:   while (i < 10) { i++; }
来源：http://hz.nanxinkj.top/gtuhhpmyuy.html

Java: while (i < 10) { i++; }
来源：http://hz.aibaodan.cn/gtffslrxzs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.gzhubu.top/gtgbzfdrrb.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhaomingkeji.xyz/gtcymdvilu.html

C#:   while (i < 10) { i++; }
来源：http://hz.ivvv.top/gtgnupzxuw.html

[B08] do-while（至少执行一次）
来源：http://hz.zdqjudy.top/gtptlmtfli.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.smart0.xyz/gthajhtirj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhiwuduotai.top/gtaiklbrqo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yangfankeji.com/gtvjbhkuij.html

TS:   do { i++; } while (i < 10);
来源：http://hz.c1oappe.top/gthkxiqdbt.html

Java: do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gttylykyrq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.dashuyun.cn/gtiohfxgav.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hongshengwenyu.top/gtoewjbyor.html

C#:   do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gtxinsivvp.html

[B09] break 与 continue
来源：http://hz.shangyingyoupin.top/gttsunynaz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shanyushiyangtech.top/gtqudrxukz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jqgfzy.top/gtozlevyfw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zdqjudy.top/gtkqaqmvdv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jyoumei.cn/gtecotdiuw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cqqwz.cn/gtgyvgdtwe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hywenlv.cn/gtwompdmfr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ydjk.org.cn/gtkvhsykga.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tian-w.cn/gtmtjbdsyq.html

[B10] 遍历同时拿索引
来源：http://hz.andypj.xyz/gtualtgfac.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xuetiantiany.cn/gtvclnprgr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jinghuilouyu.cn/gtcftvztkr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.cashguo.top/gtzsbvorgz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.fengsongda.top/gtdldkyzsw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.nwbrower.top/gtsewjaxoc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jyoumei.cn/gtmsypgqqo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xuetiantiany.cn/gtpwkgkxij.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shangyingyoupin.top/gtgygdeouv.html

[B11] 生成数字序列 / 区间
来源：http://hz.cheryme.top/gtrgwnjyrw.html

Py:   list(range(0, 10, 2))
来源：http://hz.snrcjt.cn/gtmvnruwrh.html

PHP:  range(0, 10, 2);
来源：http://hz.yj20258.top/gtaearomqz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.c1oappe.top/gtwridaupa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zdqjudy.top/gtrluvktpa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.snrcjt.cn/gtzaxhgrnz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.guowangkeji.top/gtnfclufse.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zdqjudy.top/gtzjkipzzu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.sysykeji.top/gtoojgtwbi.html

[B12] 跳出多层循环
来源：http://hz.gogol.net.cn/gtloywzpwl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gzhubu.top/gtswtquuaw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.aibaodan.cn/gtbeiyxmxi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtlgtwwyng.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gtytjzzebj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgfzy.top/gtijuwlsju.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.c1oappe.top/gtzhpdlniu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.guannengcc.top/gtqglxxhww.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.guannengcc.top/gtdysdsewk.html

[B13] 判断是否为数字
来源：http://hz.yueranfly.top/gtbrmyhcpp.html

Py:   isinstance(x, (int, float))
来源：http://hz.sweek.top/gtyozqrlbn.html

PHP:  is_numeric($x)
来源：http://hz.shanyushiyangkeji.top/gtlfntwbbo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shuidangran.top/gtpqvpsbca.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nwbrower.top/gthgthjfzm.html

Java: x instanceof Number
来源：http://hz.sxryk.cn/gtnqzlbfvb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ehwqpu.com/gtxmnxghpq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.fengsongda.top/gthxfiokar.html

C#:   x is int or double or decimal
来源：http://hz.sxryk.cn/gtefjqajkk.html

[B14] 判断值是否在集合内
来源：http://hz.yanxiufei.cn/gtbjbtmseu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinqigfzy.top/gtjkomcrnw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.bjfxy.top/gtfzmkqwxl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangtech.top/gtjucukjin.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hongshengwenyu.top/gtmigsjlsu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jlsjyb.cn/gthmdjndsf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.gzhubu.top/gtidvtnzip.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ydzc1.top/gtnvvwoali.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhixingplan.top/gtwfxalhvy.html

[B15] 布尔运算与取反
来源：http://hz.tianlin.xyz/gtnjoxjqwg.html

Py:   a and b or not c
来源：http://hz.nwbrower.top/gtatjwydnm.html

PHP:  $a && $b || !$c
来源：http://hz.iojbl.cn/gtuzoaiyem.html

JS:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtagpwaiyd.html

TS:   a && b || !c
来源：http://hz.haohaochexian.top/gtcldapnuz.html

Java: a && b || !c
来源：http://hz.gzhubu.top/gthyatqpbd.html

Go:   a && b || !c
来源：http://hz.gogol.net.cn/gtcxbmpejn.html

Ruby: a && b || !c
来源：http://hz.zhengqikj.top/gtxdflgimo.html

C#:   a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtvkxgytxu.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xuanzx.com/gtgbfwlbxs.html

Py:   if not data: return
来源：http://hz.zycfv.cn/gtsurlzgbf.html

PHP:  if (!$data) { return; }
来源：http://hz.316326.xyz/gtybdruzxd.html

JS:   if (!data) return;
来源：http://hz.xuetiantiany.cn/gtqbftbjjq.html

TS:   if (!data) return;
来源：http://hz.meibo888.top/gtsiwdojaw.html

Java: if (data == null) return;
来源：http://hz.svipenyu.cn/gtfqlmwyuw.html

Go:   if data == nil { return }
来源：http://hz.cqqwz.cn/gtgukhzfzf.html

Ruby: return if data.nil?
来源：http://hz.chenjidiqi.icu/gttcnvwgoe.html

C#:   if (data == null) return;
来源：http://hz.zhaomingkeji.xyz/gtgssmnfca.html

================================================================================
来源：http://hz.daxiang520.top/gtodpiudxw.html

C. 函数与作用域
来源：http://hz.zhijiandao.cn/gtvevlpkgf.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtmsxwwsqq.html

[C01] 定义函数
来源：http://hz.yj20258.top/gtuuommdat.html

Py:   def add(a, b): return a + b
来源：http://hz.cheryme.top/gtbgzfukbw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhijiandao.cn/gtmbvucrbq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtbmayixjs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258.top/gtyokseyph.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtqjpulwhs.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yj20258888.top/gtxhrrfcef.html

Ruby: def add(a, b); a + b; end
来源：http://hz.quarkkingdee.top/gtghzsbkvt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtutpfbgwe.html

[C02] 默认参数
来源：http://hz.zdqjudy.top/gtotnodqmu.html

Py:   def greet(name="World"): return name
来源：http://hz.yj20258888.top/gtfxdqghgo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.dashuyun.cn/gtymlzpszs.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ehwqpu.com/gtmjvtqvgt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jqgfzy.top/gtdwkbppty.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.quarkkingdee.top/gtdfklqkjy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jyoumei.cn/gtwsipkipe.html

Ruby: def greet(name = "World") = name
来源：http://hz.snrcjt.cn/gtibluwqeh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj202588.top/gtlgttxvxb.html

[C03] 可变参数
来源：http://hz.nanxuanxn.top/gtqrkfaebn.html

Py:   def total(*args): return sum(args)
来源：http://hz.ybcxt.top/gtuygeaikm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.pycfn.com/gtgnzsnymc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yangfankeji.com/gtqvnynpzg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinqigufen.top/gtgwmkdbkf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.quarkkingdee.top/gtkgvujoab.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shanyushiyangkeji.top/gtfrdpnwuy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ppjwa.cn/gtlgaisvve.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cheryme.top/gteptsinxv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jyoumei.cn/gtmlylltmx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.haohaochexian.top/gtzedkwukl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jqgfzy.top/gtnyevtood.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.havefunace.top/gtuyqgfcso.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ppjwa.cn/gtmhetnxeb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tian-w.cn/gtaguyyrff.html

Go:   // 无：用配置结构体参数
来源：http://hz.shuidangran.top/gtxszuqieh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zdqjudy.top/gtjrgtzhbg.html

C#:   f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtnzpunhtm.html

[C05] 返回多个值
来源：http://hz.cashguo.top/gtrystpbnl.html

Py:   return a, b
来源：http://hz.shuidangran.top/gtldomsfgd.html

PHP:  return [$a, $b];
来源：http://hz.gogol.net.cn/gtkgqkpstm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.birdmap.top/gtclewmgsf.html

TS:   return { a, b };
来源：http://hz.hysaishi.cn/gtumsikryc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yuanzhike.top/gtkhrviieh.html

Go:   return a, b
来源：http://hz.hnxiangtu.top/gtiozjrepy.html

Ruby: return a, b
来源：http://hz.zhijiandao.cn/gtmutsxkqt.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.chenjidiqi.icu/gtedwwkknz.html

[C06] 匿名函数 / lambda
来源：http://hz.cheryme.top/gtqacwvjqw.html

Py:   square = lambda x: x * x
来源：http://hz.cashguo.top/gtogexjqfd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.wangshuangyany.cn/gtgfixhazx.html

JS:   const square = x => x * x;
来源：http://hz.ydzc1.top/gtwhsaznlo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhixingplan.top/gtkcqyvgio.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.feifeiyinyue.top/gtmasedosk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.guowangkeji.top/gtkckaoukq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xingfuxueyuan.xyz/gtxwtikflm.html


<!-- 参考信息 -->