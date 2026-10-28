代发 wailian999

Ruby: value = data || "默认值"
来源：http://hz.zhengqikj.top/gtsnvsufve.html

C#:   var value = data ?? "默认值";
来源：http://hz.316326.xyz/gtqrmyjcdq.html

[A16] 真假值判断规则
来源：http://hz.sufxvd.cn/gtpczawgvh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.cheryme.top/gtuwporair.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.wangdashe.top/gtheyxxalz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.xinyue.icu/gtsuddcrbn.html

TS:   if (!x) {}
来源：http://hz.gotoacloud.top/gtkkmdjfji.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.shzxlz.cn/gtnqjmgqzr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yonumen.top/gtcrdklbhf.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.ydzc1.top/gtocnetqhs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.shanyushiyangkeji.top/gtdlrimzqf.html

[A17] 位运算
来源：http://hz.vqdsnc.cn/gtezlljynr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.0kj1m.cn/gthslbgexg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yanxiufei.cn/gtlqeelmii.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xuanzx.com/gtjuatuytp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.mhx1999.top/gtyhgfnuon.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenjidiqi.icu/gtakyplyrp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.ydzc1.top/gtiejfodbz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ywan-chungtsiang.top/gtdifmdvvw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.snrcjt.cn/gturvzlaop.html

[A18] 字符与 ASCII 码互转
来源：http://hz.yj20258.top/gtgxrwrwnx.html

Py:   ord("A"); chr(65)
来源：http://hz.chenzaomai.com/gtiwxhhsny.html

PHP:  ord("A"); chr(65)
来源：http://hz.fzhhl.top/gtpvwcplcw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.ivvv.top/gtcpslukgv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.nanxuanxn.top/gtetrrxpyt.html

Java: (int) 'A'; (char) 65
来源：http://hz.jyoumei.cn/gtphysqduo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.jiagoushi.top/gtkloxmwzs.html

Ruby: "A".ord; 65.chr
来源：http://hz.hnqzz.top/gtehjmhjgs.html

C#:   (int)'A'; (char)65
来源：http://hz.hfpthk.cn/gtqjsvvuff.html

[A19] 交换两个变量
来源：http://hz.shanyushiyangtech.top/gtcdboaxta.html

Py:   a, b = b, a
来源：http://hz.snrcjt.cn/gtqjbyjlre.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.tianlin.xyz/gtrvxkkkem.html

JS:   [a, b] = [b, a];
来源：http://hz.tian-w.cn/gtbmgqotdm.html

TS:   [a, b] = [b, a];
来源：http://hz.yongpay.top/gtrdogvutw.html

Java: int t = a; a = b; b = t;
来源：http://hz.ppjwa.cn/gtzzhogtyv.html

Go:   a, b = b, a
来源：http://hz.sysykeji.top/gtevmpgfih.html

Ruby: a, b = b, a
来源：http://hz.andypj.xyz/gtcjvsnftp.html

C#:   (a, b) = (b, a);
来源：http://hz.zhengqikj.top/gttgxvqphb.html

[A20] 读取标准输入
来源：http://hz.fzhhl.top/gtuqpbgkbf.html

Py:   name = input("请输入：")
来源：http://hz.hywenlv.cn/gtewbdmdsk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.yj20258.top/gtrqeuvefk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.sweek.top/gtzmfslksm.html

TS:   // Node.js：readline 模块
来源：http://hz.jiagoushi.top/gtaxaxrjxo.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.jqgfzy.top/gtoadbawuv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.hywenlv.cn/gtefrqtviv.html

Ruby: gets.chomp
来源：http://hz.tian-w.cn/gtouylknek.html

C#:   Console.ReadLine();
来源：http://hz.xylfe.cn/gtqjkjootn.html

[A21] 保留指定小数位输出
来源：http://hz.fzhhl.top/gtdraktqkg.html

Py:   f"{3.14159:.2f}"
来源：http://hz.hongshengwenyu.top/gtrvjlbaoy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.ybcxt.top/gtcnvusckz.html

JS:   (3.14159).toFixed(2)
来源：http://hz.sufxvd.cn/gthemzzpol.html

TS:   (3.14159).toFixed(2)
来源：http://hz.dianchejie.cn/gtxjscwgxw.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.meibo888.top/gthwrvkxtr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.sysykeji.top/gtuakpblky.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.52xcode.cn/gtaapugaks.html

C#:   3.14159.ToString("F2")
来源：http://hz.0kj1m.cn/gtvvrrrwep.html

[A22] 获取字符串长度
来源：http://hz.jiagoushi.top/gtlznavwbx.html

Py:   len(s)
来源：http://hz.ybcxt.top/gtetastyxd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yangfankeji.com/gticntyjhs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.kuanghao11.cn/gtwruxojyx.html

TS:   s.length
来源：http://hz.daxiang520.top/gtopkjmwno.html

Java: s.length()
来源：http://hz.jyoumei.cn/gtkksvtrys.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.meibo888.top/gtjldkvcml.html

Ruby: s.length
来源：http://hz.zhengqikj.top/gtgjtekamy.html

C#:   s.Length
来源：http://hz.jlsjyb.cn/gtalryjfck.html

[A23] 大小写转换
来源：http://hz.cashguo.top/gtadmigwvf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.chenzaomai.com/gtlhivgsya.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yongpay.top/gthosxeqph.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.gogol.net.cn/gtnhggmodr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.fengsongda.top/gthalkaluy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenlongwang.top/gtjbctglxs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.9152youxi.cn/gtppuzrmae.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xziqi.cn/gtkeqbhakv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.aizwys.cn/gttytcihvx.html

[A24] 去除首尾空白
来源：http://hz.bjfxy.top/gtoazndlwa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.ybcxt.top/gtfsmbyvlk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.quarkkingdee.top/gtcipgezxo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hywenlv.cn/gtdjqdkyxx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhijiandao.cn/gtedvmsreq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jinghuilouyu.cn/gtctmocjog.html

Go:   strings.TrimSpace(s)
来源：http://hz.haohaochexian.top/gtddkolzxy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zycfv.cn/gthrmtbucv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.havefunace.top/gtfjnosgfs.html

[A25] 字符串比较
来源：http://hz.shuidangran.top/gtswfvhqzi.html

Py:   s1 == s2; s1 != s2
来源：http://hz.wangdashe.top/gtzwavxile.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jinghuilouyu.cn/gtcyjmqbuu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hfpthk.cn/gtpvlxcuzn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.nanxuanxn.top/gtjshlflyp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.chenzaomai.com/gtetvcuetp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.9152youxi.cn/gtvrkfaasx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ehwqpu.com/gtrjeclbpq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.zhaomingkeji.xyz/gteguqgqfx.html

[A26] 类型转换总览
来源：http://hz.shangyingyoupin.top/gtyxpjmgwl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.gotoacloud.top/gtztmbvyxl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.sysykeji.top/gtuwwizsuu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yanxiufei.cn/gtbkhdgnfz.html

TS:   Number() String() Boolean() x as number
来源：http://hz.ywan-chungtsiang.top/gtulycbcor.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.aibaodan.cn/gtgtshfccs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.sysykeji.top/gtjrcqpdij.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yuanzhike.top/gtgcvszoyt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.xingfuxueyuan.xyz/gtunonmblz.html

================================================================================
来源：http://hz.tianlin.xyz/gtdcybdgfi.html

B. 流程控制
来源：http://hz.andypj.xyz/gtupcblfkd.html

================================================================================
来源：http://hz.andypj.xyz/gtvkzqmtlf.html

[B01] 条件判断 if / else
来源：http://hz.xingfuxueyuan.xyz/gtibakyadz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.shanyushiyangkeji.top/gtigxdgmmf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.snrcjt.cn/gtqcmgjujg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cqqwz.cn/gtykiohout.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.birdmap.top/gtzcdlybgw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.sufxvd.cn/gthqwkoxeo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhixingplan.top/gtipcgmxke.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.bjfxy.top/gtdcllltme.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.cqqwz.cn/gtabxhtona.html

[B02] 多分支 else if / elif
来源：http://hz.daria6918.cn/gtirkwzvxi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.nanxinkj.top/gtknojesgw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.xziqi.cn/gttzglwcav.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cucudq.cn/gttyjstrjl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gogol.net.cn/gtmupataao.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yangfankeji.com/gtyxecsppe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yj20258.top/gturziixhy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.pengpengdd.cyou/gtmpknybqq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.iojbl.cn/gtofcybrjm.html

[B03] switch / match / case
来源：http://hz.havefunace.top/gthrjwcple.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yj20258.top/gtfybnvfta.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.shangyingyoupin.top/gtqaksjuuj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yonumen.top/gtnctlfrvf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenzaomai.com/gtcsxengyl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.cqqwz.cn/gtmjkgyclh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.xuetiantiany.cn/gtrfbqvzbq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yueranfly.top/gtbmfngzee.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.guannengcc.top/gtablcjnng.html

[B04] for 计数循环
来源：http://hz.cdnleiting.top/gtlkxkjvxl.html

Py:   for i in range(10): print(i)
来源：http://hz.shanyushiyangkeji.top/gtyvdkxnmz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.fzhhl.top/gtujshabxt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pengpengdd.cyou/gtwulkipbb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cdnleiting.top/gtfzenqqsk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.tanke756.top/gtcqxumjhw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.gaohongyu789.top/gtjvwxqbsb.html

Ruby: 10.times { |i| puts i }
来源：http://hz.birdmap.top/gtwhquajum.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhaomingkeji.xyz/gtqnhhjfwi.html

[B05] 遍历数组 / 列表
来源：http://hz.yonumen.top/gttswsbtqv.html

Py:   for item in arr: print(item)
来源：http://hz.guannengcc.top/gtbyqunths.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jyoumei.cn/gtqrqgpjps.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.sufxvd.cn/gtppvqfmzo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhongyouzk.top/gtpzzyvycq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.9152youxi.cn/gttromtmyn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.316326.xyz/gtcddpyvol.html

Ruby: arr.each { |item| puts item }
来源：http://hz.shuidangran.top/gtdhrwmjjb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.aibaodan.cn/gtyktkccco.html

[B06] 遍历字典 / 对象
来源：http://hz.dashuyun.cn/gtzgurwqgs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.vqdsnc.cn/gthyzszcmr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.vqdsnc.cn/gtzekxmvng.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.redwolf501.top/gtjofmzhie.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.pycfn.com/gtfxphkyjm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.guannengcc.top/gtoybgiwip.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zycfv.cn/gtpouxsdch.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.chenzaomai.com/gtgjpdvkml.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jiagoushi.top/gtdyvnppgg.html

[B07] while 循环
来源：http://hz.bjfxy.top/gtncjansmo.html

Py:   while i < 10: i += 1
来源：http://hz.ppjwa.cn/gtbzrggmsc.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jinqigufen.top/gthtghkiob.html

JS:   while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtxuuliasl.html

TS:   while (i < 10) { i++; }
来源：http://hz.jinqigufen.top/gtwldtfchx.html

Java: while (i < 10) { i++; }
来源：http://hz.fengsongda.top/gtuvnwqbye.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.gotoacloud.top/gttbieplpn.html

Ruby: while i < 10; i += 1; end
来源：http://hz.quarkkingdee.top/gtizjjafrr.html

C#:   while (i < 10) { i++; }
来源：http://hz.tianlin.xyz/gtnwyabkaq.html

[B08] do-while（至少执行一次）
来源：http://hz.dashuyun.cn/gtcxwduvrm.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cheryme.top/gtatphgcwg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhoulong.xyz/gtfqwmztew.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yonumen.top/gtgbunagxt.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtehxwxkms.html

Java: do { i++; } while (i < 10);
来源：http://hz.xingfuxueyuan.xyz/gtktjumvxb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.pengpengdd.cyou/gtkujizjei.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhengqikj.top/gtnvbbfnbe.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ydjk.org.cn/gtnudftggf.html

[B09] break 与 continue
来源：http://hz.xingfuxueyuan.xyz/gtpjjbadun.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cdnleiting.top/gtovxohtqg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.c1oappe.top/gtofhbocsb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtqpgnmaxj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenzaomai.com/gtosrvyumd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtqvikaxut.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ehwqpu.com/gtcxaigmzg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ivvv.top/gttuzuctny.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jiagoushi.top/gtqwwmepke.html

[B10] 遍历同时拿索引
来源：http://hz.dashuyun.cn/gtcysfvzux.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cdnleiting.top/gtzdocjmuk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zycfv.cn/gtbxmctuvr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jinqigufen.top/gtxdnplxvi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jiagoushi.top/gttrzqxzpc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.nanxuanxn.top/gthlzyqefo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.guowangkeji.top/gttqxznmhn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zycfv.cn/gtvtsshjir.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.redwolf501.top/gtzojxkdoi.html

[B11] 生成数字序列 / 区间
来源：http://hz.snrcjt.cn/gtorrwulcr.html

Py:   list(range(0, 10, 2))
来源：http://hz.hfpthk.cn/gtfihaikpr.html

PHP:  range(0, 10, 2);
来源：http://hz.dashuyun.cn/gtlyaclmmk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cashguo.top/gtyhiqbkbb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hywenlv.cn/gtxjtqkblp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigufen.top/gthsqjtrmt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gogol.net.cn/gtulxewayp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yuanzhike.top/gtyzxleaxq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.gaohongyu789.top/gtfftpgewq.html

[B12] 跳出多层循环
来源：http://hz.ywan-chungtsiang.top/gtjmzkiihi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nanxinkj.top/gtlvczfoef.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jiagoushi.top/gtowhpbhwb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtiiokcgpt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gtfnysjqbc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gttzqjamzb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ehwqpu.com/gtnrghzedx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.fzhhl.top/gtuawgehhu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xziqi.cn/gtuzszdvwi.html

[B13] 判断是否为数字
来源：http://hz.birdmap.top/gtxfefdvwn.html

Py:   isinstance(x, (int, float))
来源：http://hz.nanxinkj.top/gtlshchkvg.html

PHP:  is_numeric($x)
来源：http://hz.xingfuxueyuan.xyz/gtnjjagmyd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.meibo888.top/gtrnyebjqp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydzc1.top/gtdvmqwfyd.html

Java: x instanceof Number
来源：http://hz.mhx1999.top/gtncqupizu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.aizwys.cn/gtivvwebim.html

Ruby: x.is_a?(Numeric)
来源：http://hz.wangdashe.top/gtlocdfwxz.html

C#:   x is int or double or decimal
来源：http://hz.guannengcc.top/gtafrlnkhv.html

[B14] 判断值是否在集合内
来源：http://hz.gotoacloud.top/gtpioxnfqw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yvedp.cn/gtilmdjejt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.birdmap.top/gtfjiknzig.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhixingplan.top/gtdrdodiys.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.meibo888.top/gtbconuizu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yj20258888.top/gttfpaigad.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guannengcc.top/gtdbvtozwh.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cqqwz.cn/gtfkfoskun.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jianghu66.top/gtajhxfkiw.html

[B15] 布尔运算与取反
来源：http://hz.smart0.xyz/gtcgiovpyn.html

Py:   a and b or not c
来源：http://hz.zhengqikj.top/gtgundwzyq.html

PHP:  $a && $b || !$c
来源：http://hz.yj20258.top/gtlkjyfnxi.html

JS:   a && b || !c
来源：http://hz.ivvv.top/gtrsnqtaes.html

TS:   a && b || !c
来源：http://hz.xylfe.cn/gtdzjtigii.html

Java: a && b || !c
来源：http://hz.dashuyun.cn/gtxwjfayix.html

Go:   a && b || !c
来源：http://hz.shzxlz.cn/gtkponiopc.html

Ruby: a && b || !c
来源：http://hz.jlsjyb.cn/gttzeoujly.html

C#:   a && b || !c
来源：http://hz.nwbrower.top/gtstkxsxki.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tianlin.xyz/gtdxchcbuo.html

Py:   if not data: return
来源：http://hz.sxryk.cn/gtxqpgoqlr.html

PHP:  if (!$data) { return; }
来源：http://hz.gaohongyu789.top/gtubwfczed.html

JS:   if (!data) return;
来源：http://hz.wangshuangyany.cn/gtjhdhzybj.html

TS:   if (!data) return;
来源：http://hz.hongshengwenyu.top/gtosjnyzlt.html

Java: if (data == null) return;
来源：http://hz.zhijiandao.cn/gtygkyytix.html

Go:   if data == nil { return }
来源：http://hz.jyoumei.cn/gtyriwqaot.html

Ruby: return if data.nil?
来源：http://hz.0kj1m.cn/gtnpnuqmhr.html

C#:   if (data == null) return;
来源：http://hz.wangdashe.top/gtqriduhai.html

================================================================================
来源：http://hz.zhijiandao.cn/gtrwwbtpoa.html

C. 函数与作用域
来源：http://hz.ivvv.top/gtydztngvd.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtayqpynoh.html

[C01] 定义函数
来源：http://hz.cheryme.top/gtzjmlicec.html

Py:   def add(a, b): return a + b
来源：http://hz.tianlin.xyz/gtbdybmkbz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtdpkvkatj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zycfv.cn/gttnwsrvcy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.mhx1999.top/gtwjedcjfm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gtedwszsnl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hnqzz.top/gtmuvtpzeu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.andypj.xyz/gtqjctdpis.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gtqhtqlwkx.html

[C02] 默认参数
来源：http://hz.tian-w.cn/gtuwkouomj.html

Py:   def greet(name="World"): return name
来源：http://hz.ivvv.top/gtiirqyztb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fengsongda.top/gttnmmtzwe.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinqigufen.top/gteakxnqkc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinyuanbaomall.cn/gtwayrjqvu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.havefunace.top/gtvsdkyzlw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ehwqpu.com/gtmyurerwp.html

Ruby: def greet(name = "World") = name
来源：http://hz.xuetiantiany.cn/gtmxlgowhd.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nanxinkj.top/gtdtdyvuyo.html

[C03] 可变参数
来源：http://hz.chenlongwang.top/gtefuqnqbn.html

Py:   def total(*args): return sum(args)
来源：http://hz.jlsjyb.cn/gttgevqxpj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sxryk.cn/gtaaiwrsus.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yangfankeji.com/gtexwvyisj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenzaomai.com/gttomboteu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cucudq.cn/gtkycvsnpu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yangfankeji.com/gtsqbonykh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.guannengcc.top/gtwikwpusy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ivvv.top/gtnekibbpg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xuetiantiany.cn/gtkiypsbji.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hnxiangtu.top/gtftmjwgdn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shanyushiyangtech.top/gtgmlpxsek.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gogol.net.cn/gtodygkcbn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhoulong.xyz/gtdgrgpbst.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.nanxinkj.top/gtvgefdczr.html

Go:   // 无：用配置结构体参数
来源：http://hz.jyoumei.cn/gtikgkxfni.html

Ruby: f(a: 1, b: 2)
来源：http://hz.316326.xyz/gtqnwsdmuj.html

C#:   f(a: 1, b: 2)
来源：http://hz.gzhubu.top/gtawosowxj.html

[C05] 返回多个值
来源：http://hz.pengpengdd.cyou/gtirbvfurr.html

Py:   return a, b
来源：http://hz.yongpay.top/gtafseoaac.html

PHP:  return [$a, $b];
来源：http://hz.zhixingplan.top/gthkfhbqar.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.smart0.xyz/gtimtveqpl.html

TS:   return { a, b };
来源：http://hz.zhoulong.xyz/gthrpolmcn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.9152youxi.cn/gtddbwihuz.html

Go:   return a, b
来源：http://hz.guannengcc.top/gtbryydbza.html

Ruby: return a, b
来源：http://hz.svipenyu.cn/gtjnltphvl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj20258.top/gtlxcbrypc.html

[C06] 匿名函数 / lambda
来源：http://hz.xuetiantiany.cn/gtchfavdld.html

Py:   square = lambda x: x * x
来源：http://hz.yj20258.top/gtdueawuzp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.daria6918.cn/gtugksxnsn.html

JS:   const square = x => x * x;
来源：http://hz.xingfuxueyuan.xyz/gthasneujc.html


<!-- 参考信息 -->